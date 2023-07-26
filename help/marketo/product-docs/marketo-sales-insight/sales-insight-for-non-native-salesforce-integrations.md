---
unique-page-id: 45417125
description: Sales Insight for Non-Native Salesforce集成 — Marketo文档 — 产品文档
title: Sales Insight for Non-Native Salesforce集成
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 0%

---

# Sales Insight for Non-Native Salesforce集成 {#sales-insight-for-non-native-salesforce-integrations}

如果您的Adobe Marketo Engage帐户是通过自定义或非本机集成连接到Salesforce，请使用本文配置Sales Insight。

>[!PREREQUISITES]
>
>* 在开始设置MSI之前，已为您的Marketo实例启用“MSI非本地”功能。 如果不是，并且您已购买该功能，请联系 [Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. 如果您尚未购买此功能，请联系Adobe客户团队（您的客户经理）。
>* 具有的Salesforce帐户 [MSI包设置](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* MARKETO REST API [已成功设置](https://developers.marketo.com/rest-api/){target="_blank"}. 公开的CRUD API将是执行非本机同步的基础。
>* 读取 [此博客帖子](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} 以便了解对象和关系。
>* 设置Salesforce对象以显示18个字符不区分大小写的全局唯一标识符，而不是15个字符区分大小写的全局唯一标识符。

>[!NOTE]
>
>Marketo MSI管理面板中的REST API配置无法用于非本机同步。

## 要成功实现MSI的非本机同步，需要满足以下条件 {#successful-non-native-sync-for-msi-requires-the-following}

1. 将Salesforce Sales用户同步到Marketo。

   Salesforce销售用户是拥有Salesforce中的潜在客户/联系人的外部用户。 需要为Salesforce Sales用户更新Marketo销售人员。 此 *externalSalesPersonId* 字段是销售人员更新插入的必备字段。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo销售人员字段</strong></td> 
      <td><strong>Salesforce销售用户字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce销售用户不区分大小写的全局唯一标识符</td> 
      <td><p>向外部Salesforce Sales User对象标识Marketo销售人员记录。</p><p>要求先同步销售人员，然后再同步其他对象，以便创建适当的关系。</p></td> 
     </tr> 
    </tbody> 
   </table>

   * 销售人员的API文档： [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target="_blank"}
   * 同步销售人员的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Sales_Persones/syncSalesPersonesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persones/syncSalesPersonesUsingPOST){target="_blank"}

1. 将Salesforce帐户同步到Marketo。

   需要为Salesforce帐户更新Marketo公司。 此 _externalCompanyId_ 和 _externalSalesPersonId_ 字段必须用于公司的更新。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo公司字段</strong></td> 
      <td><strong>Salesforce帐户字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Salesforce帐户不区分大小写的全局唯一标识符</td> 
      <td>向外部Salesforce帐户对象标识Marketo公司记录。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce销售用户不区分大小写的全局唯一标识符</td> 
      <td>向作为帐户所有者的外部Salesforce Sales User对象标识Marketo公司记录。<br><br>还用于在Marketo中将本公司与拥有公司记录的销售人员相关联。 要求在设置此字段之前先同步销售人员。</td> 
     </tr> 
    </tbody> 
   </table>

   * 适用于公司的API文档： [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target="_blank"}
   * 同步公司的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target="_blank"}

1. 将Salesforce潜在客户/联系人同步到Marketo。

   您需要为Salesforce潜在客户/联系人更新插入一个Marketo潜在客户。 此 _externalPersonId_， _externalSalesPersonId_、和 _externalCompanyId_ 字段必须用于Lead的更新。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo潜在客户字段</strong></td> 
      <td><strong>Salesforce潜在客户/联系人字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Salesforce潜在客户/联系人不区分大小写的全局唯一标识符</td> 
      <td>将该Marketo Lead记录标识到外部Salesforce Lead/Contact对象。<br><br>这是为MSI非本机引入的新字段。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce销售用户不区分大小写的全局唯一标识符</td> 
      <td>标识拥有此潜在客户/联系人的外部Salesforce Sales User对象。<br><br>还将潜在客户与Marketo中的销售人员关联起来。 要求首先正确同步销售人员。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Salesforce帐户不区分大小写的全局唯一标识符</td> 
      <td>标识潜在客户/联系人所属的外部Salesforce Account对象。<br><br>还将潜在客户记录关联到Marketo中的公司。 要求首先正确同步Salesforce帐户。</td> 
     </tr> 
    </tbody> 
   </table>

   * 潜在客户的API文档： [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/)
   * 用于同步潜在客户的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. 将Salesforce Opportunities同步到Marketo。

   您需要为Salesforce Opportunity更新Marketo Opportunity 。 此 _externalOpportunityId_， _externalCompanyId_、和 _externalSalesPersonId_ 字段必须用于更新Opportunity。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo机会对象字段</strong></td> 
      <td><strong>Salesforce机会对象字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Salesforce潜在客户/联系人不区分大小写的全局唯一标识符</td> 
      <td>向外部Salesforce Opportunity对象标识Marketo Opportunity记录。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Salesforce帐户不区分大小写的全局唯一标识符</td> 
      <td>标识此机会所属的外部Salesforce Account对象。 <br><br>要求首先正确同步Salesforce帐户。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Salesforce销售用户不区分大小写的全局唯一标识符</td> 
      <td>标识拥有此Opportunity的外部Salesforce销售用户对象。 </td> 
     </tr> 
    </tbody> 
   </table>

   * 机会的API文档： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * 有关同步机会的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target="_blank"}

1. 将Salesforce联系人角色同步到Marketo。

   随后，可以通过Marketo Opportunity Role同步Salesforce Opportunity的Salesforce联系人角色。 机会角色记录要求 _externalOpportunityId_， _角色_、和 _leadId_ 字段。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo机会角色字段</strong></td> 
      <td><strong>Salesforce联系人角色字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Salesforce机会不区分大小写的全局唯一标识符</td> 
      <td>向外部Salesforce Opportunity对象标识Marketo Opportunity角色。<br><br>要求首先正确同步Salesforce Opportunity。</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>不适用，这将是Marketo潜在客户ID</td> 
      <td>这将是同步的Salesforce联系人的Marketo潜在客户ID。<br><br>联系人在Marketo中同步后，您可以使用不区分大小写的Salesforce联系人全局唯一标识符作为externalPersonId，并使用Marketo REST API查询Marketo潜在客户。</td> 
     </tr> 
     <tr> 
      <td>角色</td> 
      <td>Salesforce联系人的Role字段</td> 
      <td>描述此机会的联系人的角色。</td> 
     </tr> 
    </tbody> 
   </table>

   * 机会的API文档： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * 有关同步机会的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target="_blank"}

1. 将上一个有趣时刻/MSI评分字段同步到SFDC。

   将Salesforce对象正确同步到Marketo后，您就可以利用MSI功能。 MSI最后一个有趣时刻/评分字段将在潜在客户的REST API中公开。 这些字段由MSI计算并且是只读的。

   Marketo潜在客户的“上一个有趣时刻”/评分字段需要使用REST API潜在客户端点定期同步到Salesforce。 使用以下方式查询Marketo潜在客户的此端点 _externalPersonId_ 作为filterType，并将Salesforce潜在客户GUID作为filterValue传递。

   | GET/rest/v1/leads.json？filterType=externalPersonId&amp;filterValues=salesforceLeadId1，salesforceLeadId2 |
   |---|

   然后，您可以使用这些字段的值同步到Salesforce潜在客户/联系人对象。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo潜在客户字段</strong></td> 
      <td><strong>Salesforce潜在客户/联系人字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentType</td> 
      <td>标签：上一个有趣的时刻类型<br>名称：Last_Interested_Moment_Type__c</td> 
      <td>潜在客户最后一个有趣时刻的类型</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentDate</td> 
      <td><p>标签：上一个有趣的时刻日期</p><p>名称：Last_Interested_Moment_Date__c</p></td> 
      <td>潜在客户最后一个有趣时刻的日期</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentDesc</td> 
      <td><p>标签：上一个有趣时刻描述</p><p>名称：Last_Interested_Moment_Desc__c</p></td> 
      <td>商机最后有趣时刻的描述</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentSource</td> 
      <td><p>标签：上一个有趣时刻源</p><p>名称：Last_Interested_Moment_Source__c</p></td> 
      <td>潜在客户最后一个有趣时刻的来源</td> 
     </tr> 
     <tr> 
      <td>优先级</td> 
      <td><p>标签：参与度</p><p>名称： Priority__c</p></td> 
      <td>商机的优先级</td> 
     </tr> 
     <tr> 
      <td>相对紧迫性</td> 
      <td><p>标签：相对紧急值</p><p>名称：Urgency_Value__c</p></td> 
      <td>潜在客户的相对紧迫性</td> 
     </tr> 
     <tr> 
      <td>相对评分</td> 
      <td><p>标签：相对评分值</p><p>名称：Relative_Score_Value__c</p></td> 
      <td>商机的相对评分</td> 
     </tr> 
    </tbody> 
   </table>

   潜在客户REST API的文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target="_blank"}.

   正确使用外部字段是成功进行非本机同步的关键。 如果您未能在某些视图中查看数据，则可能是因为某个字段未正确同步。 例如，如果在查看“帐户”下的MSI构件时，没有显示商机的活动和有趣的时刻，则可能是商机的公司或帐户未正确同步。 在指定外部字段时对此潜在客户执行GET请求将帮助您验证该潜在客户是否正确同步。 此外，Marketo中外部销售人员的电子邮件必须与Salesforce中该用户的电子邮件匹配。 如果电子邮件不匹配，数据可能不会显示在Salesforce的Marketo选项卡中。

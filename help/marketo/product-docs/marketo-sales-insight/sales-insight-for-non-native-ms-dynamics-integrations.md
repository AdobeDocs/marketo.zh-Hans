---
description: Sales Insight for Non-Native MS Dynamics集成 — Marketo文档 — 产品文档
title: Sales Insight for Non-Native MS Dynamics集成
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1413'
ht-degree: 0%

---

# Sales Insight for Non-Native MS Dynamics集成 {#sales-insight-for-non-native-ms-dynamics-integrations}

如果您的Adobe Marketo Engage帐户通过自定义或非本机集成连接到MS Dynamics，请使用本文配置Sales Insight。

>[!PREREQUISITES]
>
>* 在开始设置MSI之前，已为您的Marketo实例启用“MSI非本机”功能。 如果不是，并且您已购买该功能，请联系 [Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. 如果您尚未购买此功能，请联系Adobe客户团队（您的客户经理）。
>* 下载 [用于自定义同步的MSI包](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.
>* 具有MSI设置的MS Dynamics订阅(我们仅支持 [Dynamics在线](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target="_blank"} 此时)。
>* MARKETO REST API [已成功设置](https://developers.marketo.com/rest-api/){target="_blank"}. 公开的CRUD API将是执行非本机同步的基础。
>* 读取 [此博客帖子](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} 以便了解对象和关系。

## 要成功实现MSI的非本机同步，需要满足以下条件 {#successful-non-native-sync-for-msi-requires-the-following}

1. 将MS Dynamics销售用户同步到Marketo。

   MS Dynamics销售用户是拥有MS Dynamics中的潜在客户/联系人的外部用户。 需要为MS Dynamics销售用户更新Marketo销售人员。 externalSalesPersonId字段强制用于更新销售人员。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo销售人员字段</strong></td> 
      <td><strong>MS Dynamics用户字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics用户不区分大小写的全局唯一标识符</td> 
      <td><p>将Marketo销售人员记录标识到外部MS Dynamics用户对象。</p><p>要求先同步销售人员，然后再同步其他对象，以便创建适当的关系。</p></td> 
     </tr> 
    </tbody> 
   </table>

   * 面向销售人员的API文档： [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target="_blank"}
   * 用于同步销售人员的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Sales_Persones/syncSalesPersonesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persones/syncSalesPersonesUsingPOST){target="_blank"}

1. 将MS Dynamics帐户同步到Marketo。

   需要为MS Dynamics帐户更新Marketo公司。 此 _externalCompanyId_ 和 _externalSalesPersonId_ 字段必须用于本公司之更新植入。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo公司字段</strong></td> 
      <td><strong>MS Dynamics帐户字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>MS Dynamics帐户不区分大小写的全局唯一标识符</td> 
      <td>向外部MS Dynamics帐户对象标识Marketo公司记录。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics销售用户不区分大小写的全局唯一标识符</td> 
      <td>向作为帐户所有者的外部MS Dynamics Sales User对象标识Marketo公司记录。<br><br>还用于在Marketo中将本公司与拥有公司记录的销售人员相关联。 要求在设置此字段之前先同步销售人员。</td> 
     </tr> 
    </tbody> 
   </table>

   * 适用于公司的API文档： [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target="_blank"}
   * 同步公司的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target="_blank"}

1. 将MS Dynamics潜在客户/联系人同步到Marketo。

   您需要为MS Dynamics潜在客户/联系人更新插入Marketo潜在客户。 此 _externalPersonId_， _externalSalesPersonId_、和 _externalCompanyId_ 字段必须用于Lead的更新。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo潜在客户字段</strong></td> 
      <td><strong>MS Dynamics潜在客户/联系人字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>MS Dynamics潜在客户/联系人不区分大小写的全局唯一标识符</td> 
      <td>将Marketo Lead记录标识到外部MS Dynamics Lead/Contact对象。<br><br>这是为MSI非本机引入的新字段。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics销售用户不区分大小写的全局唯一标识符</td> 
      <td>标识拥有此Lead/Contact的外部MS Dynamics销售用户对象。<br><br>还将潜在客户与Marketo中的销售人员关联起来。 要求首先正确同步销售人员。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>MS Dynamics帐户不区分大小写的全局唯一标识符</td> 
      <td>标识潜在客户/联系人所属的外部MS Dynamics帐户对象。<br><br>还将潜在客户记录关联到Marketo中的公司。 要求首先正确同步MS Dynamics帐户。</td> 
     </tr> 
    </tbody> 
   </table>

   * 潜在客户的API文档： [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/){target="_blank"}
   * 用于同步潜在客户的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST){target="_blank"}

1. 将MS Dynamics机会同步到Marketo。

   您需要为MS Dynamics Opportunity更新插入Marketo Opportunity。 此 _externalOpportunityId_， _externalCompanyId_、和 _externalSalesPersonId_ 字段必须用于更新投放Opportunity。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo机会对象字段</strong></td> 
      <td><strong>MS Dynamics机会对象字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>MS Dynamics潜在客户/联系人不区分大小写的全局唯一标识符</td> 
      <td>向外部MS Dynamics Opportunity对象标识Marketo Opportunity记录。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>MS Dynamics帐户不区分大小写的全局唯一标识符</td> 
      <td>标识此机会所属的外部MS Dynamics帐户对象。 <br><br>要求首先正确同步MS Dynamics帐户。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics销售用户不区分大小写的全局唯一标识符</td> 
      <td>标识拥有此Opportunity的外部MS Dynamics销售用户对象。 </td> 
     </tr> 
    </tbody> 
   </table>

   * 机会的API文档： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * 用于同步机会的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target="_blank"}

1. 将MS Dynamics联系人角色同步到Marketo。

   随后，可以通过Marketo Opportunity Role同步MS Dynamics Opportunity的MS Dynamics联系人角色。 机会角色记录要求 _externalOpportunityId_， _角色_、和 _leadId_ 字段。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo机会角色字段</strong></td> 
      <td><strong>MS Dynamics联系人角色字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>MS Dynamics机会不区分大小写的全局唯一标识符</td> 
      <td>向外部MS Dynamics机会对象标识Marketo机会角色。<br><br>要求首先正确同步MS Dynamics Opportunity。</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>不适用，这将是Marketo潜在客户ID</td> 
      <td>这将是同步的MS Dynamics联系人的Marketo潜在客户ID。<br><br>联系人在Marketo中同步后，您可以使用不区分大小写的MS Dynamics联系人全局唯一标识符作为externalPersonId，并使用Marketo REST API查询Marketo潜在客户。</td> 
     </tr> 
     <tr> 
      <td>角色</td> 
      <td>MS Dynamics联系人的“角色”字段</td> 
      <td>描述此机会的联系人的角色。</td> 
     </tr> 
    </tbody> 
   </table>

   * 机会的API文档： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target="_blank"}
   * 用于同步机会的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST){target="_blank"}

1. 将最后一个有趣的时刻/MSI评分字段同步到MS Dynamics。

   将MS Dynamics对象正确同步到Marketo后，您就可以利用MSI功能。 MSI最后一个有趣时刻/评分字段将在REST API中向潜在客户公开。 这些字段由MSI计算并且是只读的。

   Marketo潜在客户的“上一个有趣时刻”/“得分”字段将需要使用REST API潜在客户端点定期同步到MS Dynamics。 使用以下方式查询Marketo潜在客户的此端点 _externalPersonId_ 作为filterType，并将MS Dynamics潜在客户GUID作为filterValue传递。

   | GET/rest/v1/leads.json？filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1，MS DynamicsLeadId2 |
   |---|

   然后，您可以使用这些字段的值同步到MS Dynamics潜在客户/联系人对象。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo潜在客户字段</strong></td> 
      <td><strong>MS Dynamics潜在客户/联系人字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentType</td> 
      <td>标签：上一个有趣时刻类型<br>名称：Last_Interested_Moment_Type__c</td> 
      <td>潜在客户上一个有趣时刻的类型</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentDate</td> 
      <td><p>标签：上一个有趣时刻日期</p><p>名称：Last_Interested_Moment_Date__c</p></td> 
      <td>潜在客户最后一个有趣时刻的日期</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentDesc</td> 
      <td><p>标签：上一个有趣时刻描述</p><p>名称：Last_Interested_Moment_Desc__c</p></td> 
      <td>潜在客户最后一个有趣时刻的描述</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentSource</td> 
      <td><p>标签：上一个有趣时刻源</p><p>名称：Last_Interested_Moment_Source__c</p></td> 
      <td>潜在客户最后一个有趣时刻的来源</td> 
     </tr> 
     <tr> 
      <td>优先级</td> 
      <td><p>标签：参与度</p><p>名称：优先级__c</p></td> 
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

   * 潜在客户REST API的文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#！/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target="_blank"}.

   正确使用外部字段是成功进行非本机同步的关键。 如果未能在某些视图中查看数据，则可能是某个字段未正确同步。 例如，如果在查看“帐户”下的MSI构件时，没有显示商机的活动和有趣的时刻，则可能是商机的公司或帐户未正确同步。 在指定外部字段时对此潜在客户执行GET请求将帮助您验证该潜在客户是否正确同步。 此外，Marketo中外部销售人员的电子邮件必须与MS Dynamics中该用户的电子邮件匹配。 如果电子邮件不匹配，数据可能不会显示在MS Dynamics的Marketo选项卡中。

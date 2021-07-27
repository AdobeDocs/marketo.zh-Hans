---
unique-page-id: 45417125
description: 用于非本机Salesforce集成的销售分析 — Marketo文档 — 产品文档
title: 针对非本机Salesforce集成的销售分析
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
source-git-commit: 73c5375c6e2ec3b2dce09595be1f61f302ff4c25
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 0%

---

# 针对非本机Salesforce集成的销售分析 {#sales-insight-for-non-native-salesforce-integrations}

如果您的Marketo帐户通过自定义或非本机集成连接到Salesforce，请使用本文档配置Sales Insight。

>[!PREREQUISITES]
>
>* 在开始设置MSI之前，为Marketo实例启用了“MSI非本机”功能(如果MSI未启用，并且您已购买该功能，请联系[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support) — 如果您尚未购买此功能，请联系您的客户成功经理)。
>* 设置了[MSI包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)的Salesforce帐户。
>* Marketo REST API [已成功设置](https://developers.marketo.com/rest-api/)。 公开的CRUD API将是执行非本机同步的基础。
>* 请阅读[此博客文章](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/)以了解对象和关系。
>* 设置Salesforce对象以显示18个字符的全局唯一标识符（不区分大小写），而不是15个字符的全局唯一标识符。


>[!NOTE]
>
>Marketo MSI管理面板中的REST API配置不能用于非本机同步。

## MSI的非本机同步成功需要满足以下条件 {#successful-non-native-sync-for-msi-requires-the-following}

1. 将Salesforce Sales用户同步到Marketo。

   Salesforce Sales User是在Salesforce中拥有Lead/Contacts的外部用户。 需要为Salesforce销售用户更新Marketo销售人员。 *externalSalesPersonId*&#x200B;字段强制用于Sales Person的插入。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo销售人员字段</strong></td> 
   <td><strong>Salesforce Sales用户字段</strong></td> 
   <td><strong>描述</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales用户不区分大小写的全局唯一标识符</td> 
   <td><p>将Marketo销售人员记录标识为外部Salesforce销售用户对象。</p><p>它要求销售人员在同步其他对象之前先同步，以便创建正确的关系。</p></td> 
  </tr> 
 </tbody> 
</table>

面向销售人员的API文档：[https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/)\
用于同步销售人员的API文档：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST)

1. 将Salesforce帐户同步到Marketo。

   需要更新Marketo公司的Salesforce帐户。 _externalCompanyId_&#x200B;和&#x200B;_externalSalesPersonId_&#x200B;字段是公司升级的强制字段。

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
   <td>将Marketo公司记录标识为外部Salesforce帐户对象。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales用户不区分大小写的全局唯一标识符</td> 
   <td>将Marketo公司记录标识为外部Salesforce Sales User对象（其为帐户所有者）。<br><br>亦用于将本公司与拥有本公司记录之销售人士联系。在设置此字段之前，必须先同步销售人员。</td> 
  </tr> 
 </tbody> 
</table>

适用于公司的API文档：[https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. 将Salesforce潜在客户/联系人同步到Marketo。

   您需要为Salesforce潜在客户/联系人添加Marketo潜在客户。 _externalPersonId_、_externalSalesPersonId_&#x200B;和&#x200B;_externalCompanyId_&#x200B;字段的强制要求用于Lead的更新。

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
   <td>将Marketo潜在客户记录标识为外部Salesforce潜在客户/联系人对象。<br><br>这是为MSI非本机引入的新字段。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales用户不区分大小写的全局唯一标识符</td> 
   <td>标识拥有此潜在客户/联系人的外部Salesforce销售用户对象。<br><br>此外，还将销售线索与Marketo的销售人员相关联。要求销售人员先正确同步。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce帐户不区分大小写的全局唯一标识符</td> 
   <td>标识潜在客户/联系人所属的外部Salesforce帐户对象。<br><br>此外，还将销售线索记录与Marketo的一家公司关联。强制要求先正确同步Salesforce帐户。</td> 
  </tr> 
 </tbody> 
</table>

潜在客户的API文档：[`https://developers.marketo.com/rest-api/lead-database/leads/`](https://developers.marketo.com/rest-api/lead-database/leads/)\
有关同步潜在客户的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. 将Salesforce机会同步到Marketo。

   您需要为Salesforce Opportunity插入Marketo Opportunity。 _externalOpportunityId_、_externalCompanyId_&#x200B;和&#x200B;_externalSalesPersonId_&#x200B;字段的强制要求用于Opportunity的更新。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Opportunity对象字段</strong></td> 
   <td><strong>Salesforce机会对象字段</strong></td> 
   <td><strong>描述</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforce潜在客户/联系人不区分大小写的全局唯一标识符</td> 
   <td>将Marketo Opportunity记录标识为外部Salesforce Opportunity对象。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce帐户不区分大小写的全局唯一标识符</td> 
   <td>标识此Opportunity所属的外部Salesforce帐户对象。 <br><br>强制要求先正确同步Salesforce帐户。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales用户不区分大小写的全局唯一标识符</td> 
   <td>标识拥有此Opportunity的外部Salesforce Sales User对象。 </td> 
  </tr> 
 </tbody> 
</table>

Opportunity的API文档：[`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. 将Salesforce联系角色同步到Marketo。

   然后，可以通过Marketo Opportunity Role同步Salesforce Opportunity的Salesforce联系角色。 “机会角色”记录授权&#x200B;_externalOpportunityId_、_角色_&#x200B;和&#x200B;_leadId_&#x200B;字段。

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
   <td>Salesforce Opportunity不区分大小写的全局唯一标识符</td> 
   <td>将Marketo Opportunity角色标识为外部Salesforce Opportunity对象。<br><br>要求先正确同步Salesforce Opportunity。</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>不适用，这是Marketo潜在客户ID</td> 
   <td>这将是已同步的Salesforce联系人的Marketo潜在客户ID。<br><br>在Marketo中同步联系人后，您可以使用Salesforce联系人不区分大小写的全局唯一标识符作为externalPersonId，并使用Marketo REST API查询Marketo潜在客户。</td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td>Salesforce联系人的“角色”字段</td> 
   <td>描述联系人对此机会的角色。</td> 
  </tr> 
 </tbody> 
</table>

Opportunity的API文档：[`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. 将上一个有趣的时刻/MSI评分字段同步到SFDC。

   将Salesforce对象正确同步到Marketo后，您便可以利用MSI功能。 MSI最后关注的时刻/评分字段将在REST API中公开，用于潜在客户。 这些字段由MSI计算，为只读字段。

   Marketo Lead的“最后一个有趣的时刻/评分”字段将需要使用REST API Lead端点定期同步到Salesforce。 使用&#x200B;_externalPersonId_&#x200B;作为filterType查询Marketo潜在客户的此端点，并将Salesforce潜在客户GUID作为filterValue传递。

   | GET/rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
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
   <td>msiLastInterestMomentType</td> 
   <td>标签：最后一个有趣的时刻类型<br>名称：Last_Interest_Moment_Type__c</td> 
   <td>潜在客户的最后一个有趣时刻的类型</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestMomentDate</td> 
   <td><p>标签：最后有趣的时刻日期</p><p>名称：Last_Interest_Moment_Date__c</p></td> 
   <td>潜在客户最后一个有趣时刻的日期</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestMomentDesc</td> 
   <td><p>标签：最后有趣的瞬间描述</p><p>名称：Last_Interest_Moment_Desc__c</p></td> 
   <td>潜在客户最后一个有趣时刻的描述</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestMomentSource</td> 
   <td><p>标签：最后有趣的时刻来源</p><p>名称：Last_Interest_Moment_Source__c</p></td> 
   <td>潜在客户最后一个有趣时刻的来源</td> 
  </tr> 
  <tr> 
   <td>优先级</td> 
   <td><p>标签：参与度</p><p>名称：优先级__c</p></td> 
   <td>潜在客户的优先级</td> 
  </tr> 
  <tr> 
   <td>relativeUrquency</td> 
   <td><p>标签：相对紧急值</p><p>名称：紧急_值__c</p></td> 
   <td>领导的相对紧迫性</td> 
  </tr> 
  <tr> 
   <td>相对评分</td> 
   <td><p>标签：相对评分值</p><p>名称：Relative_Score_Value__c</p></td> 
   <td>潜在客户的相对评分</td> 
  </tr> 
 </tbody> 
</table>

Lead REST API的文档：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET)。

正确使用外部字段是成功进行非本机同步的关键。 如果您在某些视图中看不到数据，则可能会发现某个特定字段未正确同步。 例如，如果在潜在客户的帐户下查看MSI小组件时未显示潜在客户的活动和有趣的时刻，则潜在客户的公司或帐户可能未正确同步。 在指定外部字段时对此潜在客户执行GET请求，将帮助您验证该潜在客户是否正确同步。 此外，Marketo中外部销售人员的电子邮件必须与Salesforce中该用户的电子邮件匹配。 如果电子邮件不匹配，则数据可能不会显示在Salesforce的Marketo选项卡中。

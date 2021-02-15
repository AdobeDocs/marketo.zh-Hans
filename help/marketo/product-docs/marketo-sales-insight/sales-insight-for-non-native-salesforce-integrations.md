---
unique-page-id: 45417125
description: 针对非本机Salesforce集成的Sales Insight - Marketo Docs — 产品文档
title: 针对非本机Salesforce集成的Sales Insight
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 0%

---


# 针对非本机Salesforce集成的Sales Insight {#sales-insight-for-non-native-salesforce-integrations}

如果您的Marketo帐户通过自定义或非本机集成连接到Salesforce，请使用此文档配置Sales Insight。

>[!PREREQUISITES]
>
>* 联系您的客户成功经理，为您的Marketo实例启用“MSI非本机”功能。
>* 设置了MSI包的Salesforce帐户。
>* Marketo REST API [已成功设置](https://developers.marketo.com/rest-api/)。 公开的CRUD API将是执行非本机同步的基础。
>* 阅读[此博客文章](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/)以了解对象和关系。
>* 设置Salesforce对象以显示18个字符不区分大小写的全局唯一标识符，而不是15个字符区分大小写的全局唯一标识符。

>



>[!NOTE]
>
>Marketo MSI管理面板中的REST API配置不能用于非本机同步。

## MSI的非本机同步成功需要以下{#successful-non-native-sync-for-msi-requires-the-following}

1. 将Salesforce Sales用户同步到Marketo。

   Salesforce Sales User是拥有Salesforce中的Lead/Contacts的外部用户。 需要为Salesforce Sales用户更新Marketo Sales人员。 *externalSalesPersonId*&#x200B;字段用于Sales Person的更新。

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
   <td><strong>说明</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales用户不区分大小写的全局唯一标识符</td> 
   <td><p>标识外部Salesforce Sales用户对象的Marketo Sales Person记录。</p><p>它要求首先同步销售人员，然后再同步其他对象，以创建正确的关系。</p></td> 
  </tr> 
 </tbody> 
</table>

销售人员的API文档：[https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/)\
用于同步销售人员的API文档：[https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST)

1. 将Salesforce帐户同步到Marketo。

   需要为Salesforce帐户更新Marketo公司。 *externalCompanyId*&#x200B;和&#x200B;*externalSalesPersonId*&#x200B;字段是升级公司所必需的。

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
   <td><strong>说明</strong></td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce帐户不区分大小写的全局唯一标识符</td> 
   <td>标识外部Salesforce帐户对象的Marketo公司记录。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales用户不区分大小写的全局唯一标识符</td> 
   <td>标识作为帐户所有者的外部Salesforce Sales用户对象的Marketo公司记录。<br><br>也用于Market中，以将公司与拥有公司记录的销售人员关联。在设置此字段之前，必须先同步销售人员。</td> 
  </tr> 
 </tbody> 
</table>

公司的API文档：[https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. 将Salesforce潜在客户/联系人同步到Marketo。

   您需要为Salesforce潜在客户/联系人添加Marketo潜在客户。 *externalPersonId*、*externalSalesPersonId*&#x200B;和&#x200B;*externalCompanyId*&#x200B;字段是用于提升潜在客户的。

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
   <td><strong>说明</strong></td> 
  </tr> 
  <tr> 
   <td>externalPersonId</td> 
   <td>Salesforce潜在客户/联系人不区分大小写的全局唯一标识符</td> 
   <td>标识指向外部Salesforce潜在客户/联系人对象的Marketo潜在客户记录。<br><br>这是为MSI非本机版引入的新字段。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales用户不区分大小写的全局唯一标识符</td> 
   <td>标识拥有此潜在客户/联系人的外部Salesforce Sales用户对象。<br><br>还将销售线索与Marketo的销售人员关联。要求让销售人员正确地先同步。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce帐户不区分大小写的全局唯一标识符</td> 
   <td>标识潜在客户/联系人所属的外部Salesforce帐户对象。<br><br>还将销售线索记录与Marketo中的公司相关。要求先正确同步Salesforce帐户。</td> 
  </tr> 
 </tbody> 
</table>

潜在客户的API文档：[`https://developers.marketo.com/rest-api/lead-database/leads/`](https://developers.marketo.com/rest-api/lead-database/leads/)\
同步Lead的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. 将Salesforce机会同步到Marketo。

   您需要为Salesforce Opportunity添加Marketo Opportunity。 *externalOpportunityId*、*externalCompanyId*&#x200B;和&#x200B;*externalSalesPersonId*&#x200B;字段是用于Opportunity的更新的。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Opportunity对象字段</strong></td> 
   <td><strong>Salesforce业务机会对象字段</strong></td> 
   <td><strong>说明</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforce潜在客户/联系人不区分大小写的全局唯一标识符</td> 
   <td>标识外部Salesforce Opportunity对象的Marketo Opportunity记录。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce帐户不区分大小写的全局唯一标识符</td> 
   <td>标识此Opportunity所属的外部Salesforce帐户对象。 <br><br>要求先正确同步Salesforce帐户。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales用户不区分大小写的全局唯一标识符</td> 
   <td>标识拥有此Opportunity的外部Salesforce Sales用户对象。 </td> 
  </tr> 
 </tbody> 
</table>

Opportunity的API文档：[`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. 将Salesforce联系人角色同步到Marketo。

   然后，可以通过Marketo Opportunity角色同步Salesforce Opportunity的Salesforce联系角色。 “业务机会角色”记录要求&#x200B;*externalOpportunityId*、*role*&#x200B;和&#x200B;*leadId*&#x200B;字段。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Opportunity角色字段</strong></td> 
   <td><strong>Salesforce联系人角色字段</strong></td> 
   <td><strong>说明</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforce Opportunity不区分大小写的全局唯一标识符</td> 
   <td>标识外部Salesforce Opportunity对象的Marketo Opportunity角色。<br><br>要求首先正确同步Salesforce Opportunity。</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>否，这将是Marketo潜在客户ID</td> 
   <td>这将是已同步的Salesforce联系人的Marketo潜在客户ID。<br><br>在Marketo中同步联系人后，您可以使用Salesforce Contact全局不区分大小写的唯一标识符作为Marketo Lead的externalPersonId和查询，使用Marketo REST API。</td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td>Salesforce联系人的角色字段</td> 
   <td>描述此机会的联系人的角色。</td> 
  </tr> 
 </tbody> 
</table>

Opportunity的API文档：[`https://developers.marketo.com/rest-api/lead-database/opportunities/`](https://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. 将“上次感兴趣的时刻/MSI评分”字段同步到SFDC。

   Salesforce对象正确同步到Marketo后，您便可以利用MSI功能。 MSI上一个有趣的时刻/评分字段将显示在潜在客户的REST API中。 这些字段由MSI计算，为只读。

   营销人员潜在客户的“最后有趣的时刻/评分”字段需要使用REST API潜在客户端点定期同步到Salesforce。 使用&#x200B;*externalPersonId*&#x200B;作为filterType查询Marketo Lead的此端点，并将Salesforce Lead GUID作为filterValue传入。

   | GET/rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   然后，您可以使用这些字段的值同步到您的Salesforce潜在客户/联系人对象。

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
   <td><strong>说明</strong></td> 
  </tr> 
  <tr> 
   <td>msiLastInteredMomentType</td> 
   <td>标签：上一个有趣的瞬间类型<br>名称：Last_Interest_Moment_Type__c</td> 
   <td>潜在客户的最后一个有趣时刻的类型</td> 
  </tr> 
  <tr> 
   <td>msiLastInteredMomentDate</td> 
   <td><p>标签：最后有趣的时刻</p><p>名称：Last_Interest_Moment_Date__c</p></td> 
   <td>潜在客户最后一个有趣时刻的日期</td> 
  </tr> 
  <tr> 
   <td>msiLastInteredMomentDesc</td> 
   <td><p>标签：最后有趣的时刻描述</p><p>名称：Last_Interest_Moment_Desc__c</p></td> 
   <td>潜在客户最后一个有趣时刻的描述</td> 
  </tr> 
  <tr> 
   <td>msiLastInteredMomentSource</td> 
   <td><p>标签：最后有趣的时刻</p><p>名称：Last_Interest_Moment_Source__c</p></td> 
   <td>潜在客户最后有趣时刻的来源</td> 
  </tr> 
  <tr> 
   <td>优先级</td> 
   <td><p>标签：参与</p><p>名称：优先级__c</p></td> 
   <td>潜在客户的优先级</td> 
  </tr> 
  <tr> 
   <td>relativeUrquency</td> 
   <td><p>标签：相对紧急值</p><p>名称：紧急情况_值__c</p></td> 
   <td>潜在客户的相对紧急性</td> 
  </tr> 
  <tr> 
   <td>相对评分</td> 
   <td><p>标签：相对评分值</p><p>名称：Relative_Score_Value__c</p></td> 
   <td>潜在客户的相对评分</td> 
  </tr> 
 </tbody> 
</table>

潜在客户REST API的文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET)。

正确使用外部字段是成功实现非本机同步的关键。 如果某些视图中未能看到数据，则某个字段可能未正确同步。 例如，如果潜在客户的活动和有趣时刻在其帐户下查看MSI构件时未显示，则潜在客户的公司或帐户可能未正确同步。 在指定外部字段时对此潜在客户执行GET请求将帮助您验证该潜在客户是否正确同步。 此外，Marketo中外部销售人员的电子邮件必须与Salesforce中该用户的电子邮件匹配。 如果电子邮件不匹配，则数据可能无法显示在Salesforce的Marketo选项卡中。


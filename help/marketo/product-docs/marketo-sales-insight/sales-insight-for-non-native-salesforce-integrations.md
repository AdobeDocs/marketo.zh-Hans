---
unique-page-id: 45417125
description: 针对非本机Salesforce集成的销售分析- Marketo Docs —— 产品文档
title: 针对非本机Salesforce集成的销售分析
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 0%

---


# 针对非本机Salesforce集成的销售分析 {#sales-insight-for-non-native-salesforce-integrations}

如果您的Marketo帐户通过自定义或非本机集成连接到Salesforce，请使用此文档配置Sales Insight。

>[!NOTE]
>
>**先决条件**
>
>* 联系您的客户成功经理，为您的Marketo实例启用“MSI非本机”功能。
>* 已设置MSI包的Salesforce帐户。
>* Marketo REST API [设置成功](http://developers.marketo.com/rest-api/)。 公开的CRUD API将是执行非本机同步的基础。
>* 阅 [读此博客](http://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/) ，以了解对象和关系。
>* 设置Salesforce对象以显示18个字符不区分大小写的全局唯一标识符，而不是15个字符区分大小写的全局唯一标识符。

>



>[!NOTE]
>
>Marketo MSI管理面板中的REST API配置不能用于非本机同步。

## MSI的非本机同步成功需要以下 {#successful-non-native-sync-for-msi-requires-the-following}

1. 将Salesforce销售用户同步到Marketo。

   Salesforce Sales User是拥有Salesforce中的Lead/Contacts的外部用户。 需要为Salesforce销售用户更新营销人员销售人员。 外 *部SalesPersonId* 字段是Sales Person的升级必需字段。

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
   <td><strong>说明</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales用户不区分大小写的全局唯一标识符</td> 
   <td><p>标识外部Salesforce销售用户对象的Marketo Sales Person记录。</p><p>它要求首先同步销售人员，然后再同步其他对象，以创建正确的关系。</p></td> 
  </tr> 
 </tbody> 
</table>

销售人员的API文档： [https://developers.marketo.com/rest-api/lead-database/sales-persons/](http://developers.marketo.com/rest-api/lead-database/sales-persons/)\
用于同步销售人员的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST)

1. 将Salesforce帐户同步到Marketo。

   需要为Salesforce帐户更新营销公司。 外 *部CompanyId**和外部SalesPersonId字段* 是用于公司的更新的。

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
   <td>将营销人员公司记录标识为外部Salesforce销售用户对象（其是帐户所有者）。<br><br>也可在Market中用于将公司与拥有公司记录的销售人员关联。 要求先同步销售人员，然后再设置此字段。</td> 
  </tr> 
 </tbody> 
</table>

公司的API文档： [https://developers.marketo.com/rest-api/lead-database/companies/](http://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. 将Salesforce潜在客户／联系人同步到Marketo。

   您需要为Salesforce潜在客户／联系人添加Marketo Lead。 外 *部PersonId*、外 *部SalesPersonId*&#x200B;和外 *部CompanyId* 字段是Lead的升级必需的。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo潜在客户字段</strong></td> 
   <td><strong>Salesforce潜在客户／联系人字段</strong></td> 
   <td><strong>说明</strong></td> 
  </tr> 
  <tr> 
   <td>externalPersonId</td> 
   <td>Salesforce潜在客户／联系人不区分大小写的全局唯一标识符</td> 
   <td>将Marketo Lead记录标识为外部Salesforce Lead/Contact对象。<br><br>这是为MSI非本机版引入的新字段。</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Salesforce Sales用户不区分大小写的全局唯一标识符</td> 
   <td>标识拥有此潜在客户／联系人的外部Salesforce销售用户对象。<br><br>还将销售线索与营销人员关联。 要求首先正确同步销售人员。</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Salesforce帐户不区分大小写的全局唯一标识符</td> 
   <td>标识潜在客户／联系人所属的外部Salesforce帐户对象。<br><br>还将销售线索记录与Marketo中的公司相关。 要求先正确同步Salesforce帐户。</td> 
  </tr> 
 </tbody> 
</table>

潜在客户的API文档： [`https://developers.marketo.com/rest-api/lead-database/leads/`](http://developers.marketo.com/rest-api/lead-database/leads/)\
同步Lead的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. 将Salesforce机会同步到Marketo。

   您需要为Salesforce Opportunity插入Marketo Opportunity。 外 *部OpportunityId*、外 *部CompanyId*&#x200B;和外 *部SalesPersonId* 字段是Opportunity的更新必需的。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo Opportunity对象字段</strong></td> 
   <td><strong>Salesforce Opportunity对象字段</strong></td> 
   <td><strong>说明</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Salesforce潜在客户／联系人不区分大小写的全局唯一标识符</td> 
   <td>将Marketo Opportunity记录标识为外部Salesforce Opportunity对象。</td> 
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

Opportunity的API文档： [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](http://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. 将Salesforce联系人角色同步到Marketo。

   然后，可以通过Marketo Opportunity角色同步Salesforce Opportunity的Salesforce联系人角色。 Opportunity Role记录要求 *外部Opportunity* Id *、角色**和LeadId* 字段。

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
   <td>将Marketo Opportunity角色标识为外部Salesforce Opportunity对象。<br><br>要求首先正确同步Salesforce Opportunity。</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>N/A，这将是Marketo Lead ID</td> 
   <td>这将是已同步的Salesforce联系人的Marketo潜在客户ID。<br><br>在Marketo中同步联系人后，您可以使用Salesforce联系人不区分大小写的全局唯一标识符作为外部PersonId和营销人员潜在客户的查询，使用Marketo REST API。</td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td>Salesforce联系人的角色字段</td> 
   <td>描述此机会的联系人的角色。</td> 
  </tr> 
 </tbody> 
</table>

Opportunity的API文档： [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](http://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. 将上一个有趣的时刻/MSI评分字段同步到SFDC。

   Salesforce对象正确同步到Marketo后，您便可以利用MSI功能。 MSI上一个有趣的时刻／评分字段将在REST API中显示，用于潜在客户。 这些字段由MSI计算，为只读字段。

   营销人员潜在客户的最后一个有趣的时刻／评分字段将需要使用REST API潜在客户端点定期同步到Salesforce。 查询Marketo Lead的此端点，使 *用externalPersonId* 作为filterType，并在Salesforce Lead GUID中传递作为filterValue。

   | GET/rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   然后，您可以使用这些字段的值同步到您的Salesforce潜在客户／联系人对象。

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Marketo潜在客户字段</strong></td> 
   <td><strong>Salesforce潜在客户／联系人字段</strong></td> 
   <td><strong>说明</strong></td> 
  </tr> 
  <tr> 
   <td>msiLastInterestMomentType</td> 
   <td>标签：上一个有趣的<br>时刻TypeName:Last_Interest_Moment_Type_c</td> 
   <td>潜在客户的最后一个有趣时刻的类型</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestMomentDate</td> 
   <td><p>标签：最后一个有趣的时刻日期</p><p>名称：Last_Interest_Moment_Date_c</p></td> 
   <td>潜在客户最后一个有趣时刻的日期</td> 
  </tr> 
  <tr> 
   <td>msiLastInteredMomentDesc</td> 
   <td><p>标签：最后一个有趣的瞬间描述</p><p>名称：Last_Interent_Moment_Desc__c</p></td> 
   <td>潜在客户最后一个有趣时刻的描述</td> 
  </tr> 
  <tr> 
   <td>msiLastInteredMomentSource</td> 
   <td><p>标签：最后有趣的时刻源</p><p>名称：Last_Interest_Moment_Source_c</p></td> 
   <td>潜在客户最后有趣时刻的来源</td> 
  </tr> 
  <tr> 
   <td>优先级</td> 
   <td><p>标签：参与</p><p>名称：优先级__c</p></td> 
   <td>潜在客户的优先级</td> 
  </tr> 
  <tr> 
   <td>relativeRequerty</td> 
   <td><p>标签：相对紧急值</p><p>名称：紧急情况_值_c</p></td> 
   <td>潜在客户的相对紧迫性</td> 
  </tr> 
  <tr> 
   <td>相对评分</td> 
   <td><p>标签：相对评分值</p><p>名称：Relative_Score_Value_c</p></td> 
   <td>潜在客户的相对评分</td> 
  </tr> 
 </tbody> 
</table>

潜在客户REST API的文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET)。

正确使用外部字段是成功实现非本机同步的关键。 如果您在某些视图中看不到数据，则某个字段可能未正确同步。 例如，如果潜在客户的活动和有趣时刻在查看其帐户下的MSI构件时未显示，则潜在客户的公司或帐户可能未正确同步。 指定外部字段时执行此潜在客户的GET请求将帮助您验证该潜在客户是否正确同步。 此外，Market中外部销售人员的电子邮件必须与Salesforce中该用户的电子邮件相匹配。 如果电子邮件不匹配，数据可能不会显示在Salesforce的“营销人员”选项卡中。


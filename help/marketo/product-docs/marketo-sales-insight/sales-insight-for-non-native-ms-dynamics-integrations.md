---
description: 面向非本机MS Dynamics集成的销售分析 — Marketo文档 — 产品文档
title: 非本机MS Dynamics集成的Sales Insight
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
source-git-commit: 3a62fe40856b9b3f2eab61e22eaa38e1b9c44d7e
workflow-type: tm+mt
source-wordcount: '1442'
ht-degree: 0%

---

# 非本机MS Dynamics集成的Sales Insight {#sales-insight-for-non-native-ms-dynamics-integrations}

如果您的Adobe Marketo Engage帐户通过自定义或非本机集成连接到MS Dynamics，请使用本文配置Sales Insight。

>[!PREREQUISITES]
>
>* 在开始设置MSI之前，为Marketo实例启用“MSI非本机”功能(如果未启用，且您已购买该功能，请联系 [Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;} — 如果您尚未购买此功能，请联系您的客户成功经理)。
>* 下载 [用于自定义同步的MSI包](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target=&quot;_blank&quot;}。
>* MSI设置的MS Dynamics订阅(我们仅支持 [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target=&quot;_blank&quot;})。
>* Marketo REST API [成功设置](https://developers.marketo.com/rest-api/){target=&quot;_blank&quot;}。 公开的CRUD API将是执行非本机同步的基础。
>* 读取 [此博客帖子](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target=&quot;_blank&quot;}以了解对象和关系。


## MSI的非本机同步成功需要满足以下条件 {#successful-non-native-sync-for-msi-requires-the-following}

1. 将MS Dynamics Sales用户同步到Marketo。

   MS Dynamics Sales User是MS Dynamics中拥有潜在客户/联系人的外部用户。 需要为MS Dynamics Sales用户更新Marketo销售人员。 外部SalesPersonId字段的权限用于Sales Person的插入。

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
      <td><p>将Marketo销售人员记录标识为外部MS Dynamics用户对象。</p><p>它要求销售人员在同步其他对象之前先同步，以便创建正确的关系。</p></td> 
     </tr> 
    </tbody> 
   </table>

   * 面向销售人员的API文档： [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target=&quot;_blank&quot;}
   * 用于同步销售人员的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Persons/syncSalesPersonsUsingPOST){target=&quot;_blank&quot;}

1. 将MS Dynamics帐户同步到Marketo。

   需要更新Marketo公司的MS Dynamics帐户。 的 _externalCompanyId_ 和 _externalSalesPersonId_ 字段用于更新公司。

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
      <td>将Marketo公司记录标识为外部MS Dynamics帐户对象。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics Sales用户不区分大小写的全局唯一标识符</td> 
      <td>将Marketo公司记录标识为外部MS Dynamics Sales User对象（其为帐户所有者）。<br><br>亦用于将本公司与拥有本公司记录之销售人士联系。 在设置此字段之前，必须先同步销售人员。</td> 
     </tr> 
    </tbody> 
   </table>

   * 适用于公司的API文档： [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target=&quot;_blank&quot;}
   * 用于同步公司的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST){target=&quot;_blank&quot;}

1. 将MS Dynamics Lead/Contacts同步到Marketo。

   您需要为MS Dynamics Lead/Contact插入Marketo Lead。 的 _externalPersonId_, _externalSalesPersonId_&#x200B;和 _externalCompanyId_ 字段用于Lead的插入。

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
      <td>MS Dynamics Lead/Contact全局唯一标识符不区分大小写</td> 
      <td>将Marketo潜在客户记录标识为外部MS Dynamics潜在客户/联系人对象。<br><br>这是为MSI非本机引入的新字段。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics Sales用户不区分大小写的全局唯一标识符</td> 
      <td>标识拥有此潜在客户/联系人的外部MS Dynamics Sales User对象。<br><br>此外，还将销售线索与Marketo的销售人员相关联。 要求销售人员先正确同步。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>MS Dynamics帐户不区分大小写的全局唯一标识符</td> 
      <td>标识潜在客户/联系人所属的外部MS Dynamics帐户对象。<br><br>此外，还将销售线索记录与Marketo的一家公司关联。 强制要求先正确同步MS Dynamics帐户。</td> 
     </tr> 
    </tbody> 
   </table>

   * 潜在客户的API文档： [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/){target=&quot;_blank&quot;}
   * 有关同步潜在客户的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST){target=&quot;_blank&quot;}

1. 将MS Dynamics机会同步到Marketo。

   您需要为MS Dynamics Opportunity插入Marketo Opportunity。 的 _externalOpportunityId_, _externalCompanyId_&#x200B;和 _externalSalesPersonId_ 字段被强制用于Opportunity的更新。

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Marketo Opportunity对象字段</strong></td> 
      <td><strong>MS Dynamics Opportunity对象字段</strong></td> 
      <td><strong>描述</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>MS Dynamics Lead/Contact全局唯一标识符不区分大小写</td> 
      <td>将Marketo Opportunity记录标识为外部MS Dynamics Opportunity对象。</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>MS Dynamics帐户不区分大小写的全局唯一标识符</td> 
      <td>标识此Opportunity所属的外部MS Dynamics帐户对象。 <br><br>强制要求先正确同步MS Dynamics帐户。</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>MS Dynamics Sales用户不区分大小写的全局唯一标识符</td> 
      <td>标识拥有此Opportunity的外部MS Dynamics Sales User对象。 </td> 
     </tr> 
    </tbody> 
   </table>

   * Opportunity的API文档： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;}
   * 用于同步机会的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunitys/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunitys/syncOpportunitiesUsingPOST){target=&quot;_blank&quot;}

1. 将MS Dynamics联系人角色同步到Marketo。

   然后，可以通过Marketo Opportunity Role同步MS Dynamics Opportunity的MS Dynamics Contact Roles。 “机会角色”记录授权 _externalOpportunityId_, _角色_&#x200B;和 _leadId_ 字段。

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
      <td>MS Dynamics Opportunity全局唯一标识符不区分大小写</td> 
      <td>将Marketo Opportunity角色标识为外部MS Dynamics Opportunity对象。<br><br>要求首先正确同步MS Dynamics Opportunity。</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>不适用，这是Marketo潜在客户ID</td> 
      <td>这将是已同步的MS Dynamics联系人的Marketo潜在客户ID。<br><br>在Marketo中同步联系人后，您可以使用MS Dynamics Contact全局不区分大小写的唯一标识符作为externalPersonId，并使用Marketo REST API查询Marketo潜在客户。</td> 
     </tr> 
     <tr> 
      <td>角色</td> 
      <td>MS Dynamics联系人的“角色”字段</td> 
      <td>描述联系人对此机会的角色。</td> 
     </tr> 
    </tbody> 
   </table>

   * Opportunity的API文档： [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;}
   * 用于同步机会的API文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunitys/syncOpportunitiesUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunitys/syncOpportunitiesUsingPOST){target=&quot;_blank&quot;}

1. 将“上次感兴趣的时刻/MSI评分”字段同步到MS Dynamics。

   将MS Dynamics对象正确同步到Marketo后，您便可以利用MSI功能。 MSI最后关注的时刻/评分字段将在REST API中公开，用于潜在客户。 这些字段由MSI计算，为只读字段。

   Marketo Lead的“最后一个有趣的时刻/评分”字段将需要使用REST API Lead端点定期同步到MS Dynamics。 使用查询Marketo Lead的此端点 _externalPersonId_ 作为filterType，并将MS Dynamics潜在客户GUID作为filterValue传递。

   | GET/rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   然后，您可以使用这些字段的值同步到MS Dynamics Lead/Contact对象。

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
      <td>msiLastInterestMomentType</td> 
      <td>标签：最后有趣的时刻类型<br>名称：Last_Interest_Moment_Type__c</td> 
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

   * Lead REST API的文档： [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target=&quot;_blank&quot;}。
   正确使用外部字段是成功进行非本机同步的关键。 如果您在某些视图中看不到数据，则可能会发现某个特定字段未正确同步。 例如，如果在潜在客户的帐户下查看MSI小组件时未显示潜在客户的活动和有趣的时刻，则潜在客户的公司或帐户可能未正确同步。 在指定外部字段时对此潜在客户执行GET请求，将帮助您验证该潜在客户是否正确同步。 此外，Marketo中外部销售人员的电子邮件必须与MS Dynamics中该用户的电子邮件匹配。 如果电子邮件不匹配，则数据可能不会显示在MS Dynamics的Marketo选项卡中。

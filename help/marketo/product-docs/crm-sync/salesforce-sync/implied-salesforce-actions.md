---
unique-page-id: 4719304
description: 默示的Salesforce操作- Marketo文档——产品文档
title: 隐含的Salesforce操作
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# 隐含的Salesforce操作 {#implied-salesforce-actions}

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

运行特定于Salesforce的流步骤时，有时会自动执行额外步骤。 以下是规则，您知道：

当人员当前 *不在Salesforce.com中 [作为联系人](http://Salesforce.com)* 或潜在客户时，这些规则将适用。

<table> 
 <thead> 
  <tr> 
   <th>Marketo Flow步骤</th> 
   <th>自动操作</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>添加到SFDC活动</td> 
   <td>将人员同步到SFDC</td> 
  </tr> 
  <tr> 
   <td>在SFDC活动中更改状态</td> 
   <td>将人员同步<br>到SFDC Dd到SFDC活动</td> 
  </tr> 
  <tr> 
   <td>更改所有者</td> 
   <td><p>将人员同步到SFDC</p></td> 
  </tr> 
  <tr> 
   <td>转换人员</td> 
   <td><p>将人员同步到SFDC</p></td> 
  </tr> 
  <tr> 
   <td>创建任务</td> 
   <td>将人员同步到SFDC</td> 
  </tr> 
 </tbody> 
</table>

您可以使用SFDC类型过滤器在智能列表中过滤 **掉SFDC记录** ，并将运算符设置为“不为空”。 所有SFDC记录在此字段中都有值。

请记住，仅当潜在客户当前不在Salesforce.com中时，才会执 [行这些自动操作](http://Salesforce.com)

Salesforce同步很酷，对吧？

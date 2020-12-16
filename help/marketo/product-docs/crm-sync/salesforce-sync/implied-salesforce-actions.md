---
unique-page-id: 4719304
description: 默示的Salesforce操作- Marketo文档——产品文档
title: 隐含的Salesforce操作
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---


# 隐含的Salesforce操作 {#implied-salesforce-actions}

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

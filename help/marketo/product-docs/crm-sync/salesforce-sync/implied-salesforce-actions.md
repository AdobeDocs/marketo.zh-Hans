---
unique-page-id: 4719304
description: 默示的Salesforce操作 — Marketo文档 — 产品文档
title: 默示的Salesforce操作
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---


# 默示的Salesforce操作{#implied-salesforce-actions}

运行特定于Salesforce的流步骤时，有时会自动执行额外步骤。 以下是规则，您知道：

当此人当前不在[Salesforce.com](https://Salesforce.com)_中时，这些规则将适用_。

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
   <td>将人员同步到SFDC<br>添加到SFDC活动</td> 
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

您可以使用&#x200B;**SFDC类型**&#x200B;过滤器在智能列表中过滤掉SFDC记录，并将运算符设置为“不为空”。 所有SFDC记录在此字段中都有值。

请记住，这些自动操作仅在潜在客户当前不在[Salesforce.com](https://salesforce.com)时发生

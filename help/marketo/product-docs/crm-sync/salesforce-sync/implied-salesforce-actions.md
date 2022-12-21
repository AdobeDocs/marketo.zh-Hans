---
unique-page-id: 4719304
description: 隐含的Salesforce操作 — Marketo文档 — 产品文档
title: 默示的Salesforce操作
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---

# 默示的Salesforce操作 {#implied-salesforce-actions}

当运行特定于Salesforce的流步骤时，有时会自动执行额外的步骤。 以下是规则，因此您知道：

这些规则将适用 _当人员当前不在 [Salesforce.com](https://Salesforce.com)_ 作为联系人或潜在客户。

<table> 
 <thead> 
  <tr> 
   <th>Marketo流量步骤</th> 
   <th>自动操作</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>添加到SFDC营销活动</td> 
   <td>将人员同步到SFDC</td> 
  </tr> 
  <tr> 
   <td>在SFDC促销活动中更改状态</td> 
   <td>将人员同步到SFDC<br>添加到SFDC营销活动</td> 
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

您可以使用 **SFDC类型** 将运算符设置为“不为空”时进行筛选。 所有SFDC记录在此字段中都有值。

请记住，这些自动操作仅在潜在客户当前不在 [Salesforce.com](https://salesforce.com)

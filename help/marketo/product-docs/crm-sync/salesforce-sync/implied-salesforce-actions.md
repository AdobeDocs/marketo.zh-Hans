---
unique-page-id: 4719304
description: 默认为Salesforce操作 — Marketo文档 — 产品文档
title: 隐含的Salesforce操作
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---

# 隐含的Salesforce操作 {#implied-salesforce-actions}

当特定于Salesforce的流程步骤运行时，有时会自动执行额外的步骤。 规则如下，您知道：

这些规则将适用 _当人员当前不在 [Salesforce.com](https://Salesforce.com)_ 作为联系人或潜在客户。

<table> 
 <thead> 
  <tr> 
   <th>Marketo流程步骤</th> 
   <th>自动操作</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>添加到SFDC Campaign</td> 
   <td>将人员同步到SFDC</td> 
  </tr> 
  <tr> 
   <td>在SFDC Campaign中更改状态</td> 
   <td>将人员同步到SFDC<br>添加到SFDC Campaign</td> 
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

您可以使用以下代码过滤掉智能列表中的SFDC记录 **SFDC类型** 运算符设置为“不为空”的筛选条件。 所有SFDC记录在此字段中都有一个值。

请记住，仅当潜在客户当前不在中时，才会发生这些自动操作 [Salesforce.com](https://salesforce.com)

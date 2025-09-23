---
unique-page-id: 4719304
description: 隐含的Salesforce操作 — Marketo文档 — 产品文档
title: 隐含的 Salesforce 操作
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 27%

---

# 隐含的 Salesforce 操作 {#implied-salesforce-actions}

当特定于[!DNL Salesforce]的流程步骤运行时，有时会自动执行额外的步骤。 规则如下，您知道：

当此人当前不是在[Salesforce.com](https://Salesforce.com){target="_blank"}中作为联系人或潜在客户时，将应用这些规则。

<table>
 <thead>
  <tr>
   <th>Marketo流程步骤</th>
   <th>自动操作</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>添加到 SFDC 营销活动</td>
   <td>将人员同步到 SFDC</td>
  </tr>
  <tr>
   <td>更改 SFDC 营销活动中的状态</td>
   <td>将人员同步到SFDC<br>添加至SFDC Campaign</td>
  </tr>
  <tr>
   <td>更改所有者</td>
   <td><p>将人员同步到 SFDC</p></td>
  </tr>
  <tr>
   <td>转换人员</td>
   <td><p>将人员同步到 SFDC</p></td>
  </tr>
  <tr>
   <td>创建任务</td>
   <td>将人员同步到 SFDC</td>
  </tr>
 </tbody>
</table>

您可以使用运算符设置为“**[!UICONTROL SFDC Type]**”的[!UICONTROL is not empty]过滤器过滤掉智能列表中的SFDC记录。 所有SFDC记录在此字段中都有一个值。

请记住，仅当潜在客户当前不在[Salesforce.com](https://salesforce.com){target="_blank"}中时，才会发生这些自动操作

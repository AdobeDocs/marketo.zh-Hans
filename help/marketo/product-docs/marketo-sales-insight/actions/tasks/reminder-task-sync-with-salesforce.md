---
description: 与Salesforce同步提醒任务 — Marketo文档 — 产品文档
title: 与Salesforce同步提醒任务
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# 与Salesforce同步提醒任务 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>要了解如何启用任务同步签出 [将Sales Insight Actions任务/提醒同步到Salesforce任务](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

启用任务同步设置后，用户将看到他们的提醒任务与Salesforce进行双向同步。 这意味着，用户可以通过Salesforce或Sales Insight Actions管理任务，并且确信系统将保持一致性。

## 提醒任务字段同步 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

以下是Sales Insight Actions中的提醒任务字段及其对应的Salesforce字段（通过双向任务同步支持）的列表。

<table>
 <tr>
  <th>销售分析操作任务字段</th>
  <th>Salesforce任务字段</th>
  <th>Salesforce任务</th>
 </tr>
 <tr>
  <td>任务名称</td>
  <td>主题字段</td>
  <td>简短摘要字段，用于显示任务的标题。</td>
 </tr>
 <tr>
  <td>状态</td>
  <td>任务状态</td>
  <td><p>显示任务的状态。 Sales Insight Actions任务具有两种状态，这些状态映射到Salesforce任务状态选取列表中的两个值。</p>
  <p>在Sales Insight Actions中打开=未在Salesforce中启动。</p>
  <p>在Sales Insight Actions中完成=在Salesforce中完成。</p>
  <p>Salesforce中的其他状态值将不会同步到Sales Insight Actions。</p></td>
 </tr>
 <tr>
  <td>优先级</td>
  <td>优先级</td>
  <td><p>“销售分析活动”优先级可以是“正常”或“高”，它们映射到Salesforce中的“正常”和“高”优先级值。</p>
  <p>Salesforce中的低优先级值将不会同步到Sales Insight Actions。</p></td>
 </tr>
 <tr>
  <td>到期日期</td>
  <td>到期日期</td>
  <td>任务的到期日期。</td>
 </tr>
 <tr>
  <td>详细信息</td>
  <td>注释</td>
  <td>显示有关应该使用提醒任务完成的内容的更多详细信息。</td>
 </tr>
</table>

## 首次将Sales Insight Actions任务与Salesforce同步 {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

当您首次打开Sales Insight Actions与Salesforce任务之间的同步时，我们会导入您的Salesforce任务。 我们会 **非** 将您在Sales Insight Actions中拥有的任何当前任务推送到Salesforce。 为了减少杂乱和重复项，从Sales Insight Actions同步到Salesforce中的唯一任务是创建的 *之后* 您可以将Sales Insight Actions与SFDC同步。

以下是同步Sales Insight Actions和SFDC任务时会发生的情况：

* 在同步任务时单击“保存”后，它们就会开始进行同步。 这最初需要一些时间。

* 过去24小时内已更新或创建的任何提醒都将从SFDC拉入到Sales Insight Actions。 同步基于到期日期，所有这些任务将在后端进行同步，但在指挥中心，您只能看到今天和明天到期的任务。

* 如果以前启用了同步，并且您删除了SFDC中的任何任务，则过去15天内删除的任何任务都将从命令中心删除。

* 只要启用同步，我们就会不断在Sales Insight Actions和SFDC之间同步任务。

初次同步后，您在Sales Insight Actions中创建、编辑、完成或删除的任何任务都将同步到Salesforce中的任务列表。 在Salesforce中创建、编辑、完成或删除的任何内容，都将在Sales Insight Actions中更新您的任务列表。

要开启此同步，只需选中您的页面中的 [“设置”页面](https://toutapp.com/login) 在Web应用程序中。

>[!NOTE]
>
>任务的“主题”字段可以在“销售分析操作”中更新，而且该更新将在Salesforce主题字段中针对相应的已同步任务进行同步(如果您使用 `{{activity_subject}}` 中的动态字段 [活动详细信息自定义](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) 设置。 相反，对Salesforce中的subject字段所做的任何更新将 _非_ 同步到“销售分析操作”提醒任务主题字段。

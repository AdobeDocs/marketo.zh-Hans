---
description: 与Salesforce同步提醒任务 — Marketo文档 — 产品文档
title: 与Salesforce同步提醒任务
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 与Salesforce同步提醒任务 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>了解如何启用任务同步签出 [将Sales Connect任务/提醒同步到Salesforce任务](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

启用任务同步设置后，用户将看到他们的提醒任务与Salesforce双向同步。 这意味着用户可以从Salesforce或Sales Connect中管理任务，并且确信系统将保持一致性。

## 提醒任务字段同步 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

以下是Sales Connect中的提醒任务字段及其通过双向任务同步支持的相应Salesforce字段的列表。

<table>
 <tr>
  <th>Sales Connect任务字段</th>
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
  <td><p>显示任务的状态。 Sales Connect任务有两种状态，它们映射到Salesforce任务状态选取列表中的两个值。</p>
  <p>在Sales Connect中打开=未在Salesforce中启动。</p>
  <p>在Sales Connect中完成=在Salesforce中完成。</p>
  <p>Salesforce中的其他状态值将不会同步到Sales Connect。</p></td>
 </tr>
 <tr>
  <td>优先级</td>
  <td>优先级</td>
  <td><p>Sales Connect优先级可以是“正常”或“高”，它们映射到Salesforce中的“正常”和“高”优先级值。</p>
  <p>Salesforce中的低优先级值将不会同步到Sales Connect。</p></td>
 </tr>
 <tr>
  <td>到期日期</td>
  <td>到期日期</td>
  <td>任务的截止日期。</td>
 </tr>
 <tr>
  <td>详细信息</td>
  <td>评论</td>
  <td>显示有关应该使用提醒任务完成的内容的更多详细信息。</td>
 </tr>
</table>

## 首次将Sales Connect任务与Salesforce同步 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

当您首次打开Sales Connect和Salesforce任务之间的同步时，我们会导入您的Salesforce任务。 我们会 **非** 将您在Sales Connect中拥有的任何当前任务推送到Salesforce。 为了减少杂乱和重复项，从Sales Connect同步到Salesforce中的唯一任务是创建任务 *之后* 将Sales Connect与SFDC同步。

以下是同步Sales Connect和SFDC任务时所发生的情况：

* 在同步的任务上单击“保存”后，它们就会开始进行同步。 这最初将需要一些时间。

* 过去24小时内已更新或创建的任何提醒都将从SFDC拉入Sales Connect。 同步基于到期日期，所有这些任务将在后端进行同步，但在命令中心，您只能看到今天和明天到期的任务。

* 如果以前启用了同步，并且您删除了SFDC中的任何任务，则过去15天内删除的任何任务都将从命令中心删除。

* 只要已启用同步，我们就会在Sales Connect和SFDC之间不断同步任务。

初始同步后，您在Sales Connect中创建、编辑、完成或删除的任何任务都将同步到Salesforce中的任务列表中。 在Salesforce中创建、编辑、完成或删除的任何内容都将更新Sales Connect中的任务列表。

要打开此同步，只需选中您的页面中的 [“设置”页面](https://toutapp.com/login) 在Web应用程序中。

>[!NOTE]
>
>任务的subject字段可以在Sales Connect中更新，而且该更新将同步到相应同步任务的Salesforce subject字段中(如果您使用 `{{activity_subject}}` 您的中的动态字段 [活动详细信息自定义](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) 设置。 反过来，对Salesforce中的主题字段所做的任何更新都将 _非_ 同步到Sales Connect提醒任务主题字段。

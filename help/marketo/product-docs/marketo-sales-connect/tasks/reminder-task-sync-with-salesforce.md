---
description: 与Salesforce同步提醒任务 — Marketo文档 — 产品文档
title: 提醒任务与Salesforce同步
hide: true
hidefromtoc: true
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
source-git-commit: 87f43fb58b5739c0465a1a74fb60cdf5c5f6b759
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# 提醒任务与Salesforce同步 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>了解如何启用任务同步签出 [将Sales Connect任务/提醒同步到Salesforce任务](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

启用任务同步设置后，用户将看到其提醒任务与Salesforce双向同步。 这意味着用户可以通过Salesforce或Sales Connect管理任务，并确信系统将保持一致。

## 提醒任务字段同步 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

下面是Sales Connect中的提醒任务字段及其相应的Salesforce字段的列表，这些字段通过双向任务同步受支持。

<table>
 <tr>
  <th>Sales Connect任务字段</th>
  <th>Salesforce任务字段</th>
  <th>Salesforce任务</th>
 </tr>
 <tr>
  <td>任务名称</td>
  <td>主题字段</td>
  <td>用于显示任务标题的简短摘要字段。</td>
 </tr>
 <tr>
  <td>状态</td>
  <td>任务状态</td>
  <td><p>显示任务的状态。 Sales Connect任务具有两种状态，这些状态映射到Salesforce任务状态选取列表中的两个值。</p>
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
  <td>任务到期的日期。</td>
 </tr>
 <tr>
  <td>详细信息</td>
  <td>评论</td>
  <td>显示有关应使用提醒任务完成的内容的更多详细信息。</td>
 </tr>
</table>

## 首次将销售连接任务与Salesforce同步 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

首次打开Sales Connect和Salesforce任务之间的同步时，我们会导入您的Salesforce任务。 我们会 **not** 将您在Sales Connect中拥有的任何当前任务推送到Salesforce。 为了减少混乱和重复项，从Sales Connect到Salesforce中同步的任务只有创建的任务 *after* 将Sales Connect与SFDC同步。

下面是同步Sales Connect和SFDC任务时发生的情况：

* 单击“保存任务”同步后，这些任务即开始同步。 这最初需要一些时间。

* 在过去24小时内更新或创建的任何提醒都将从SFDC提取到Sales Connect。 同步基于到期日期，所有这些任务都将在后端同步，但在命令中心，您将只看到今天和明天到期的任务。

* 如果之前已打开同步，并且您删除了SFDC中的任何任务，则过去15天内删除的任何任务都将从命令中心删除。

* 只要同步处于启用状态，我们就会在Sales Connect和SFDC之间不断同步任务。

初始同步后，您在Sales Connect中创建、编辑、完成或删除的任何任务都将同步到Salesforce中的任务列表。 而在Salesforce中创建、编辑、完成或删除的任何内容都将在Sales Connect中更新您的任务列表。

要打开此同步，只需选中 [“设置”页面](https://toutapp.com/login) 在web应用程序中。
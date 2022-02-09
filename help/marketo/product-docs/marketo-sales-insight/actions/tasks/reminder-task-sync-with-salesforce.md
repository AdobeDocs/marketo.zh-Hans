---
description: 与Salesforce同步提醒任务 — Marketo文档 — 产品文档
title: 提醒任务与Salesforce同步
hide: true
hidefromtoc: true
source-git-commit: acb077e9d6e9fa4027d660ee182a13820f16ad83
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# 提醒任务与Salesforce同步 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>了解如何启用任务同步签出 [将Sales Insight操作任务/提醒同步到Salesforce任务](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

启用任务同步设置后，用户将看到其提醒任务与Salesforce双向同步。 这意味着用户可以从Salesforce或Sales Insight Actions管理任务，并确信系统将保持一致。

## 提醒任务字段同步 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

下面是Sales Insight Actions中的提醒任务字段列表，以及通过双向任务同步支持的相应Salesforce字段。

<table>
 <tr>
  <th>Sales Insight Actions任务字段</th>
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
  <td><p>显示任务的状态。 “销售分析活动”任务具有两种状态，它们映射到Salesforce任务状态选取列表中的两个值。</p>
  <p>在Sales Insight操作中打开=未在Salesforce中启动。</p>
  <p>在Sales Insight操作中完成=在Salesforce中完成。</p>
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
  <td>任务到期的日期。</td>
 </tr>
 <tr>
  <td>详细信息</td>
  <td>评论</td>
  <td>显示有关应使用提醒任务完成的内容的更多详细信息。</td>
 </tr>
</table>

## 首次将销售分析操作任务与Salesforce同步 {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

首次打开Sales Insight Actions和Salesforce任务之间的同步时，我们会导入您的Salesforce任务。 我们会 **not** 将您在Sales Insight Actions中拥有的任何当前任务推送到Salesforce。 为了减少混乱和重复项，从Sales Insight Actions同步到Salesforce中的任务只有创建的任务 *after* 您可以将Sales Insight操作与SFDC同步。

以下是同步Sales Insight操作和SFDC任务时发生的情况：

* 单击“保存任务”同步后，这些任务即开始同步。 这最初需要一些时间。

* 在过去24小时内更新或创建的任何提醒都将从SFDC提取到Sales Insight Actions。 同步基于到期日期，所有这些任务都将在后端同步，但在命令中心，您将只看到今天和明天到期的任务。

* 如果之前已打开同步，并且您删除了SFDC中的任何任务，则过去15天内删除的任何任务都将从命令中心删除。

* 只要启用了同步，我们就会在Sales Insight Actions和SFDC之间不断同步任务。

在初始同步之后，您在Sales Insight Actions中创建、编辑、完成或删除的任何任务都将同步到Salesforce中的任务列表。 而且，在Salesforce中创建、编辑、完成或删除的任何内容都将更新Sales Insight Actions中的任务列表。

要打开此同步，只需选中 [“设置”页面](https://toutapp.com/login) 在web应用程序中。

>[!NOTE]
>
>任务的主题字段可在Sales Insight Actions中更新，如果您使用 `{{activity_subject}}` 动态字段， [活动详细信息自定义](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) 设置。 相反，对Salesforce中的主题字段所做的任何更新都将 _not_ 同步到Sales Insight Actions提醒任务主题字段。

---
unique-page-id: 2953132
description: 了解批量处理和触发智能营销活动 — Marketo文档 — 产品文档
title: 了解批量处理和触发智能营销活动
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 了解批量处理和触发智能营销活动 {#understanding-batch-and-trigger-smart-campaigns}

智能营销活动有两种类型：批次和触发器。

## 批量智能营销活动 {#batch-smart-campaign}

>[!NOTE]
>
>**条件**
>
>批量促销活动在特定时间启动，并且同时影响一组特定人员。 例如，向加利福尼亚的所有人发送电子邮件。

批量智能营销活动将仅在智能列表部分中具有过滤器（即无触发器）。

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

单击 **计划** 选项卡将确认智能营销活动设置为“批处理”。

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**批量智能营销活动**

* 可以安排为重复事件，例如每天、每周和每月。 也可以让它们只运行一次。
* 在 [项目计划视图](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). 智能营销活动中的“等待”步骤之后的任何内容都不会包含在视图中。

<br> 

## 触发智能营销活动 {#trigger-smart-campaign}

>[!NOTE]
>
>**条件**
>
>触发智能营销活动根据触发的事件每次影响一个人。 例如，单击电子邮件中的链接即是触发器。

如果智能营销活动在智能列表部分内至少使用一个触发器，则会自动将模式设置为触发。

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

单击 **计划** 选项卡将确认智能营销活动设置为“已触发”。

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**触发智能营销活动**

* 无法安排重复发生。 它们只能设置为活动或非活动。
* 您可以设置多个触发器。 但是，如果触发了任何触发器，则将运行营销活动操作。

>[!TIP]
>
>使用 [活动日志](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) 用于查看在智能营销活动中逐步发生的情况。 您可以在人员详细信息页面的最后一个选项卡中找到活动日志。

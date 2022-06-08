---
unique-page-id: 2953473
description: SFDC同步 — 活动同步 — Marketo文档 — 产品文档
title: SFDC同步 — 活动同步
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# SFDC同步：活动同步 {#sfdc-sync-activity-sync}

Marketo还会通过Salesforce活动数据进行同步。 以下是一些问题和答案。

## Marketo会同步哪些类型的活动数据？ {#what-types-of-activity-data-does-marketo-sync-over}

Marketo通过与潜在客户或联系人关联的事件和任务进行同步。

## 活动详细信息如何在两个系统之间保持同步？ {#how-are-activity-details-kept-in-sync-between-the-two-systems}

同步是从Salesforce到Marketo的一种方式。 但是，您可以在Salesforce中使用 [创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) 流步骤或 [自定义活动同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) 到Salesforce。

## 我能否使用Marketo创建任务？ {#can-i-create-a-task-using-marketo}

是，您可以使用 [创建任务流操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

## 哪些触发器/过滤器与活动相关？ {#what-are-the-triggers-filters-related-to-activity}

触发器

* 活动已记录
* 活动已更新

过滤器

* 活动已记录/未记录活动已记录
* 活动已更新/未更新活动

>[!TIP]
>
>不确定“不活动”的措辞？ “不”是指非活动过滤器。 请在此处了解有关这些报表包的更多信息： [在智能列表中使用不活动过滤器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

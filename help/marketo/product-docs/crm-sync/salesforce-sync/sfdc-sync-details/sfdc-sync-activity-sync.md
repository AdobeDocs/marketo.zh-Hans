---
unique-page-id: 2953473
description: SFDC同步 — Activity Sync - Marketo文档 — 产品文档
title: SFDC同步 — 活动同步
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# SFDC同步：活动同步 {#sfdc-sync-activity-sync}

Marketo还通过Salesforce活动数据进行同步。 以下是一些问题和答案。

## Marketo同步哪些类型的活动数据？ {#what-types-of-activity-data-does-marketo-sync-over}

Marketo可通过与潜在客户或联系人关联的事件和任务进行同步。

## 活动详细信息如何在这两个系统之间保持同步？ {#how-are-activity-details-kept-in-sync-between-the-two-systems}

从Salesforce到Marketo，同步是单向的。 但是，您可以在Salesforce中使用 [创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) 流程步骤或 [自定义活动同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) Salesforce。

## 我可以使用Marketo创建任务吗？ {#can-i-create-a-task-using-marketo}

可以，您可以使用 [“创建任务流”操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

## 与活动相关的触发器/过滤器有哪些？ {#what-are-the-triggers-filters-related-to-activity}

触发器

* 活动已记录
* 活动已更新

过滤器

* 活动已记录/未记录活动
* 活动已更新/未更新活动

>[!TIP]
>
>不确定“非活动”的措辞吗？ “非”是指非活动筛选器。 可在此处详细了解它们： [在智能列表中使用非活动筛选器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

---
unique-page-id: 2953473
description: SFDC同步 — Activity Sync - Marketo文档 — 产品文档
title: SFDC同步 — 活动同步
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 1%

---

# SFDC同步：活动同步 {#sfdc-sync-activity-sync}

Marketo还通过[!DNL Salesforce]活动数据进行同步。 以下是一些问题和答案。

## Marketo通过哪些类型的活动数据进行同步？ {#what-types-of-activity-data-does-marketo-sync-over}

Marketo会同步与潜在客户或联系人关联的事件和任务。

## 两个系统之间的活动详细信息如何保持同步？ {#how-are-activity-details-kept-in-sync-between-the-two-systems}

同步是单向的，从[!DNL Salesforce]到Marketo。 但您可以使用[!DNL Salesforce]创建任务[流程步骤或](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)自定义活动同步[到](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md)在[!DNL Salesforce]中创建任务。

## 我可以使用Marketo创建任务吗？ {#can-i-create-a-task-using-marketo}

可以，您可以使用[创建任务流操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}。

## 与活动相关的触发器/过滤器有哪些？ {#what-are-the-triggers-filters-related-to-activity}

触发器

* 活动已记录
* 活动已更新

过滤器

* 活动已记录/未记录活动
* 活动已更新/未更新活动

>[!TIP]
>
>不确定“非活动”的措辞吗？ “非”是指非活动筛选器。 在此处了解有关它们的更多信息：[在智能列表中使用非活动筛选器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}

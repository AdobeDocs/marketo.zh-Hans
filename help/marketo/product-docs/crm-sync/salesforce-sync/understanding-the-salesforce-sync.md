---
unique-page-id: 4719283
description: 了解Salesforce同步 — Marketo文档 — 产品文档
title: 了解Salesforce同步
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---

# 了解Salesforce同步 {#understanding-the-salesforce-sync}

Marketo和Salesforce像豌豆和胡萝卜一样走到一起。 我们保持您的销售和营销数据同步。

## 同步的工作原理 {#how-sync-works}

Marketo每天与Salesforce同步。 每次同步都需要一些时间，然后暂停5分钟，然后重新开始。

>[!NOTE]
>
>由于Marketo正在从Salesforce复制整个数据库，因此您的订阅中的首次同步可能需要数小时甚至数天。 之后，每次同步通常需要几秒钟或几分钟，并且只同步已更改的数据。

![](assets/sync-illustration.png)

Salesforce和Marketo之间的同步仅对潜在客户、联系人和Salesforce营销活动进行双向同步。 在这些情况下，只要您在Salesforce或Marketo中进行更改，您的更新就会反映在这两个系统中。 所有其他同步仅从Salesforce到Marketo。 单击下面的链接以了解每个链接的详细信息。

## Marketo和Salesforce之间同步了哪些内容？ {#what-is-synced-between-marketo-and-salesforce}

* [潜在客户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [联系人](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [帐户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [用户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [机会](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforce营销活动](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [自定义对象](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [活动](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>此 [您在Marketo中为Salesforce输入的凭据](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 用于同步数据。 仅包含这些凭据有权访问的数据。

Marketo与Salesforce的合作是世界上同类产品中最强大的。 这感觉像魔术；进行了更改，另一个系统很快便处于最新状态。

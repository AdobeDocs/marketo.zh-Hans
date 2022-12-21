---
unique-page-id: 4719283
description: 了解Salesforce同步 — Marketo文档 — 产品文档
title: 了解Salesforce同步
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---

# 了解Salesforce同步 {#understanding-the-salesforce-sync}

Marketo和Salesforce一起吃豌豆和胡萝卜。 我们将您的销售和营销数据保持同步。

## 同步工作原理 {#how-sync-works}

Marketo每天都会与Salesforce同步。 每次同步都需要一段时间，然后会暂停5分钟，然后再次开始。

>[!NOTE]
>
>您订阅中的首次同步可能需要数小时甚至数天，因为Marketo正在从Salesforce复制整个数据库。 之后，每次同步通常需要数秒或数分钟，并且只同步已更改的数据。

![](assets/sync-illustration.png)

Salesforce和Marketo之间的同步仅适用于潜在客户、联系人和Salesforce促销活动。 在这些情况下，无论您何时在Salesforce或Marketo中进行更改，您的更新都将反映在这两个系统中。 所有其他同步仅从Salesforce到Marketo。 有关每个链接的详细信息，请单击以下链接。

## Marketo与Salesforce之间有何同步？ {#what-is-synced-between-marketo-and-salesforce}

* [潜在客户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [联系人](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [帐户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [用户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [机会](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforce促销活动](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [自定义对象](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [活动](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>的 [您在Marketo for Salesforce中输入的凭据](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 用于通过同步数据。 将只包含这些凭据有权访问的数据。

Marketo与Salesforce的同步是全球同类公司中最强大的。 感觉就像魔法；更改后，另一个系统即将更新。

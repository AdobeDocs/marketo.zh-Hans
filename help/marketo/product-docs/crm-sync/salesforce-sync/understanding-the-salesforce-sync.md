---
unique-page-id: 4719283
description: 了解Salesforce同步 — Marketo文档 — 产品文档
title: 了解Salesforce同步
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# 了解Salesforce同步{#understanding-the-salesforce-sync}

Marketo和Salesforce一起吃豌豆和胡萝卜。 我们可以同步您的销售和营销数据。

## 同步的工作原理{#how-sync-works}

Marketo每天都与Salesforce同步。 每次同步都需要一段时间，然后暂停5分钟，然后再次开始。

>[!NOTE]
>
>您订阅中的首次同步可能需要数小时甚至数天，因为Marketo正在从Salesforce复制整个数据库。 之后，每次同步通常需要几秒钟或几分钟，并且只同步已更改的数据。

![](assets/sync-illustration.png)

Salesforce与Marketo之间的同步仅针对潜在客户、联系人和Salesforce活动双向。 在这些情况下，无论您何时在Salesforce或Marketo中进行更改，您的更新都将反映在两个系统中。 所有其他同步仅从Salesforce到Marketo。 单击以下链接可了解每个链接的详细信息。

## Marketo与Salesforce之间同步了什么？{#what-is-synced-between-marketo-and-salesforce}

* [潜在客户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [联系人](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [帐户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [用户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [机会](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforce活动](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [自定义对象](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [活动](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>您在Marketo中为Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)输入的[凭据用于同步数据。 将仅包含这些凭据有权访问的数据。

Marketo与Salesforce的同步是全球同类产品中最强大的。 感觉就像魔法；更改后，另一个系统即将更新。

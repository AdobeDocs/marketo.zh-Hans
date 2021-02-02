---
unique-page-id: 4719283
description: 了解Salesforce同步- Marketo文档——产品文档
title: 了解Salesforce同步
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# 了解Salesforce同步{#understanding-the-salesforce-sync}

Marketo和Salesforce一起吃豆子和胡萝卜。 我们可同步您的销售和营销数据。

## 同步如何工作{#how-sync-works}

Marketo每天都与Salesforce同步。 每次同步都需要一些时间，然后暂停5分钟，然后再次开始。

>[!NOTE]
>
>您订阅中的第一次同步可能需要数小时甚至数天，因为Marketo正在从Salesforce复制整个数据库。 之后，每次同步通常需要几秒钟或几分钟，并且只同步已更改的数据。

![](assets/sync-illustration.png)

Salesforce和Marketo之间的同步仅针对潜在客户、联系人和Salesforce活动是双向的。 在这些情况下，只要您在Salesforce或Marketo中进行更改，您的更新就会反映在这两个系统中。 所有其他同步仅从Salesforce到Marketo。 单击以下链接可了解每个链接的详细信息。

## Marketo和Salesforce之间同步了什么？{#what-is-synced-between-marketo-and-salesforce}

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

Marketo与Salesforce的同步是世界上同类产品中最强大的。 感觉就像魔法；更改后，另一个系统即将更新。

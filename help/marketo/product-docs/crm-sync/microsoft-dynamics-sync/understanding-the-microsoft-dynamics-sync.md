---
unique-page-id: 10098625
description: 了解Microsoft Dynamics同步 — Marketo文档 — 产品文档
title: 了解Microsoft Dynamics同步
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# 了解Microsoft Dynamics同步 {#understanding-the-microsoft-dynamics-sync}

Marketo和Microsoft动力集团于一身。 我们将您的销售和营销数据保持同步。

>[!NOTE]
>
>Marketo目前仅支持与Java 7兼容的SSL证书。

>[!CAUTION]
>
>我们当前不支持对Marketo Dynamics同步进行沙盒刷新。 如果您需要刷新Dynamics CRM沙盒，则需要新的Marketo沙盒。 有关更多详细信息，请联系Adobe客户团队（您的客户经理）。

## 同步工作原理 {#how-sync-works}

Marketo每天都会将数据与Microsoft Dynamics持续同步。 它是使用后台同步，分批进行，而不是实时进行。

>[!NOTE]
>
>订阅中的首次同步需要几分钟到几小时，具体取决于数据库的大小。 Marketo从Dynamics复制整个数据库。 之后，每次同步通常需要数秒或数分钟，并且只同步已更改的数据。

Marketo与Dynamics之间的同步对于潜在客户和联系人是双向的。 如果您在Marketo或Dynamics中进行更改，则更新将反映在两个系统中。 所有其他字段（如帐户和机会）仅以一种方式同步，从Dynamics到Marketo。

## Marketo与Microsoft Dynamics之间有何同步？ {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [潜在客户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [联系人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [帐户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [用户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* 团队（系统用户组）
* [机会](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [自定义实体](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

的 [您在Marketo for Dynamics中输入的凭据](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) 用于通过同步数据。

>[!NOTE]
>
>如果源实例与Microsoft Dynamics集成，则不支持实例复制。

---
unique-page-id: 10098625
description: 了解Microsoft Dynamics Sync - Marketo Docs —— 产品文档
title: 了解Microsoft Dynamics同步
translation-type: tm+mt
source-git-commit: 20d4c8a079916f47267df3dab5a8e663f6eb019b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 了解Microsoft Dynamics同步{#understanding-the-microsoft-dynamics-sync}

Marketo和Microsoft Dynamics携手合作。 我们可同步您的销售和营销数据。

>[!NOTE]
>
>Marketo目前仅支持与Java 7兼容的SSL证书。

## 同步如何工作{#how-sync-works}

Market能够每天与Microsoft Dynamics连续同步数据。 它是使用后台同步，分批，而不是实时完成的。

>[!NOTE]
>
>订阅中第一次同步需要几分钟到几小时，具体取决于数据库的大小。 Marketo从Dynamics复制整个数据库。 之后，每次同步通常需要几秒钟或几分钟，并且只同步已更改的数据。

Marketo和Dynamics之间的同步对于潜在客户和联系人是双向的。 如果您在Marketo或Dynamics中进行了更改，您的更新将反映在两个系统中。 所有其他字段（如帐户和机会）仅以一种方式同步，从Dynamics到Marketo。

## Marketo与Microsoft Dynamics之间同步了什么？{#what-is-synced-between-marketo-and-microsoft-dynamics}

* [潜在客户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [联系人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [帐户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [用户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* 团队（SystemUsers组）
* [机会](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [自定义实体](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>您在Marketo中为Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)输入的[凭据用于同步数据。

>[!CAUTION]
>
>目前不支持Marketo Dynamics Sync的沙箱刷新。 如果需要刷新Dynamics CRM沙箱，将需要新的Marketo沙箱。 有关更多详细信息，请联系您的客户成功经理。

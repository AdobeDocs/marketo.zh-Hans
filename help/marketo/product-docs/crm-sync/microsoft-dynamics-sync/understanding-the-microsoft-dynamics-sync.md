---
unique-page-id: 10098625
description: 了解 [!DNL Microsoft Dynamics] 同步 — Marketo文档 — 产品文档
title: 了解 Microsoft Dynamics 同步
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 3%

---

# 了解[!DNL Microsoft Dynamics]同步 {#understanding-the-microsoft-dynamics-sync}

Marketo和[!DNL Microsoft Dynamics]一起运行。 我们将保持您的销售和营销数据同步。

>[!CAUTION]
>
>我们当前不支持[!DNL Marketo Dynamics]同步的沙盒刷新。 如果您需要刷新[!DNL Dynamics] CRM沙盒，则需要新的Marketo沙盒。 请联系您的客户成功经理以了解更多详细信息。

## 同步的工作方式 {#how-sync-works}

Marketo每天、全天持续与[!DNL Microsoft Dynamics]同步数据。 它使用后台同步批量完成，而不是实时完成。

>[!NOTE]
>
>您的订阅中第一次同步需要几分钟到几小时，具体取决于数据库的大小。 Marketo从[!DNL Dynamics]复制整个数据库。 之后，每次同步通常需要几秒钟或几分钟，并且只同步已更改的数据。

对于潜在客户和联系人，Marketo与[!DNL Dynamics]之间的同步是双向的。 如果您在Marketo或[!DNL Dynamics]中进行更改，您的更新将反映在这两个系统中。 所有其他字段（如帐户和商机）仅以单向方式同步，从[!DNL Dynamics]到Marketo。

## Marketo和[!DNL Microsoft Dynamics]之间同步了哪些内容？ {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [潜在客户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [联系人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [帐户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [用户](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* 团队（系统用户组）
* [商机](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [自定义实体](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

您在Marketo中为[输入的 [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)凭据用于同步数据。

>[!NOTE]
>
>如果源实例与[!DNL Microsoft Dynamics]集成，则不支持实例复制。

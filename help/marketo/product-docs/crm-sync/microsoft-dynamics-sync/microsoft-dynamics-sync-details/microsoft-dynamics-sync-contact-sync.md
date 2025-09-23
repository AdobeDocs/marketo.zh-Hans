---
unique-page-id: 3571833
description: Microsoft Dynamics同步 — 联系人同步 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步 — 联系人同步
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]同步：联系人同步 {#microsoft-dynamics-sync-contact-sync}

您是否知道Marketo将您的整个数据库与[!DNL Dynamics]同步？ 它同步，然后等待5分钟，然后每天再次同步。 以下是Marketo如何专门处理[!DNL Dynamics]联系人的一些详细信息。

## 两个系统之间的详细信息如何保持同步？ {#how-are-details-kept-in-sync-between-the-two-systems}

联系人同步是双向的。 如果您对[!DNL Dynamics]中的联系人或Marketo中的人员进行了更改，则您的更新将反映在这两个系统中。

## 如果两个系统中的同一字段同时发生更改，该怎么办？ （数据冲突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

尽管这种情况很少见，但Marketo将赢得人员的支持，[!DNL Dynamics]将赢得联系人的支持。 这是因为我们认为营销部门对人具有权威性，而官方的联系人记录系统是在销售(CRM)部门。

## 我可以使用Marketo创建联系人吗？ {#can-i-create-a-contact-using-marketo}

可以。[下面是操作方法](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}。

>[!NOTE]
>
>使用“将人员同步到Microsoft”流程操作（仅在触发器营销活动中）时，将在[!DNL Dynamics]中实时创建潜在客户/联系人。

## 我可以手动强制同步人员或联系人吗？ {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

不会，自动后台同步是在Marketo和[!DNL Dynamics]之间同步更新的唯一方法。 [将人员同步到Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)不会强制同步潜在客户。

## 哪些字段将同步到Marketo？ {#what-fields-will-sync-to-marketo}

您可以[选择要在安装过程中同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)。 但Marketo将仅同步[!DNL Dynamics]同步用户有权访问的字段。

## Marketo是否会遵守[!DNL Dynamics]验证规则？ {#will-marketo-respect-the-dynamics-validation-rules}

是，如果存在冲突，它将在潜在客户活动日志中记录结果。

---
unique-page-id: 3571833
description: Microsoft Dynamics同步 — 联系人同步 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步 — 联系人同步
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
source-git-commit: 7fcbaeda589682fdb5a75b89a0abd8661181566e
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Microsoft Dynamics同步：联系人同步 {#microsoft-dynamics-sync-contact-sync}

您知道Marketo会使用Dynamics同步整个数据库吗？ 它会同步，然后等待5分钟，然后每天再次同步，一整天都在同步。 以下是有关Marketo如何专门处理Dynamics联系人的一些详细信息。

## 这两个系统之间的详细信息如何保持同步？ {#how-are-details-kept-in-sync-between-the-two-systems}

联系人同步是双向的。 如果您在Dynamics中更改了联系人或在Marketo中更改了人员，则您的更新将反映在两个系统中。

## 如果同时对两个系统中的同一字段进行更改，该怎么办？ （数据冲突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

尽管这种情况很少见，但Marketo将赢得人们的青睐，动力将赢得人脉。 这是因为我们认为营销部门对人具有权威性，而官方的联系人记录系统在销售(CRM)部门。

## 我能否使用Marketo创建联系人？ {#can-i-create-a-contact-using-marketo}

是的。 [下面是操作方法](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md).

>[!NOTE]
>
>使用“将人员同步到Microsoft”流程操作（仅在触发器促销活动中）时，将在Dynamics中实时创建潜在客户/联系人。

## 我是否可以手动强制同步人员或联系人？ {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

不能，自动后台同步是在Marketo和Dynamics之间同步更新的唯一方法。 的 [将人员同步到Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) 不会强制同步潜在客户。

## 哪些字段将同步到Marketo? {#what-fields-will-sync-to-marketo}

您可以 [选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) 设置期间。 但Marketo将仅同步Dynamics同步用户有权访问的字段。

## Marketo是否会遵守Dynamics验证规则？ {#will-marketo-respect-the-dynamics-validation-rules}

是的，如果发生冲突，它将在潜在客户活动日志中记录结果。

---
unique-page-id: 3571848
description: Microsoft Dynamics Sync -Lead Sync - Marketo Docs — 产品文档
title: Microsoft Dynamics Sync -Lead Sync
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Microsoft Dynamics同步：潜在客户同步{#microsoft-dynamics-sync-lead-sync}

Marketo到Dynamics的同步功能非常强大。 下面是详细信息：

## 如何在两个系统之间保持详细信息同步？{#how-are-details-kept-in-sync-between-the-two-systems}

同步是双向的。 如果您在Dynamics中对潜在客户或Marketo中的人员进行了更改，您的更新将反映在两个系统中。

>[!NOTE]
>
>删除不总是自动在两个方向同步。 请参阅[删除潜在客户或联系人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md)。

## 如果同时对两个系统中的同一字段进行更改怎么办？ （数据冲突）{#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

尽管这很罕见，但Marketo将赢得人（线索），Dynamics将赢得联系人。 这是因为我们认为营销部门对人具有权威性，而官方的联系人记录系统是在销售(CRM)部门。

## 我是否可以使用Marketo在Dynamics中创建潜在客户？{#can-i-create-a-lead-in-dynamics-using-marketo}

是，使用[将人员同步到Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)流操作。 如果潜在客户不存在，则这将在Dynamics中创建潜在客户。 如果潜在客户确实存在，流步骤将不执行任何操作。

>[!NOTE]
>
>使用“将人员同步到Microsoft”流动操作(仅在触发活动中)时，将在Dynamics中实时创建潜在客户/联系人。

## 我是否可以手动强制将某人从Marketo同步到Dynamics中的潜在客户？{#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

否，自动后台同步是在Marketo和Dynamics之间同步更新的唯一方式。 [将人员同步到Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)流操作不会强制潜在客户进行同步。

## 哪些字段将同步到Marketo?{#what-fields-will-sync-to-marketo}

您可以在设置过程中[选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)。

## Marketo是否会遵守Dynamics验证规则？{#will-marketo-respect-the-dynamics-validation-rules}

是的。 如果数据格式错误或缺少必填字段信息，同步将失败。 如果发生这种情况，Marketo将在人员的活动日志中记录结果。

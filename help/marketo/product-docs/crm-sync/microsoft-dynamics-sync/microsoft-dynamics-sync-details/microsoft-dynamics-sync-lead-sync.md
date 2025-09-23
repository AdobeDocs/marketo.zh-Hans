---
unique-page-id: 3571848
description: Microsoft Dynamics同步 — 潜在客户同步 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步 — 潜在客户同步
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]同步：潜在客户同步 {#microsoft-dynamics-sync-lead-sync}

Marketo到[!DNL Dynamics]的同步处理功能非常强大。 以下是详细信息：

## 两个系统之间的详细信息如何保持同步？ {#how-are-details-kept-in-sync-between-the-two-systems}

同步是双向的。 如果您对[!DNL Dynamics]中的潜在客户或Marketo中的人员进行了更改，则您的更新将反映在这两个系统中。

>[!NOTE]
>
>删除操作并不总是自动双向同步。 请参阅[删除潜在客户或联系人](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}。

## 如果两个系统中的同一字段同时发生更改，该怎么办？ （数据冲突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

尽管这种情况很少见，但Marketo将赢得人员（潜在客户），[!DNL Dynamics]将赢得联系人。 这是因为我们认为营销部门对人具有权威性，而官方的联系人记录系统是在销售(CRM)部门。

## 我可以使用Marketo在[!DNL Dynamics]中创建潜在客户吗？ {#can-i-create-a-lead-in-dynamics-using-marketo}

是，使用[[!UICONTROL Sync Person to Microsoft]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)流程操作。 如果潜在客户不存在，这将在[!DNL Dynamics]中创建潜在客户。 如果潜在客户确实存在，则流程步骤将不会执行任何操作。

>[!NOTE]
>
>使用“[!UICONTROL Sync Person to Microsoft]”流程操作（仅在触发器营销活动中）时，将在[!DNL Dynamics]中实时创建潜在客户/联系人。

## 我能否在[!DNL Dynamics]中手动强制将人员从Marketo同步到潜在客户？ {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

不会，自动后台同步是在Marketo和[!DNL Dynamics]之间同步更新的唯一方法。 [[!UICONTROL Sync Person to Microsoft]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)流程操作不会强制同步潜在客户。

## 哪些字段将同步到Marketo？ {#what-fields-will-sync-to-marketo}

您可以[选择要在安装过程中同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}。

## Marketo是否会遵守[!DNL Dynamics]验证规则？ {#will-marketo-respect-the-dynamics-validation-rules}

可以。如果数据格式错误或缺少必填字段信息，同步将失败。 如果发生这种情况，Marketo将在人员的活动日志中记录结果。

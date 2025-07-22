---
unique-page-id: 3571838
description: Microsoft Dynamics同步 — 字段同步 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步 — 字段同步
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]同步：字段同步 {#microsoft-dynamics-sync-field-sync}

Marketo到[!DNL Dynamics]的同步处理功能非常强大。 详情如下。

## 这两个系统之间的字段详细信息如何保持同步？ {#how-are-field-details-kept-in-sync-between-the-two-systems}

对于潜在客户和联系人实体，同步是双向的。 如果您对[!DNL Dynamics]中的潜在客户或联系人或Marketo中的人员进行了更改，则您的更新将反映在这两个系统中。

对于帐户、用户、商机、团队和自定义实体，同步是单向的：[!DNL Dynamics]到Marketo。 如果您在[!DNL Dynamics]中对这些实体进行了更改，则您的更新将反映在Marketo中。

## 如果两个系统中的同一字段同时发生更改，该怎么办？ （数据冲突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

尽管这种情况很少见，但Marketo将赢得人员（潜在客户），[!DNL Dynamics]将赢得联系人。 这是因为我们认为营销部门对人具有权威性，而官方的联系人记录系统是在销售(CRM)部门。 对于单向同步实体，[!DNL Dynamics]将始终获胜。

## 我可以使用Marketo在[!DNL Dynamics]中创建字段吗？ {#can-i-create-a-field-in-dynamics-using-marketo}

否，当前不支持此操作。

## 我在[!DNL Dynamics]中创建了一个字段。 能否将其同步到Marketo？ {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

可以，只要您的同步用户在[中拥有对字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)的访问权限，您就可以[!DNL Dynamics]同步该字段。

## 哪些字段将同步到Marketo？ {#what-fields-will-sync-to-marketo}

您可以[选择要在安装过程中同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}。

## 如果在同步Marketo和[!DNL Dynamics]后需要添加自定义字段，该怎么办？ {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

您可以随时添加字段，并希望数据从[!DNL Dynamics]刷新到Marketo。 有关详细信息，请参阅[将快速同步与 [!DNL Microsoft Dynamics] 一起使用以获取新的自定义字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)。

## 如果要在将字段添加到同步后删除[!DNL Dynamics]中的字段，该怎么办？ {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo存储对要同步的字段的引用。 如果删除[!DNL Dynamics]中的字段，我们建议在禁用[同步](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)的情况下执行此操作。 然后通过编辑并保存[选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)来刷新Marketo中的架构。

---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs — 产品文档
title: Microsoft Dynamics Sync — 字段同步
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Microsoft Dynamics同步：字段同步{#microsoft-dynamics-sync-field-sync}

Marketo到Dynamics的同步功能非常强大。 下面是详细信息。

## 字段详细信息如何在两个系统之间保持同步？{#how-are-field-details-kept-in-sync-between-the-two-systems}

同步对于潜在客户和联系实体是双向的。 如果您在Dynamics中对潜在客户或联系人或Marketo中的人员进行了更改，您的更新将反映在两个系统中。

对于帐户、用户、机会、团队和自定义实体，同步是单向的：动态到Marketo。 如果您在Dynamics中更改了这些实体，您的更新将反映在Marketo中。

## 如果同时对两个系统中的同一字段进行更改怎么办？ （数据冲突）{#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

尽管这很罕见，但Marketo将赢得人（线索），Dynamics将赢得联系人。 这是因为我们认为营销部门对人具有权威性，而官方的联系人记录系统是在销售(CRM)部门。 对于单向同步实体，Dynamics将始终获胜。

## 我是否可以使用Marketo在Dynamics中创建字段？{#can-i-create-a-field-in-dynamics-using-marketo}

否，当前不支持。

## 我在Dynamics上创建了一个字段。 能否将其同步到Marketo?{#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

是的，只要同步用户在Dynamics中有权访问字段，您就可以[同步字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)。

## 哪些字段将同步到Marketo?{#what-fields-will-sync-to-marketo}

您可以在设置过程中[选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)。

## 如果我需要在Marketo和Dynamics同步后添加自定义字段，该怎么办？{#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

您可以随时添加字段，并期望数据从Dynamics刷新到Marketo。 有关详细信息，请参阅[与Microsoft Dynamics快速同步以获取新自定义字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)。

## 如果我要在将字段添加到同步后删除Dynamics中的字段，该怎么办？{#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo存储对要同步的字段的引用。 如果您在Dynamics中删除字段，我们建议在[sync disabled](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md)的情况下执行此操作。 然后，在Marketo中编辑并保存[选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)，以刷新模式。

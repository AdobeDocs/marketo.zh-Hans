---
unique-page-id: 3571838
description: Microsoft Dynamics同步 — 字段同步 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步 — 字段同步
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Microsoft Dynamics同步：字段同步 {#microsoft-dynamics-sync-field-sync}

Marketo到Dynamics的同步功能非常强大。 细节如下。

## 字段详细信息如何在两个系统之间保持同步？ {#how-are-field-details-kept-in-sync-between-the-two-systems}

对于引线和联系实体，同步是双向的。 如果您在Dynamics中更改了潜在客户或联系人，或在Marketo中更改了人员，则您的更新将反映在两个系统中。

对于帐户、用户、机会、团队和自定义实体，同步是单向的：动态至Marketo。 如果您在Dynamics中更改这些实体，则更新将反映在Marketo中。

## 如果同时对两个系统中的同一字段进行更改，该怎么办？ （数据冲突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

尽管这种情况很少见，但Marketo将为人（领先者）赢得胜利，Dynamics将为联系人赢得胜利。 这是因为我们认为营销部门对人具有权威性，而官方的联系人记录系统在销售(CRM)部门。 对于单向同步实体，Dynamics将始终获胜。

## 我能否使用Marketo在Dynamics中创建字段？ {#can-i-create-a-field-in-dynamics-using-marketo}

否，当前不支持此功能。

## 我在Dynamics中创建了一个字段。 我可以将其同步到Marketo吗？ {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

是的，你可以 [同步字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-4-of-4-connect.md#select-fields-to-sync) 只要同步用户在Dynamics中有权访问该同步。

## 哪些字段将同步到Marketo? {#what-fields-will-sync-to-marketo}

您可以 [选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-4-of-4-connect.md#select-fields-to-sync) 设置期间。

## 如果在同步Marketo和Dynamics后需要添加自定义字段，该怎么办？ {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

您可以随时添加字段，并期待数据从Dynamics刷新到Marketo。 请参阅 [使用与Microsoft Dynamics快速同步来获取新的自定义字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) 以了解详细信息。

## 如果我要在将字段添加到同步后删除Dynamics中的字段，该怎么办？ {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo存储对要同步的字段的引用。 如果删除Dynamics中的字段，我们建议使用 [已禁用](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). 然后，通过编辑和保存 [选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

---
unique-page-id: 3571840
description: Microsoft Dynamics同步 — 用户同步 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步 — 用户同步
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
source-git-commit: 7fcbaeda589682fdb5a75b89a0abd8661181566e
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Microsoft Dynamics同步：用户同步 {#microsoft-dynamics-sync-user-sync}

您知道Marketo会使用Dynamics同步整个数据库吗？ 它会同步，然后等待5分钟，然后每天再次同步，一整天都在同步。 以下是有关Marketo如何专门处理Dynamics帐户的一些详细信息。

为实现集成，您需要专用的Microsoft Dynamics CRM用户。 我们将此用户称为同步用户。

## 用户详细信息如何在两个系统之间保持同步？ {#how-are-user-details-kept-in-sync-between-the-two-systems}

用户同步是一种方式 — 将Dynamics同步到Marketo。 如果您在Dynamics中对用户进行更改，则所做的更改将反映在Marketo中。

## 我能否使用Marketo创建用户？ {#can-i-create-an-user-using-marketo}

不。 Marketo无法在Dynamics中创建用户。

## 哪些字段将同步到Marketo? {#which-fields-will-sync-to-marketo}

您可以 [选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) 设置期间。 但Marketo将仅同步Dynamics同步用户有权访问的字段。

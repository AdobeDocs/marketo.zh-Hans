---
unique-page-id: 3571840
description: Microsoft Dynamics同步 — 用户同步 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步 — 用户同步
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Microsoft Dynamics同步：用户同步 {#microsoft-dynamics-sync-user-sync}

您是否知道Marketo Engage将整个数据库与Dynamics同步？ 它同步，然后等待5分钟，然后每天再次同步。 以下是Marketo如何专门处理Dynamics帐户的一些详细信息。

您需要一个专用的Microsoft Dynamics CRM用户才能进行集成。 我们将此用户称为“同步用户”。

## 这两个系统之间的用户详细信息如何保持同步？ {#how-are-user-details-kept-in-sync-between-the-two-systems}

用户同步是一种方式 — Dynamics到Marketo。 如果您在Dynamics中更改用户，这些更改将反映在Marketo中。

## 我可以使用Marketo创建用户吗？ {#can-i-create-an-user-using-marketo}

不适用。 Marketo无法在Dynamics中创建用户。

## 哪些字段将同步到Marketo？ {#which-fields-will-sync-to-marketo}

您可以[选择要在安装过程中同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}。 但Marketo将仅同步Dynamics同步用户有权访问的字段。

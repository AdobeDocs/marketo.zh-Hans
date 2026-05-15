---
unique-page-id: 3571840
description: 了解用户数据如何从Microsoft Dynamics同步到Marketo。 了解哪些所有者字段同步以及如何在智能列表和流操作中使用它们。
title: Microsoft [!DNL Dynamics] 同步 — 用户同步
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/8H1bMdkhxcvyTuYtHHk00GUy4uycuQ1unsGbZ19AjCM
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 160
ht-degree: 0%

---

# Microsoft [!DNL Dynamics]同步：用户同步 {#microsoft-dynamics-sync-user-sync}

Marketo将整个数据库与[!DNL Dynamics]同步。 它同步，然后等待5分钟，然后每天再次同步。 以下是Marketo如何专门处理[!DNL Dynamics]帐户的一些详细信息。

为了实现集成，您需要一个专用的Microsoft [!DNL Dynamics] CRM用户。 我们将此用户称为“同步用户”。

## 这两个系统之间的用户详细信息如何保持同步？ {#how-are-user-details-kept-in-sync-between-the-two-systems}

用户同步是单向的 — [!DNL Dynamics]到Marketo。 如果您在[!DNL Dynamics]中更改用户，这些更改将反映在Marketo中。

## 我可以使用Marketo创建用户吗？ {#can-i-create-an-user-using-marketo}

不会。 Marketo无法在[!DNL Dynamics]中创建用户。

## 哪些字段将同步到Marketo？ {#which-fields-will-sync-to-marketo}

您可以[选择要在安装过程中同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)。 但Marketo将仅同步[!DNL Dynamics]同步用户有权访问的字段。

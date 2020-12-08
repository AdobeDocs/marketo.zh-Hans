---
unique-page-id: 3571840
description: Microsoft Dynamics Sync —— 用户同步- Marketo Docs —— 产品文档
title: Microsoft Dynamics同步——用户同步
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Microsoft Dynamics同步：用户同步 {#microsoft-dynamics-sync-user-sync}

您知道Market会用Dynamics同步您的整个数据库吗？ 它会同步，然后等待5分钟，然后每天再次同步。 下面是有关Marketo如何具体处理Dynamics帐户的一些详细信息。

为进行集成，您需要一个专用的Microsoft Dynamics CRM用户。 我们将此用户称为同步用户。

## 用户详细信息如何在两个系统之间保持同步？ {#how-are-user-details-kept-in-sync-between-the-two-systems}

用户同步是一种方式- Dynamics到Marketo。 如果您在Dynamics中对用户进行了更改，更改将反映在Marketo中。

## 我是否可以使用Marketo创建用户？ {#can-i-create-an-user-using-marketo}

不。 Marketo无法在Dynamics中创建用户。

## 哪些字段将同步到Marketo? {#which-fields-will-sync-to-marketo}

您可以 [在设置过程中选择要同步](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) 的字段。 但Marketo将仅同步Dynamics同步用户有权访问的字段。

---
unique-page-id: 3571833
description: Microsoft Dynamics Sync -Contact Sync - Marketo Docs —— 产品文档
title: Microsoft Dynamics Sync —— 联系人同步
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---


# Microsoft Dynamics同步：联系同步 {#microsoft-dynamics-sync-contact-sync}

您知道Market会用Dynamics同步您的整个数据库吗？ 它会同步，然后等待5分钟，然后每天再次同步。 下面是Marketo如何具体处理Dynamics Contacts的一些详细信息。

## 如何在两个系统之间保持详细信息同步？ {#how-are-details-kept-in-sync-between-the-two-systems}

联系人同步是双向的。 如果您对Dynamics中的联系人或Marketo中的人员进行了更改，您的更新将反映在两个系统中。

## 如果同时对两个系统中的同一字段进行更改，该怎么办？ （数据冲突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

尽管这很少见，但Marketo将赢得人们的青睐，Dynamics将赢得人脉。 这是因为我们认为营销部门对于人具有权威性，而官方的联系记录系统在销售(CRM)部门。

## 我是否可以使用Marketo创建联系人？ {#can-i-create-a-contact-using-marketo}

是的。 [这是方法](microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md)。

>[!NOTE]
>
>当使用“将人员同步到Microsoft”流动操作(仅在触发活动中)时，将在Dynamics中实时创建潜在客户／联系人。

## 我是否可以手动强制个人或联系人进行同步？ {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

不可以，自动后台同步是在Marketo和Dynamics之间同步更新的唯一方式。 Sync [Person to Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) （将人员同步到Microsoft）不会强制潜在客户进行同步。

## 哪些字段将同步到Marketo? {#what-fields-will-sync-to-marketo}

您可以 [在设置过程中选择要同步](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) 的字段。 但Marketo将仅同步Dynamics同步用户有权访问的字段。

## Marketo是否会遵守Dynamics验证规则？ {#will-marketo-respect-the-dynamics-validation-rules}

是，如果存在冲突，则会在潜在客户活动日志中记录结果。

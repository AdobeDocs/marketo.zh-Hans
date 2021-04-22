---
unique-page-id: 45417322
description: 删除潜在客户或联系人 — Marketo Docs — 产品文档
title: 删除潜在客户或联系人
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# 删除潜在客户或联系人{#deleting-a-lead-or-contact}

在Microsoft Dynamics中删除潜在客户/联系人时，需要了解一些事情。

* Marketo不会仅因Dynamics中删除了潜在客户而自动删除他人。 而是将字段“Microsoft is Deleted”标志设置为true。 如果需要，您可以触发此字段以删除Marketo中的记录。

* “删除人员”流动操作：这仅会删除Marketo中的人员（Dynamics中也不提供删除这些人员的选项）。

* 如果在Marketo中删除了潜在客户（但在Dynamics中未删除），并在之后在Dynamics中更新了该潜在客户，则会在Marketo中创建新人员（相同的电子邮件地址，新人员ID）。

* 如果在Dynamics(但不在Marketo)中删除某个潜在客户，然后随后通过“将人员同步到Microsoft”流动操作运行，它将在Dynamics中创建新的潜在客户。

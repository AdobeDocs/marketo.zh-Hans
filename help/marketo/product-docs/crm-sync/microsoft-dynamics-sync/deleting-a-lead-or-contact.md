---
unique-page-id: 45417322
description: 删除潜在客户或联系人- Marketo Docs —— 产品文档
title: 删除潜在客户或联系人
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# 删除潜在客户或联系人 {#deleting-a-lead-or-contact}

在Microsoft Dynamics中删除潜在客户／联系人时，需要了解一些事情。

-Marketo不会仅因Dynamics中删除了潜在客户而自动删除他人。 而是将字段“Microsoft is Deleted”标志设置为true。 如果需要，您可以触发此字段以删除Marketo中的记录。

-“删除人员”流动操作：这只会删除Marketo中的人员（Dynamics中也不提供删除这些人员的选项）。

-如果Marketo中删除了潜在客户（但Dynamics中未删除），并在Dynamics中更新了该潜在客户，则会在Marketo中创建新人员（相同的电子邮件地址，新人员ID）。

-如果在Dynamics（但不在Marketo中）中删除潜在客户，然后通过“将人员同步到Microsoft”流动操作，它将在Dynamics中创建新的潜在客户。

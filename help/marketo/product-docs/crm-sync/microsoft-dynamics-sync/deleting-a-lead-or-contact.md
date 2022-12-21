---
unique-page-id: 45417322
description: 删除潜在客户或联系人 — Marketo文档 — 产品文档
title: 删除潜在客户或联系人
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# 删除潜在客户或联系人 {#deleting-a-lead-or-contact}

在删除Microsoft Dynamics中的潜在客户/联系人时，需了解一些事项。

* Marketo不会仅因在Dynamics中删除了潜在客户而自动删除人员。 而是将字段“Microsoft已删除”标记设置为true。 如有需要，您可以触发此字段以删除Marketo中的记录。

* “删除人员”流程操作：这仅会删除Marketo中的人员（在Dynamics中也删除人员的选项不可用）。

* 如果在Marketo中删除了某个潜在客户（但未在Dynamics中删除），并在之后的Dynamics中对其进行了更新，则该潜在客户将在Marketo中创建新人员（相同的电子邮件地址、新人员ID）。

* 如果在Dynamics(但不在Marketo中)中删除某个潜在客户，然后通过“将人员同步到Microsoft”流程操作运行，则它将在Dynamics中创建一个新潜在客户。

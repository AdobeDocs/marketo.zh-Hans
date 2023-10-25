---
unique-page-id: 45417322
description: 删除潜在客户或联系人 — Marketo文档 — 产品文档
title: 删除潜在客户或联系人
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 删除潜在客户或联系人 {#deleting-a-lead-or-contact}

关于删除Microsoft Dynamics中的潜在客户/联系人，需要了解几点事项。

* Marketo Engage不会只因为潜在客户已在Dynamics中删除而自动删除人员。 相反，“Microsoft已删除”字段标志设置为true。 如果需要，您可以触发此字段以删除Marketo中的记录。

* “删除人员”流程操作：此操作仅删除Marketo中的人员（在Dynamics中用于同时删除人员的选项不可用）。

* 如果在Marketo中删除潜在客户（但不在Dynamics中），并在删除后在Dynamics中更新潜在客户，则它将在Marketo中创建一个新人员（相同的电子邮件地址和新人员ID）。

* 如果在Dynamics中删除潜在客户(但不在Marketo中)，然后通过“将人员同步到Microsoft”流程操作运行，则它将在Dynamics中创建一个新潜在客户。

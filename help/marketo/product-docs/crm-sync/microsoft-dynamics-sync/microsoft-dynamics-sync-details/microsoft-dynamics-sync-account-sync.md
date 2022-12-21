---
unique-page-id: 3571836
description: Microsoft Dynamics同步 — 帐户同步 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步 — 帐户同步
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Microsoft Dynamics同步：帐户同步 {#microsoft-dynamics-sync-account-sync}

您知道Marketo会使用Dynamics同步整个数据库吗？ 它会同步，然后等待5分钟，然后每天再次同步，一整天都在同步。 以下是有关Marketo如何专门处理Dynamics帐户的一些详细信息。

## 信息同步的方式是什么？ {#which-way-does-the-information-sync}

只有一种方式：从动力学到Marketo。

## 如何进行更新？ {#how-do-the-updates-work}

如果您更新Marketo中某个联系人的“帐户”字段，则会更改Marketo中属于该帐户的所有联系人的值。 它未同步到Dynamics。 但是，下次在Dynamics中更新该帐户时，更改将覆盖Marketo中的所有帐户信息。

## 我能否使用Marketo创建帐户？ {#can-i-create-an-account-using-marketo}

否. Marketo无法在Dynamics中创建帐户。

## 哪些字段将同步到Marketo? {#which-fields-will-sync-to-marketo}

您可以 [选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) 设置期间。 但Marketo将仅同步Dynamics同步用户有权访问的字段。

## Dynamics中“帐户”字段的更改是否会导致每个联系人的“更改数据值”活动日志？  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

大多数情况下，是的。 但是，如果一个帐户的联系人数超过5,000，并且该帐户上的字段在Dynamics中发生更改，则我们会同步更改，但不会记录5,000个以上联系人的活动。

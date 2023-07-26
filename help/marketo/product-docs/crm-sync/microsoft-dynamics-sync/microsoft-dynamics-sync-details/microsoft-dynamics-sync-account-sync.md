---
unique-page-id: 3571836
description: Microsoft Dynamics同步 — 帐户同步 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步 — 帐户同步
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Microsoft Dynamics同步：帐户同步 {#microsoft-dynamics-sync-account-sync}

您是否知道Marketo会将您的整个数据库与Dynamics同步？ 它同步，然后等待5分钟，然后每天再次同步。 以下是Marketo如何专门处理Dynamics帐户的一些详细信息。

## 信息以何种方式同步？ {#which-way-does-the-information-sync}

只有一个方法：从Dynamics到Marketo。

## 这些更新是如何工作的？ {#how-do-the-updates-work}

如果您在Marketo中更新某个联系人的“帐户”字段，则会在Marketo中更改属于该帐户的所有联系人的值。 它不会同步到Dynamics。 但是，下次在Dynamics中更新该帐户时，这些更改将覆盖Marketo中的所有帐户信息。

## 我可以使用Marketo创建帐户吗？ {#can-i-create-an-account-using-marketo}

否. Marketo无法在Dynamics中创建帐户。

## 哪些字段将同步到Marketo？ {#which-fields-will-sync-to-marketo}

您可以 [选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) 设置期间。 但Marketo将仅同步Dynamics同步用户有权访问的字段。

## Dynamics中“帐户”字段的更改是否会导致每个联系人的更改数据值活动日志？  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

大部分，是的。 但是，如果某个帐户拥有超过5,000个联系人，并且该帐户上的某个字段在Dynamics中发生更改，我们会同步该更改，但不会记录5,000多个联系人的活动。

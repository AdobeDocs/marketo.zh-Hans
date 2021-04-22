---
unique-page-id: 3571836
description: Microsoft Dynamics Sync — 帐户同步 — Marketo Docs — 产品文档
title: Microsoft Dynamics Sync — 帐户同步
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Microsoft Dynamics同步：帐户同步{#microsoft-dynamics-sync-account-sync}

您知道Marketo会用Dynamics同步整个数据库吗？ 它会同步，然后等待5分钟，然后每天再次同步。 以下是有关Marketo如何具体对待Dynamics帐户的一些详细信息。

## 信息以哪种方式同步？{#which-way-does-the-information-sync}

只有一种方式：从Dynamics到Marketo。

## 这些更新如何工作？{#how-do-the-updates-work}

如果您更新Marketo中某个联系人的“帐户”字段，它会更改Marketo中属于该帐户的所有联系人的值。 它与Dynamics不同步。 但是，下次在Dynamics中更新该帐户时，更改将覆盖Marketo中的所有帐户信息。

## 是否可以使用Marketo创建帐户？{#can-i-create-an-account-using-marketo}

不。 Marketo无法在Dynamics中创建帐户。

## 哪些字段将同步到Marketo?{#which-fields-will-sync-to-marketo}

您可以在设置过程中[选择要同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)。 但Marketo将仅同步您的Dynamics同步用户有权访问的字段。

## Dynamics中帐户字段的更改是否会导致每个联系人的更改数据值活动日志？ {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

大多数情况下，是的。 但是，如果某个帐户在Dynamics中有5,000个以上的联系人，并且该帐户上的字段发生更改，则我们会同步更改，但不会记录5,000个以上联系人的活动。

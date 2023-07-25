---
unique-page-id: 2953457
description: SFDC同步 — 联系人同步 — Marketo文档 — 产品文档
title: SFDC同步 — 联系人同步
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# SFDC同步：联系同步 {#sfdc-sync-contact-sync}

您知道Marketo将您的整个数据库与Salesforce同步吗？ 它同步，然后等待5分钟，然后每天再次同步。 以下是Marketo如何具体对待Salesforce Contacts的一些详细信息。

## 同步方向 {#sync-direction}

联系人同步是双向的。 如果您在Salesforce或Marketo中对联系人进行了更改，则您的更新将反映在这两个系统中。

## 如果两个系统同时进行更改，该怎么办？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

我们很好，让Salesforce赢。 这种数据冲突很少发生。

## 能否在Marketo中将人员转换为联系人？ {#can-i-convert-a-person-into-a-contact-in-marketo}

是，使用 **[转换人员](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)** flow操作。

>[!CAUTION]
>
>在Marketo中转化人员将在Salesforce中产生新的客户和机会。 如果不希望帐户重复，请使用Salesforce进行转换。

## 我可以手动强制同步联系人吗？ {#can-i-manually-force-a-sync-of-a-contact}

是，使用 **[将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** flow操作，它将实时同步。

## 每个标准字段是否都会同步到Marketo？ {#does-every-single-standard-field-sync-to-marketo}

不，并非所有标准字段都有用。 所有自定义字段都可以成为同步的一部分。

>[!NOTE]
>
>Marketo将仅同步您的Marketo同步用户有权访问的字段。

## Marketo是否会遵守Salesforce验证规则？ {#will-marketo-respect-the-salesforce-validation-rules}

是，如果存在冲突，它会将结果记录在潜在客户活动日志中。

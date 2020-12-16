---
unique-page-id: 2953457
description: SFDC Sync —— 联系人同步- Marketo Docs —— 产品文档
title: SFDC同步——联系同步
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---


# SFDC同步：联系同步 {#sfdc-sync-contact-sync}

您知道Marketo会将您的整个数据库与Salesforce同步吗？ 它会同步，然后等待5分钟，然后每天再次同步。 以下是有关Marketo如何具体处理Salesforce联系人的一些详细信息。

## 同步方向 {#sync-direction}

联系人同步是双向的。 如果您在Salesforce或Marketo中对联系人进行了更改，您的更新将反映在两个系统中。

## 如果同时在两个系统中进行更改怎么办？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

我们很好，让Salesforce赢。 这种数据冲突很少发生。

## 能否在Marketo中将人员转换为联系人？ {#can-i-convert-a-person-into-a-contact-in-marketo}

是，使用**转 [换人员](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**流程操作。

>[!CAUTION]
>
>在Market中将人员转换为Salesforce中将生成新帐户和机会。 如果您不想要重复帐户，请使用Salesforce进行转换。

## 我是否可以手动强制联系人进行同步？ {#can-i-manually-force-a-sync-of-a-contact}

是，使用**将 [人员同步到SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) **流动操作，它将实时同步。

## 每个标准字段是否都与Marketo同步？ {#does-every-single-standard-field-sync-to-marketo}

不，并非所有标准字段都有用。 所有自定义字段都可以作为同步的一部分。

>[!NOTE]
>
>Marketo将仅同步Marketo Sync用户有权访问的字段。

## Market是否会遵守Salesforce验证规则？ {#will-marketo-respect-the-salesforce-validation-rules}

是，如果存在冲突，则会在潜在客户活动日志中记录结果。

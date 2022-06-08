---
unique-page-id: 2953457
description: SFDC同步 — 联系人同步 — Marketo文档 — 产品文档
title: SFDC同步 — 联系人同步
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# SFDC同步：联系人同步 {#sfdc-sync-contact-sync}

您知道Marketo会将整个数据库与Salesforce同步吗？ 它会同步，然后等待5分钟，然后每天再次同步，一整天都在同步。 以下是有关Marketo如何具体处理Salesforce联系人的一些详细信息。

## 同步方向 {#sync-direction}

联系人同步是双向的。 如果您在Salesforce或Marketo中对联系人进行了更改，则您的更新将反映在两个系统中。

## 如果同时在两个系统中进行更改，该怎么办？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

我们很好，让Salesforce赢。 这种数据冲突很少发生。

## 我能将人员转换为Marketo中的联系人吗？ {#can-i-convert-a-person-into-a-contact-in-marketo}

是，使用 **[转换人员](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)** 流量操作。

>[!CAUTION]
>
>在Marketo中转换人员将在Salesforce中生成新帐户和商机。 如果您不希望重复的帐户，请使用Salesforce进行转换。

## 我能否手动强制同步联系人？ {#can-i-manually-force-a-sync-of-a-contact}

是，使用 **[将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** 流操作，它将实时同步。

## 每个标准字段是否都同步到Marketo? {#does-every-single-standard-field-sync-to-marketo}

不，并非所有标准字段都有用。 所有自定义字段都可以包含在同步中。

>[!NOTE]
>
>Marketo将仅同步Marketo同步用户有权访问的字段。

## Marketo是否会遵守Salesforce验证规则？ {#will-marketo-respect-the-salesforce-validation-rules}

是的，如果发生冲突，它将在潜在客户活动日志中记录结果。

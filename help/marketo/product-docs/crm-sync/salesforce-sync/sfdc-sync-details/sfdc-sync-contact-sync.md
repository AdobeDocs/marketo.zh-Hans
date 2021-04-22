---
unique-page-id: 2953457
description: SFDC同步 — 联系同步 — Marketo Docs — 产品文档
title: SFDC同步 — 联系同步
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# SFDC同步：联系同步{#sfdc-sync-contact-sync}

您知道Marketo将您的整个数据库与Salesforce同步吗？ 它会同步，然后等待5分钟，然后每天再次同步。 以下是有关Marketo如何具体对待Salesforce联系人的一些详细信息。

## 同步方向{#sync-direction}

联系人同步是双向的。 如果您在Salesforce或Marketo中对联系人进行了更改，您的更新将反映在两个系统中。

## 如果同时在两个系统中进行更改怎么办？{#what-if-changes-are-made-in-both-systems-at-the-same-time}

我们很好，让Salesforce赢。 这种数据冲突很少发生。

## 能否将某人转换为Marketo中的联系人？{#can-i-convert-a-person-into-a-contact-in-marketo}

是，请使用&#x200B;**[转换人员](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**&#x200B;流操作。

>[!CAUTION]
>
>在Marketo中转换人员将在Salesforce中生成新帐户和机会。 如果您不想要重复帐户，请使用Salesforce进行转换。

## 我是否可以手动强制联系人进行同步？{#can-i-manually-force-a-sync-of-a-contact}

是，使用&#x200B;**[将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)**&#x200B;流操作，它将实时同步。

## 每个标准字段都同步到Marketo吗？{#does-every-single-standard-field-sync-to-marketo}

不，并非所有标准字段都有用。 所有自定义字段都可以是同步的一部分。

>[!NOTE]
>
>Marketo将仅同步Marketo同步用户有权访问的字段。

## Marketo是否会遵守Salesforce验证规则？{#will-marketo-respect-the-salesforce-validation-rules}

是的，如果存在冲突，它将在潜在客户活动日志中记录结果。

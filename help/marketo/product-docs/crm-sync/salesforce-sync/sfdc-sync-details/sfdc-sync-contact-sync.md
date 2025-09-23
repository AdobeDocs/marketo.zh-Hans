---
unique-page-id: 2953457
description: SFDC同步 — 联系人同步 — Marketo文档 — 产品文档
title: SFDC同步 — 联系人同步
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 1%

---

# SFDC 同步：联系人同步 {#sfdc-sync-contact-sync}

您是否知道Marketo将您的整个数据库与[!DNL Salesforce]同步？ 它同步，然后等待5分钟，然后每天再次同步。 以下是Marketo如何专门处理[!DNL Salesforce]联系人的一些详细信息。

## 同步方向 {#sync-direction}

联系人同步是双向的。 如果您在[!DNL Salesforce]或Marketo中对联系人进行了更改，则您的更新将反映在这两个系统中。

## 如果两个系统同时进行更改，该怎么办？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

我们很好，让[!DNL Salesforce]获胜。 这种数据冲突很少发生。

## 能否在Marketo中将人员转换为联系人？ {#can-i-convert-a-person-into-a-contact-in-marketo}

是，使用&#x200B;**[转换人员](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}**&#x200B;流程操作。

>[!CAUTION]
>
>在Marketo中转化人员将在[!DNL Salesforce]中产生新帐户和机会。 如果不希望帐户重复，请使用[!DNL Salesforce]进行转换。

## 我可以手动强制同步联系人吗？ {#can-i-manually-force-a-sync-of-a-contact}

是，使用&#x200B;**[将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}**&#x200B;流程操作，该操作将实时同步。

## 每个标准字段是否都会同步到Marketo？ {#does-every-single-standard-field-sync-to-marketo}

不，并非所有标准字段都有用。 所有自定义字段都可以成为同步的一部分。

>[!NOTE]
>
>Marketo将仅同步您的Marketo同步用户有权访问的字段。

## Marketo是否会遵守[!DNL Salesforce]验证规则？ {#will-marketo-respect-the-salesforce-validation-rules}

是，如果存在冲突，它将在潜在客户活动日志中记录结果。

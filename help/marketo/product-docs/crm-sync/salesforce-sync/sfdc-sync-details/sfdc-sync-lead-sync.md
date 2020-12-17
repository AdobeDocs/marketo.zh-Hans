---
unique-page-id: 2953455
description: SFDC Sync -Lead Sync - Marketo Docs —— 产品文档
title: SFDC同步——潜在客户同步
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---


# SFDC同步：潜在客户同步{#sfdc-sync-lead-sync}

您知道Marketo从您的Salesforce数据库同步吗？ 它同步，等待5分钟，然后再次同步。 整天，每天。 以下是有关Marketo如何具体对待Salesforce潜在客户的一些详细信息。

## 同步方向{#sync-direction}

线索（人）和联系人同步是双向的。 如果您在Salesforce或Marketo中对记录进行了更改，您的更新将反映在两个系统中。

## 如果同时在两个系统中进行更改怎么办？{#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo获胜。 这种数据冲突很少发生。

## 我是否可以使用Marketo在Salesforce中创建潜在客户？{#can-i-create-a-lead-in-salesforce-using-marketo}

是，请使用[将人员同步到SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)流操作。 如果潜在客户不存在，则此操作将在Salesforce中创建潜在客户。

## 我是否可以手动将Market中的人员同步到Salesforce中的潜在客户？{#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

是，使用[将人员同步到SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)流操作，它将实时同步。

## 每个标准字段是否都与Marketo同步？{#does-every-single-standard-field-sync-to-marketo}

不，并非所有标准字段都有用。 所有自定义字段都可以作为同步的一部分。

>[!NOTE]
>
>Marketo将仅同步Salesforce同步用户有权访问的字段。

## Market是否会遵守Salesforce验证规则？{#will-marketo-respect-the-salesforce-validation-rules}

是的。 如果数据格式错误或缺少必填字段信息，同步将失败。 如果发生这种情况，Marketo将在Lead活动日志中记录结果。

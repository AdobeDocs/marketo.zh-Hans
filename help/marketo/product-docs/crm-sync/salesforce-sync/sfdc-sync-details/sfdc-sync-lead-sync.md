---
unique-page-id: 2953455
description: SFDC同步 — 潜在客户同步 — Marketo文档 — 产品文档
title: SFDC同步 — 潜在客户同步
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# SFDC同步：潜在客户同步 {#sfdc-sync-lead-sync}

您是否知道Salesforce数据库中的Marketo同步？ 它会同步，等待5分钟，然后再次同步。 一整天，每天。 以下是Marketo如何特别对待Salesforce潜在客户的一些详细信息。

## 同步方向 {#sync-direction}

商机（人员）和联系人同步是双向的。 如果您在Salesforce或Marketo中对记录进行了更改，则您的更新将反映在这两个系统中。

## 如果两个系统同时进行更改，该怎么办？ {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo胜出。 这种数据冲突很少发生。

## 我可以使用Marketo在Salesforce中创建潜在客户吗？ {#can-i-create-a-lead-in-salesforce-using-marketo}

是，使用 [将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) flow操作。 如果商机不存在，这将在Salesforce中创建商机。

## 我能否手动强制将Marketo中的人员同步到Salesforce中的潜在客户？ {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

是，使用 [将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) flow操作，它将实时同步。

## 每个标准字段是否都会同步到Marketo？ {#does-every-single-standard-field-sync-to-marketo}

不，并非所有标准字段都有用。 所有自定义字段都可以成为同步的一部分。

>[!NOTE]
>
>Marketo将仅同步您的Salesforce同步用户有权访问的字段。

## Marketo是否会遵守Salesforce验证规则？ {#will-marketo-respect-the-salesforce-validation-rules}

是. 如果数据格式错误或缺少必填字段信息，同步将失败。 如果发生这种情况，Marketo将在潜在客户活动日志中记录结果。

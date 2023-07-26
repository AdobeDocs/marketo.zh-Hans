---
unique-page-id: 2951103
description: 发行说明 — 2013年2月 — Marketo文档 — 产品文档
title: 发行说明 — 2013年2月
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 发行说明： 2013年2月 {#release-notes-february}

2月版包括一项强烈要求的功能，支持Apple Safari以及其他一些小的增强功能。

## 对Apple Safari的官方支持 {#official-support-for-apple-safari}

Apple Safari for Mac和Windows的最新版本完全支持与Marketo潜在客户管理结合使用。 注意：iOS上的Safari不完全兼容。

## Webhook增强功能 {#webhooks-enhancements}

增强了Webhook以转义URL/有效负载中的令牌，并且还可以通过解析来自第三方系统的XML/JSON响应（在Spark SMB Edition中不可用）来更新Marketo潜在客户字段。

## 更新了SOAP API端点 {#updated-soap-api-endpoint}

首选的SOAP API端点已更新，如管理员 — > SOAP API中所示。 请更新您的调用以使用此新端点。 对旧端点的API调用已弃用，但将继续正常运行。 （Spark SMB Edition中不提供SOAP API）

## facebook选项卡的移动设备支持 {#mobile-support-for-facebook-tabs}

从Marketo发布的Facebook选项卡将检测移动设备并将它们路由到登陆页面。 这将确保用户在不支持Facebook选项卡的移动设备上获得正确的内容(在Spark、Standard、Select SMB Editions和Marketo Social Marketing中提供)。

## 即将推出：支持多种模型 {#coming-soon-support-for-multiple-models}

我们正在为支持多种收入周期模型奠定基础，在未来的版本中，我们投票支持社区中#1RCA的构想。 在此版本中，您会注意到一些更改，包括 [智能列表筛选器和在流程步骤中添加选项](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md) 支持模型和阶段的选择。 我们还将潜在客户收入阶段和潜在客户收入周期模型字段移出“智能列表潜在客户网格”选项卡。

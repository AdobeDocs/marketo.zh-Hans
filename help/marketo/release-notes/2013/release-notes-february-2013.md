---
unique-page-id: 2951103
description: 发行说明- 2013年2月- Marketo Docs —— 产品文档
title: 发行说明- 2013年2月
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# 发行说明：2013年2月 {#release-notes-february}

2月版本包含一个强烈要求的功能、对Apple Safari的支持以及其他小的增强功能。

## 对Apple Safari的正式支持 {#official-support-for-apple-safari}

完全支持Mac和Windows版Apple Safari的最新版本，以便与Marketo Lead Management一起使用。 注意：iOS上的Safari不完全兼容。

## Webhooks增强功能 {#webhooks-enhancements}

Webhooks经过增强，可以在URL/有效负荷中转义令牌，还可以通过解析第三方系统（Spark SMB Edition中不提供）的XML/JSON响应来更新Marketo潜在客户字段。

## 更新的SOAP API端点 {#updated-soap-api-endpoint}

首选的SOAP API端点已更新，如Admin -> SOAP API中所示。 请更新您的调用以使用此新端点。 已弃用对旧端点的API调用，但将继续运行。 （Spark SMB Edition中不提供SOAP API）

## Facebook选项卡的移动支持 {#mobile-support-for-facebook-tabs}

从Marketo发布的Facebook选项卡将检测移动设备并将它们路由到登陆页。 这将确保用户在不支持Facebook选项卡的移动设备上获得正确的内容（在Spark、Standard、Select SMB Editions和Marketo Social Marketing中提供）。

## 即将推出：支持多种型号 {#coming-soon-support-for-multiple-models}

我们正在为支持多个收入周期模型奠定基础，在未来版本中，在社区中为RCA投了第一票。 在此版本中，您将注意到一些更改， [包括智能列表过滤器和在流步骤中添加选择](../../product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md) ，以支持选择模型和舞台。 我们还将“潜在客户收入阶段”和“潜在客户收入周期模型”字段移出“智能列表潜在客户”网格标签。

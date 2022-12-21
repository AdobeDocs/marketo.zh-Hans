---
unique-page-id: 2951103
description: 发行说明 — 2013年2月 — Marketo文档 — 产品文档
title: 发行说明 — 2013年2月
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 发行说明：2013年2月 {#release-notes-february}

2月版本包括一项强烈请求的功能、对Apple Safari的支持和其他小型增强功能。

## 对Apple Safari的正式支持 {#official-support-for-apple-safari}

完全支持将最新版本的Apple Safari for Mac和Windows与Marketo潜在客户管理结合使用。 注意：iOS上的Safari不兼容。

## Webhooks增强功能 {#webhooks-enhancements}

Webhook已得到增强，可对URL/有效负载中的令牌进行转义，并且还可以通过解析来自第三方系统（Spark SMB Edition中不提供）的XML/JSON响应来更新Marketo潜在客户字段。

## 更新了SOAP API端点 {#updated-soap-api-endpoint}

首选的SOAP API端点已更新，如Admin -> SOAP API中所示。 请更新您的调用以使用此新端点。 已弃用对旧端点的API调用，但将继续正常运行。 （Spark SMB版中不提供SOAP API）

## 移动设备支持Facebook选项卡 {#mobile-support-for-facebook-tabs}

从Marketo发布的facebook选项卡将检测移动设备并将其路由到登陆页面。 这将确保用户在不支持Facebook选项卡的移动设备上获得正确的内容(在Spark、Standard、Select SMB版本和Marketo Social Marketing中提供)。

## 即将推出：支持多个型号 {#coming-soon-support-for-multiple-models}

我们正在为支持多个收入周期模型做准备，在将来的版#1中为社区中的RCA投了票。 在此版本中，您会注意到一些更改，包括 [智能列表过滤器和在流程步骤中添加选项](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md) 支持选择模型和舞台。 我们还要将潜在客户收入阶段和潜在客户收入周期模型字段从智能列表潜在客户网格选项卡中移出。

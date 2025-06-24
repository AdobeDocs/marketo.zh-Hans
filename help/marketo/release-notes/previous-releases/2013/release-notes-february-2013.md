---
unique-page-id: 2951103
description: 发行说明 — 2013年2月 — Marketo文档 — 产品文档
title: 发行说明 — 2013年2月
exl-id: 9adfa676-09ea-497a-bcce-42300848b9d8
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# 发行说明： 2013年2月 {#release-notes-february}

2月版包括强烈要求的功能、对[!DNL Apple Safari]的支持以及其他小增强功能。

## 对[!DNL Apple Safari]的正式支持 {#official-support-for-apple-safari}

Mac和[!DNL Windows]的最新版本[!DNL Apple Safari]完全支持与Marketo潜在客户管理一起使用。 注意：iOS上的[!DNL Safari]不完全兼容。

## Webhook增强功能 {#webhooks-enhancements}

Webhook已得到增强，能够转义URL/有效负载中的令牌，并且还可以通过解析来自第三方系统的XML/JSON响应（在[!DNL Spark SMB Edition]中不可用）来更新Marketo潜在客户字段。

## 更新了SOAP API端点 {#updated-soap-api-endpoint}

首选的SOAP API端点已更新，显示在[!UICONTROL Admin] -> SOAP API中。 请更新您的调用以使用此新端点。 对旧端点的API调用已弃用，但将继续正常运行。 (SOAP API在[!DNL Spark SMB Edition]中不可用)

## 对[!DNL Facebook]选项卡的移动支持 {#mobile-support-for-facebook-tabs}

从Marketo发布的[!DNL Facebook]选项卡将检测移动设备并将它们路由到登陆页面。 这将确保用户在不支持[!DNL Facebook]选项卡的移动设备上获得正确内容（在[!DNL Spark]、[!DNL Standard]、[!DNL Select SMB Editions]和[!DNL Marketo Social Marketing]中可用）。

## 即将推出：支持多种模型 {#coming-soon-support-for-multiple-models}

我们正在为支持多种收入周期模型奠定基础，在未来的版本中，我们投票支持社区中#1RCA的构想。 在此版本中，您会注意到一些更改，包括[智能列表筛选器以及在流程步骤](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/find-all-leads-in-a-revenue-cycle-model.md)中添加选项，以支持模型和阶段的选择。 我们还将潜在客户收入阶段和潜在客户收入周期模型字段移出“智能列表潜在客户网格”选项卡。

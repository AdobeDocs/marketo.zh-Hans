---
unique-page-id: 2953243
description: 通知类型 — Marketo文档 — 产品文档
title: 通知类型
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 1%

---

# 通知类型 {#notification-types}

有多种通知类型。

## 营销活动失败  {#campaign-failure}

营销活动失败会通知您智能营销活动中的错误。

## CRM同步 {#crm-sync}

CRM同步通知会提醒您发现CRM同步存在的严重问题，例如权限不正确或同步已关闭。

**[!DNL Microsoft Dynamics]**

[!DNL Dynamics]通知每24小时发送一次，并包含在此时间段内同步失败的潜在客户。 失败的典型原因是重复引线（如上所述）或字段长度不匹配错误。

![](assets/image2016-1-20-11-3a19-3a58.png)

**[!DNL Salesforce]**

如果您使用[!DNL Salesforce]，则同步错误通知类似于下面的通知。 典型错误包括凭据过期和超出API限制。

![](assets/salesforcesyncerror.png)

## 参与度 {#engagement}

当人们在流中筋疲力尽时，我们会发送通知。 通知包括筋疲力尽的人数，以及一些其他信息。

![](assets/image2014-10-14-10-3a57-3a9.png)

## Facebook {#facebook}

如果您尝试在不接受服务条款的情况下将用户发送到Facebook，或者如果您在删除Marketo应用程序后尝试将用户发送到Facebook。

## 空闲触发器活动清理 {#idle-trigger-campaign-cleanup}

停用触发的智能营销活动不再获取任何活动。 了解有关[自动触发器营销活动清理](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md)的更多信息。

## LinkedIn {#linkedin}

在Marketo无法创建新受众时，登录或推送电子邮件至LinkedIn并进行三次尝试。

![](assets/linkedin.png)

## Web服务 {#web-services}

当达到每日配额时，您将会收到通知。 配额每晚在中部时间午夜重置。

>[!NOTE]
>
>我们在[开发人员文档](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/error-codes)中列出了您可能会收到的某些错误代码。

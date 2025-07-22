---
description: 回复日志记录 — Marketo文档 — 产品文档
title: 回复日志记录
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# 回复日志记录 {#reply-logging}

Sales Insight Actions允许您自动将潜在客户的回复记录到[!DNL Salesforce]。 允许您执行此操作的结构基于我们的电子邮件回复跟踪。 如果我们可以跟踪潜在客户的回复，则可以将该回复记录到[!DNL Salesforce]。

## 要求 {#requirements}

* 必须通过API日志记录来记录电子邮件
* 必须能够[跟踪回复](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* 必须与[!DNL Salesforce]连接
* 必须有[!DNL Salesforce]个[API调用](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm)可用

## 启用回复日志记录 {#enable-reply-logging}

1. 要启用回复日志记录，您可以转到[!DNL Salesforce]设置页面。 签出API日志记录后，您将看到用于检查&#x200B;_日志回复_&#x200B;的选项。

   >[!NOTE]
   >
   >回复日志记录遵循与记录已发送电子邮件相同的规则。 这包括如何记录电子邮件；如何记录到潜在客户和联系人；当存在重复记录时；如果未找到匹配记录。

## 正在将类型设置为在[!DNL Salesforce]中回复 {#setting-type-to-reply-in-salesforce}

从[!DNL Salesforce]报表中获取有意义的数据很重要。 由于能够将类型字段填充为“回复”，因此您可以通过报表获取这些数据。 与您的`[!DNL Salesforce] admin`合作以获取此设置。

1. 转到&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Customize]** > **[!UICONTROL Activities]** > **[!UICONTROL Task Fields]**。
1. 单击 **[!UICONTROL Type]**。
1. 在[!UICONTROL Task Type Picklist Values]下，单击&#x200B;**[!UICONTROL New]**。
1. 在空框中键入“Reply”。 确保将&#39;R&#39;大写，然后单击&#x200B;**[!UICONTROL Save]**。

   >[!NOTE]
   >
   >您无需在“类型”选取列表下选择“默认”。 [!DNL Sales Insight Actions]将看到此活动类型在您的[!DNL Salesforce]实例中可用，并相应地填充传入活动的任务字段。

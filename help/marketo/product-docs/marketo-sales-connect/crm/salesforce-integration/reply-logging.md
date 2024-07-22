---
unique-page-id: 14352480
description: 回复日志记录(SFDC) - Marketo文档 — 产品文档
title: 回复日志记录(SFDC)
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# 回复日志记录(SFDC) {#reply-logging-sfdc}

Sales Connect可使您能够自动将潜在客户的回复记录到Salesforce。 允许您执行此操作的结构基于我们的电子邮件回复跟踪。 如果我们可以跟踪潜在客户的回复，则可以将该回复记录到Salesforce。

## 要求 {#requirements}

* 必须通过API日志记录来记录电子邮件
* 必须能够[跟踪回复](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* 必须与Salesforce连接
* 必须有Salesforce [API调用](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm)可用

## 启用回复日志记录 {#enable-reply-logging}

1. 要启用回复日志记录，您可以转到Salesforce设置页面。 签出API日志记录后，您将看到用于检查&#x200B;_日志回复_&#x200B;的选项。

   >[!NOTE]
   >
   >回复日志记录遵循与记录已发送电子邮件相同的规则。 这包括如何记录电子邮件；如何记录到潜在客户和联系人；当存在重复记录时；如果未找到匹配记录。

## 在Salesforce中设置要回复的类型 {#setting-type-to-reply-in-salesforce}

从Salesforce报表中获取有意义的数据很重要。 由于能够将类型字段填充为“回复”，因此您可以通过报表获取这些数据。 与您的`Salesforce admin`合作以获取此设置。

1. 转到&#x200B;**设置** > **自定义** > **活动** > **任务字段**。
1. 单击&#x200B;**类型**。
1. 在任务类型选择列表值下，单击&#x200B;**新建**。
1. 在空框中键入“Reply”。 确保将&#39;R&#39;大写，然后单击&#x200B;**保存**。

   >[!NOTE]
   >
   >您无需在“类型”选取列表下选择“默认”。 Sales Connect将看到此Activity Type在您的Salesforce实例中可用，并相应地填充传入活动的task字段。

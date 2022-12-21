---
description: 回复日志记录 — Marketo文档 — 产品文档
title: 回复日志记录
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
source-git-commit: d960f0ad0d944bd2e74543f3ab15b59a8040b768
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# 回复日志记录 {#reply-logging}

Sales Insight Actions使您能够自动记录潜在客户对Salesforce的回复。 允许您执行此操作的结构基于我们的电子邮件回复跟踪。 如果我们能够跟踪潜在客户的回复，则可以将该回复记录到Salesforce。

## 要求 {#requirements}

* 必须通过API日志记录来记录电子邮件
* 必须能够 [跟踪回复](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* 必须与Salesforce连接
* 必须具有Salesforce [API调用](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) 可用

## 启用回复日志记录 {#enable-reply-logging}

1. 要启用回复日志记录，您可以转到Salesforce设置页面。 勾选API日志记录后，您将看到要检查的选项 _日志回复_.

   >[!NOTE]
   >
   >回复日志记录遵循您为记录已发送的电子邮件所采用的相同规则。 这包括电子邮件的记录方式；到潜在客户和联系人；记录重复的；如果找不到匹配记录。

## 在Salesforce中将类型设置为回复 {#setting-type-to-reply-in-salesforce}

从Salesforce报表中获取有意义的数据非常重要。 通过将类型字段填充为“回复”，您可以通过报表获取该数据。 与您的 `Salesforce admin` 来设置。

1. 转到 **设置** > **自定义** > **活动** > **任务字段**.
1. 单击 **类型**.
1. 在任务类型选取列表值下，单击 **新建**.
1. 在空框中键入“Reply”。 确保将“R”大写，然后单击 **保存**.

   >[!NOTE]
   >
   >您无需在“类型”(Type)选取列表下选择“默认”(Default)。 Sales Insight Actions将看到此活动类型在您的Salesforce实例中可用，并相应地填充传入活动的任务字段。

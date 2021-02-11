---
unique-page-id: 14352480
description: 回复日志记录(SFDC)- Marketo Docs —— 产品文档
title: 回复日志记录(SFDC)
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# 回复日志记录(SFDC){#reply-logging-sfdc}

Sales Connect为您提供自动记录潜在客户对Salesforce的回复的能力。 允许您执行此操作的结构基于我们的电子邮件回复跟踪。 如果我们可以跟踪潜在客户的回复，则可以将该回复记录到Salesforce。

## 要求{#requirements}

* 必须通过API记录记录电子邮件
* 必须能够[跟踪回复](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* 必须与Salesforce连接
* 必须具有可用的Salesforce [API调用](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm)

## 启用回复日志{#enable-reply-logging}

1. 要启用回复记录，您可以转到Salesforce设置页面。 一旦API日志记录被勾选，您将看到选项检查&#x200B;_日志回复_。

   >[!NOTE]
   >
   >回复日志记录遵循与记录已发送的电子邮件相同的规则。 这包括电子邮件的记录方式；到潜在客户和联系人；有重复记录时；如果找不到匹配记录。

## 在Salesforce中将类型设置为回复{#setting-type-to-reply-in-salesforce}

从Salesforce报表获取有意义的数据非常重要。 通过将“类型”字段填充为“回复”，您可以通过报表获取该数据。 与您的`Salesforce admin`合作以获取此设置。

1. 转至&#x200B;**设置** > **自定义** > **活动** > **任务字段**。
1. 单击&#x200B;**类型**。
1. 在“任务类型选择列表值”下，单击&#x200B;**新建**。
1. 在空框中键入“回复”。 确保将“R”大写，然后单击&#x200B;**保存**。

   >[!NOTE]
   >
   >您无需在“类型”(Type)选择列表下选择“默认”(Default)。 Sales Connect将看到此活动类型在您的Salesforce实例中可用，并相应地在传入活动上填充任务字段。

---
unique-page-id: 14352480
description: 回复日志记录(SFDC)- Marketo Docs —— 产品文档
title: 回复日志记录(SFDC)
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# 回复日志记录(SFDC) {#reply-logging-sfdc}

Sales Connect为您提供自动记录潜在客户对Salesforce的回复的能力。 允许您执行此操作的结构基于我们的电子邮件回复跟踪。 如果我们可以跟踪潜在客户的回复，则可以将该回复记录到Salesforce。

## 要求 {#requirements}

* 必须通过API记录记录电子邮件
* 必须能够 [跟踪回复](http://docs.marketo.com/x/BYPS)
* 必须与Salesforce连接
* 必须有Salesforce [API调用](http://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm)

## 启用回复记录 {#enable-reply-logging}

1. 要启用回复记录，您可以转到Salesforce [设置页面](http://docs.marketo.com/pages/assets/external-link.jspa) 。 一旦API记录被勾选，您将看到选项“勾选*日志回复”。\
   *

   >[!NOTE]
   >
   >回复日志记录遵循与记录已发送的电子邮件相同的规则。 这包括电子邮件的记录方式；到潜在客户和联系人；有重复记录时；如果找不到匹配记录。

## 在Salesforce中将类型设置为回复 {#setting-type-to-reply-in-salesforce}

从Salesforce报表获取有意义的数据非常重要。 通过将“类型”字段填充为“回复”，您可以通过报表获取该数据。 与您合作， `Salesforce admin` 获得此设置。

1. 转到**设置**>**自定义**>**活动**> **任务字段**。
1. 单击 **类型**。
1. 在“任务类型选择列表值”下，单击“ **新建**”。
1. 在空框中键入“回复”。 确保将“R”大写，然后单击“保 **存**”。

   >[!NOTE]
   >
   >您无需在“类型”(Type)选择列表下选择“默认”(Default)。 Sales Connect将看到此活动类型在您的Salesforce实例中可用，并相应地在传入活动上填充任务字段。


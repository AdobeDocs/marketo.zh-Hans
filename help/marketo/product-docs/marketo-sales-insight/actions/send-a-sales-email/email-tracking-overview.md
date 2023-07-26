---
description: 电子邮件跟踪概述 — Marketo文档 — 产品文档
title: 电子邮件跟踪概述
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 电子邮件跟踪概述 {#email-tracking-overview}

## 回复跟踪的工作方式 {#how-reply-tracking-works}

回复跟踪是通过查看您发送的每封电子邮件中的邮件ID完成的。 每个电子邮件都包含一个唯一的消息ID，使我们能够有一些最佳的回复跟踪。

>[!PREREQUISITES]
>
>与电子邮件服务器的连接： Sales Connect必须与您的收件箱连接，以便我们了解新回复何时到达。 您需要将您的Sales Connect帐户连接到Gmail。 如果您使用的是Outlook，我们需要与您的Exchange服务器集成。

如果Sales Connect无法跟踪潜在客户对电子邮件的回复，它将无法基于回复检测停止促销活动或将回复记录到Salesforce。 什么意思是任何电子邮件地址都可以回复？

这意味着，如果您向flynn@flynnsarcade.com发送电子邮件，而他使用kevinf@flynnsarcade.com做出响应，则我们可以跟踪该响应。 此外，如果您发送电子邮件至flynn@flynnsarcade.com和CC alan@encom.com ，而Alan写回了您，它还将检测该回复并结束营销活动。

## 如何跟踪您的电子邮件附件 {#how-to-track-your-email-attachments}

Sales Connect提供了对附件(.doc、.ppt、.pdf)的跟踪，以便您查看附件打开/下载的时间，以及收件人浏览的页面。 我们将允许您同时使用我们的可跟踪附件功能 [Web应用程序](https://toutapp.com/login) 和Gmail(或Google应用程序)。

>[!NOTE]
>
>附件跟踪仅适用于我们的团队计划（从我们的g3startup计划开始）。

**如何发送您的第一个可跟踪附件**

1. 撰写电子邮件或编辑模板，然后单击 **内容** 按钮。

1. 上传附件并将其发送。 我们支持PDF、Word文档和Powerpoint演示文稿。

1. 选择 **添加到电子邮件**.

1. 单击 **发送** 并触发您的实时信息源。 您会在收件人打开并通过附件进行页面浏览时看到他们。

>[!TIP]
>
>如果您不想跟踪附件，只需单击“附加文件”，就不会跟踪此附件。

## 视图跟踪的工作方式 {#how-view-tracking-works}

我们通过在您发送的电子邮件中放置不可见的图像来跟踪电子邮件打开情况。

如果有人回复了您的电子邮件，但Sales Connect说未查看该电子邮件，则收件人可能未在其电子邮件客户端中启用图像（即，单击电子邮件中的“单击此处下载图像”消息）。

关于如何在电子邮件中获得更好的跟踪统计信息的一些提示：

* 在电子邮件中加入图像（如徽标），以便鼓励收件人启用图像功能来查看邮件。
* 在电子邮件中包含作为行动号召的链接。

## 测试电子邮件未显示为已查看 {#test-email-not-showed-as-viewed}

即使您将消息发送到其他电子邮件地址，我们也不会记录您查看您在实时信息源中发送给自己的任何电子邮件。 我们的跟踪是基于设备的；只要您使用的是已登录Sales Connect的计算机，我们就会过滤掉该活动。

原因何在？ Sales Connect非常智能，而且我们的活跃用户绝不会原谅我们每次查看他们发送的电子邮件时，会在“实时信息源”活动中弹出他们自己的信息。

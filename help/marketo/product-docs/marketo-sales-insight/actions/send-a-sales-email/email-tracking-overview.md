---
description: 电子邮件跟踪概述 — Marketo文档 — 产品文档
title: 电子邮件跟踪概述
hide: true
hidefromtoc: true
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 电子邮件跟踪概述 {#email-tracking-overview}

## 回复跟踪的工作原理 {#how-reply-tracking-works}

回复跟踪通过查看您发送的每封电子邮件中的消息ID来完成。 每封电子邮件都包含一个唯一的消息ID，以便我们能够进行一些最佳的回复跟踪。

>[!PREREQUISITES]
>
>与电子邮件服务器的连接：Sales Connect必须与您的收件箱连接，以便我们知道何时收到新回复。 您需要将Sales Connect帐户连接到Gmail。 如果您使用的是Outlook，则需要与您的exchange服务器集成。

如果Sales Connect无法跟踪您的潜在客户对您电子邮件的回复，则将无法基于回复检测停止营销活动或将回复记录到Salesforce。 任何可回复的电子邮件地址是什么意思？

这意味着，如果您通过电子邮件发送flynn@flynnsarcade.com，而他回复了kevinf@flynnsarcade.com，则我们能够跟踪回复。 此外，如果您通过电子邮件发送flynn@flynnsarcade.com和CC alan@encom.com,Alan将您回复，它也会检测到回复并结束营销活动。

## 如何跟踪电子邮件附件 {#how-to-track-your-email-attachments}

Sales Connect选件跟踪您的附件(.doc、.ppt、.pdf)，以便您能够查看其打开/下载的时间，以及查看您的收件人正在浏览的页面。 我们将允许您使用 [Web应用程序](https://toutapp.com/login) 和Gmail(或Google应用程序)。

>[!NOTE]
>
>附件跟踪仅适用于我们的团队计划（从我们的g3启动计划开始）。

**如何发送您的第一个可跟踪附件**

1. 撰写电子邮件或编辑模板，然后单击 **内容** 按钮。

1. 上载附件并将其发出。 我们支持PDF、Word文档和Powerpoint演示文稿。

1. 选择 **添加到电子邮件**.

1. 单击 **发送** 并触发您的实时动态消息。 在收件人打开并通过附件页面时，您将看到这些收件人。

>[!TIP]
>
>如果不想跟踪附件，只需单击“附加文件”，此附件将不被跟踪。

## 视图跟踪的工作原理 {#how-view-tracking-works}

我们通过在您发送的电子邮件中置入不可见的图像来跟踪电子邮件打开情况。

如果有人回复您的电子邮件，但Sales Connect表示该电子邮件未被查看，则收件人很可能未在其电子邮件客户端中启用图像（即，单击电子邮件中的“单击此处下载图像”消息）。

有关在电子邮件中获取更好的跟踪统计资料的一些提示：

* 在电子邮件中包含图像（如徽标），以便鼓励收件人启用图像以查看您的消息。
* 在电子邮件中包含作为行动动员的链接。

## 测试电子邮件未显示为已查看 {#test-email-not-showed-as-viewed}

即使您将消息发送到其他电子邮件地址，我们也不会记录您查看您在实时动态消息中发送给自己的任何电子邮件。 我们的跟踪基于设备；只要您使用的计算机已登录Sales Connect，我们就会过滤掉该活动。

原因？ Sales Connect是智能的，我们的活跃用户在每次查看他们发送的电子邮件时，如果在实时信息源活动中弹出他们自己的信息，永远不会原谅我们。

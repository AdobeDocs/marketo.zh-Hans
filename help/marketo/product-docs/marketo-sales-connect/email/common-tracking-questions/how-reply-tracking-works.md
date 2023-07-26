---
unique-page-id: 14352482
description: 回复跟踪的工作方式 — Marketo文档 — 产品文档
title: 回复跟踪的工作方式
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# 回复跟踪的工作方式 {#how-reply-tracking-works}

回复跟踪是通过查看您发送的每封电子邮件中的邮件ID完成的。 每个电子邮件都包含一个唯一的消息ID，使我们能够有一些最佳的回复跟踪。

>[!PREREQUISITES]
>
>**与电子邮件服务器的连接：** Sales Connect必须连接到您的收件箱，以便我们知道何时收到新的回复。 您需要拥有您的Sales Connect帐户 [已连接到Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). 如果您使用的是Outlook，我们需要与您的集成 [exchange服务器](https://toutapp.com/next#settings/exchange_settings).

如果Sales Connect无法跟踪潜在客户对电子邮件的回复，它将无法基于回复检测停止促销活动或将回复记录到Salesforce。  什么意思是任何电子邮件地址都可以回复？

这意味着，如果您向flynn@flynnsarcade.com发送电子邮件，而他使用kevinf@flynnsarcade.com做出响应，则我们可以跟踪该响应。 此外，如果您发送电子邮件至flynn@flynnsarcade.com和CC alan@encom.com ，而Alan写回了您，它还将检测该回复并结束营销活动。

---
unique-page-id: 14352482
description: 回复跟踪的工作原理 — Marketo Docs — 产品文档
title: 回复跟踪的工作原理
translation-type: tm+mt
source-git-commit: 073b73255d49f859c32c8b4793e6798f02f7a5c4
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# 回复跟踪的工作原理{#how-reply-tracking-works}

回复跟踪是通过查看您发送的每封电子邮件中的邮件ID来完成的。 每封电子邮件都包含一个唯一的邮件ID，它允许我们进行一些最佳的回复跟踪。

>[!PREREQUISITES]
>
>**与电子邮件服务器连** 接：Sales Connect必须与您的收件箱连接，以便我们了解新回复何时到达。您需要将您的Sales Connect帐户[连接到Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)。 如果您使用Outlook，我们需要与您的[exchange server](https://toutapp.com/next#settings/exchange_settings)集成。

如果Sales Connect无法跟踪潜在客户对您电子邮件的回复，则无法基于回复检测停止活动或记录回复到Salesforce。  什么是可以回复的电子邮件地址？

这意味着，如果您发送电子邮件至flynn@flynnsarcade.com，而他以kevinf@flynnsarcade.com回复，我们可以跟踪回复。 此外，如果您通过电子邮件发送flynn@flynnsarcade.com和CC alan@encom.com，而Alan将您回复，它还会检测回复并结束活动。

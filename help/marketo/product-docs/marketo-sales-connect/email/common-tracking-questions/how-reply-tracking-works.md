---
unique-page-id: 14352482
description: 回复跟踪的工作原理- Marketo Docs —— 产品文档
title: 回复跟踪的工作方式
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# 回复跟踪的工作原理{#how-reply-tracking-works}

回复跟踪是通过查看您发送的每封电子邮件中的邮件ID来完成的。 每封电子邮件都包含一个唯一的邮件ID，它允许我们进行一些最佳回复跟踪。

>[!PREREQUISITES]
>
>**与电子邮件服务器** 连接：Sales Connect必须与您的收件箱连接，以便我们知道何时收到新回复。您需要将Sales Connect帐户[连接到Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-tab-for-gmail-users.md)。 如果您使用Outlook，我们需要与您的[exchange服务器](https://toutapp.com/next#settings/exchange_settings)集成。

如果Sales Connect无法跟踪潜在客户对您电子邮件的回复，则无法基于回复检测或记录回复到Salesforce的活动来停止。  我们指的是任何电子邮件地址都可以回复？

这意味着，如果您通过电子邮件发送flynn@flynnsarcade.com，而他以kevinf@flynnsarcade.com做出响应，我们将能够跟踪回复。 此外，如果您通过电子邮件发送flynn@flynnsarcade.com和CC alan@encom.com，而Alan将您写回，它还会检测回复并结束活动。

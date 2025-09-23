---
unique-page-id: 14352482
description: 回复跟踪的工作方式 — Marketo文档 — 产品文档
title: 回复跟踪的工作原理
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 4%

---

# 回复跟踪的工作原理 {#how-reply-tracking-works}

回复跟踪是通过查看您发送的每封电子邮件中的邮件ID完成的。 每个电子邮件都包含一个唯一的消息ID，使我们能够有一些最佳的回复跟踪。

>[!PREREQUISITES]
>
>**与电子邮件服务器的连接：** [!DNL Sales Connect]必须与您的收件箱连接，以便我们知道新回复何时到达。 您需要将您的[!DNL Sales Connect]帐户[连接到Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)。 如果您使用的是[!DNL Outlook]，我们需要与您的[Exchange服务器](https://toutapp.com/next#settings/exchange_settings)集成。

如果[!DNL Sales Connect]无法跟踪您的潜在客户对电子邮件的回复，它将无法基于回复检测停止营销活动或将该回复记录到[!DNL Salesforce]。  什么意思是任何电子邮件地址都可以回复？

这意味着，如果您向<flynn@flynnsarcade.com>发送电子邮件，而他通过<kevinf@flynnsarcade.com>进行回复，则我们可以跟踪该回复。 此外，如果您发送电子邮件<flynn@flynnsarcade.com>和抄送<alan@encom.com>，而Alan将您写回，则它还会检测回复并结束营销活动。

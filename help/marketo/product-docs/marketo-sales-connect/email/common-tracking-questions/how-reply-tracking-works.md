---
unique-page-id: 14352482
description: 回复跟踪的工作原理- Marketo Docs —— 产品文档
title: 回复跟踪的工作方式
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# 回复跟踪的工作方式 {#how-reply-tracking-works}

回复跟踪是通过查看您发送的每封电子邮件中的邮件ID来完成的。 每封电子邮件都包含一个唯一的邮件ID，它允许我们进行一些最佳回复跟踪。

>[!PREREQUISITES]
>
>**与电子邮件服务器的连接：** Sales Connect必须与您的收件箱连接，以便我们知道何时收到新的回复。 您需要将Sales Connect帐户连 [接到Gmail](http://docs.marketo.com/x/kYMOAQ)。 如果您使用Outlook，我们需要与您的exchange服务器 [集成](http://toutapp.com/next#settings/exchange_settings)。

如果Sales Connect无法跟踪潜在客户对您电子邮件的回复，则无法基于回复检测或记录回复到Salesforce的活动来停止。  我们指的是任何电子邮件地址都可以回复？

这意味着，如果您发 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#783217162b16170f3830170d0b1d2b0c190a13561b1715) 送电子邮件并 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#c08aafae93aeafb78094a8a58ea9a7a8b4b397a1b4a3a8eea3afad)他做出响应，我们可以跟踪回复。 此外，如果您通过电 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#450f2a2b162b2a32050d2a303620163124372e6b262a28) 子邮件 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#3e5f525f507e5b505d5153105d5153)和抄送，而Alan将您回复，它还会检测回复并结束活动。

---
description: 电子邮件跟踪概述 — Marketo文档 — 产品文档
title: 电子邮件跟踪概述
hide: true
hidefromtoc: true
source-git-commit: 8789ed464f532bbe76c2cb456374d9c0f505ece0
workflow-type: tm+mt
source-wordcount: '186'
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

## 回复跟踪的工作原理 {#how-reply-tracking-works}

文本

## 如何跟踪电子邮件附件 {#how-to-track-your-email-attachments}


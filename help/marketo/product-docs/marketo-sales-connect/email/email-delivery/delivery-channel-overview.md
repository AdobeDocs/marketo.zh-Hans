---
unique-page-id: 14352407
description: 投放渠道概述 — Marketo Docs — 产品文档
title: 投放渠道概述
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---


# 投放渠道概述{#delivery-channel-overview}

Marketo Sales Connect为您提供多种投递电子邮件的选项。 本文将回顾您可以利用的投放渠道、如何选择它们以及何时选择它们。

## 建议：通过电子邮件连接{#recommended-gmail-or-exchange-via-email-connection}的Gmail或Exchange

Sales Connect允许通过我们的电子邮件连接服务简化设置并增强交付能力。 电子邮件连接允许每个用户连接到其[Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)或[Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)帐户到Sales Connect，以用作所有Sales Connect电子邮件的投放渠道。

与其他投放渠道选项相比，利用Gmail或Exchange具有一些明显的优势：

* 这是一家久经考验的投放渠道，声誉卓著，有助于保持高交付能力。
* 身份验证方法（如SPF和DKIM）已由您的IT团队配置和管理，因此没有其他设置。
* 在给定电子邮件网络内发送电子邮件(即以Exchange用户身份向通过Exchange接收电子邮件的公司发送电子邮件)有助于进一步提高交付能力。

请务必注意，这些投放渠道有自己的发送限制，这些限制由Microsoft和Google强制实施。 为了克服这一问题，我们使用限制机制来帮助用户保持这些限制。 在此处了解有关[电子邮件限制的更多信息](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)。

>[!NOTE]
>
>默认情况下，O365插件将始终使用您的exchange投放渠道，而Gmail插件将始终利用您的Gmail投放渠道从插件发送电子邮件。

**跳出跟踪**:MSC可以检测发送到发件人收件箱的弹回消息，从而检测Exchange Online或Gmail用户的弹回。这些弹出通知将汇总到模板分析、活动分析和用户实时信息源通知中。 Exchange On-Prem客户不支持跳出跟踪。

## 通过SMTP {#custom-delivery-channel-via-smtp}自定义投放渠道

Sales Connect会优惠连接第三方SMTP服务器以用作销售团队首选投放渠道的其他选项。

对于以电子邮件量为首要任务的销售团队而言，使用第三方SMTP提供商是一个不错的选择。 SMTP提供商（如Sendgrid和Sparkpost）经过优化，可满足批量电子邮件投放的需求，并可进行扩展以满足那些希望部署大量电子邮件的用户的需求。

此外，第三方SMTP提供商还优惠了大量功能来帮助支持团队的可交付性需求(如电子邮件投放报告和专用IP地址)，因此对于那些希望获得更精细的控制并了解其销售电子邮件投放渠道的人来说，这是一个不错的选择。

## MSC Servers（旧版）{#msc-servers-legacy}

MSC服务器仅对某些旧版ToutApp客户可用。 这些客户将在电子邮件设置中看到MSC服务器。 所有非传统客户都不会将MSC视为一个选项，应将他们的Gmail或Outlook帐户连接到Sales Connect，以解锁投放渠道。

MSC服务器不支持DKIM和SPF身份验证方法，这可以降低交付率。 因此，我们建议所有客户连接到Gmail或Outlook，以获得最佳交付能力。

## Marketo服务器{#marketo-servers}

Marketo电子邮件服务器不与Sales Connect集成。 Marketo服务器经过优化，可进行批量投放，使其能够根据营销人员的需求进行扩展。 但是，Gmail和Exchange在1:1销售通信方面的成功率更高，因此我们建议将这些服务器用于您的销售通信。

>[!MORELIKETHIS]
>
>* [针对Gmail用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlook用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [设置自定义投放渠道](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [电子邮件连接限制](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)


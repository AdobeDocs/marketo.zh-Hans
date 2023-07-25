---
unique-page-id: 14352407
description: 投放渠道概述 — Marketo文档 — 产品文档
title: 投放渠道概述
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# 投放渠道概述 {#delivery-channel-overview}

Marketo Sales Connect为您提供多种电子邮件发送选项。 本文将介绍您可以利用的投放渠道、如何选择这些渠道以及何时选择其中一个渠道。

## 建议：通过电子邮件连接使用Gmail或Exchange {#recommended-gmail-or-exchange-via-email-connection}

Sales Connect允许通过我们的电子邮件连接服务简化设置和增强可投放性。 电子邮件连接允许每个用户连接到其 [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) 或 [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) 帐户到Sales Connect ，用作所有Sales Connect电子邮件的首选投放渠道。

与其他投放渠道选项相比，利用Gmail或Exchange具有一些明显的优势：

* 这是一个久负盛名的交付渠道，有助于保持高可交付性。
* SPF和DKIM等身份验证方法已由IT团队配置和管理，因此无需额外设置。
* 在给定的电子邮件网络中发送电子邮件（即，以Exchange用户身份向通过Exchange接收电子邮件的公司发送电子邮件）可以帮助您进一步提高可投放性。

请务必注意，这些投放渠道具有其自身的发送限制，这些限制由Microsoft和Google实施。 为此，我们利用限制机制来帮助用户保持在这些限制之内。 详细了解 [在此限制电子邮件](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>默认情况下，O365插件将始终使用您的Exchange投放渠道，而Gmail插件将始终使用Gmail投放渠道从插件投放电子邮件。

**退回跟踪**：MSC可以通过检测发送到发件人收件箱的退回消息来检测Exchange Online或Gmail用户的退回。 这些退回通知将汇总到用户的模板分析、Campaign分析和实时信息源通知中。 Exchange内部部署客户不支持退回跟踪。

## 通过SMTP的自定义投放渠道 {#custom-delivery-channel-via-smtp}

Sales Connect提供了连接第三方SMTP服务器以用作销售团队首选交付渠道的附加选项。

对于电子邮件量是第一优先级的销售团队来说，利用第三方SMTP提供商是一个很好的选择。 SMTP提供商（如Sendgrid和Sparkpost ）已针对批量电子邮件投放的需求进行了优化，并且可以扩展以满足希望部署大量电子邮件的客户的需求。

此外，第三方SMTP提供商提供了大量功能来帮助支持您团队的可投放性需求（如电子邮件投放报告和专用IP地址），因此对于希望更精细地控制其销售电子邮件投放渠道并使其可见性的客户而言，这是一个很好的选择。

## MSC服务器（旧版） {#msc-servers-legacy}

MSC服务器仅适用于某些旧版ToutApp客户。 这些客户将在其电子邮件设置中看到MSC服务器。 所有非旧版客户都不会看到MSC选项，因此应将他们的Gmail或Outlook帐户连接到Sales Connect以解锁投放渠道。

MSC服务器不支持DKIM和SPF认证方式，降低了传递率。 因此，我们建议所有客户连接到Gmail或Outlook以获得最佳可投放性。

## Marketo服务器 {#marketo-servers}

Marketo电子邮件服务器不与Sales Connect集成。 Marketo服务器针对批量交付进行了优化，以允许根据营销人员的需求进行扩展。 但是，Gmail和Exchange在1:1销售沟通方面有更高的成功率，因此我们建议将这些服务器用于您的销售沟通。

>[!MORELIKETHIS]
>
>* [Gmail用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlook用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [设置自定义投放渠道](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [电子邮件连接限制](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

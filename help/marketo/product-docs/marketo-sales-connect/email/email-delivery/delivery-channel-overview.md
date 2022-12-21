---
unique-page-id: 14352407
description: 交付渠道概述 — Marketo文档 — 产品文档
title: 投放渠道概述
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# 投放渠道概述 {#delivery-channel-overview}

Marketo Sales Connect为您提供多个用于发送电子邮件的选项。 本文将回顾您可以利用的投放渠道、选择方式以及何时选择一个渠道来替代另一个渠道。

## 建议：通过电子邮件连接Gmail或Exchange {#recommended-gmail-or-exchange-via-email-connection}

Sales Connect允许通过我们的Email Connection服务简化设置并增强可投放性。 电子邮件连接允许每个用户连接到其 [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) 或 [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) 帐户到Sales Connect以用作所有Sales Connect电子邮件的选择交付渠道。

与其他投放渠道选项相比，利用Gmail或Exchange具有一些明显的优势：

* 这是一个久经考验的投放渠道，拥有良好的声誉，有助于保持高投放能力。
* 身份验证方法（如SPF和DKIM）已由您的IT团队配置和管理，因此没有其他设置。
* 在给定的电子邮件网络内发送电子邮件（即以Exchange用户身份向通过Exchange接收电子邮件的公司发送电子邮件），这有助于进一步提高投放能力。

请务必注意，这些投放渠道具有自己的发送限制，这些限制由Microsoft和Google强制实施。 为了克服这种情况，我们使用限制机制来帮助用户保持在这些限制范围内。 详细了解 [此处为电子邮件限制](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>默认情况下，O365插件将始终使用您的Exchange投放渠道，而Gmail插件将始终利用您的Gmail投放渠道从插件投放电子邮件。

**跳出跟踪**:MSC可检测发送到发件人收件箱的退回邮件，以检测Exchange Online或Gmail用户的退回。 这些退回通知将汇总到模板分析、促销活动分析和用户的实时信息源通知中。 Exchange On-Prem客户不支持跳出跟踪。

## 通过SMTP的自定义投放渠道 {#custom-delivery-channel-via-smtp}

Sales Connect提供了连接第三方SMTP服务器以用作销售团队首选交付渠道的额外选项。

对于电子邮件量是销售团队而言，利用第三方SMTP提供程序是一个绝佳选择，其中电子邮件量是第一要务。 Sendgrid和Sparkpost等SMTP提供程序经过优化，可满足批量电子邮件投放的需求，并且可以扩展以满足那些希望部署大量电子邮件的用户的需求。

此外，第三方SMTP提供程序还提供大量功能来帮助支持您团队的可投放性需求（如电子邮件投放报告和专用IP地址），对于那些希望获得更精细控制并了解其销售电子邮件投放渠道的用户而言，这是一个绝佳选项。

## MSC服务器（旧版） {#msc-servers-legacy}

MSC服务器仅适用于某些旧版ToutApp客户。 这些客户将在其电子邮件设置中看到MSC服务器。 所有非旧版客户都不会将MSC视为一个选项，应将其Gmail或Outlook帐户连接到Sales Connect以解锁投放渠道。

MSC服务器不支持DKIM和SPF身份验证方法，这可以降低可投放性率。 因此，我们建议所有客户连接到Gmail或Outlook，以获得最佳投放能力。

## Marketo服务器 {#marketo-servers}

Marketo电子邮件服务器未与Sales Connect集成。 Marketo服务器经过优化，可批量交付，从而可以根据营销人员的需求进行扩展。 但是，Gmail和Exchange的1:1销售通信成功率较高，因此我们建议将这些服务器用于您的销售通信。

>[!MORELIKETHIS]
>
>* [面向Gmail用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [面向Outlook用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [设置自定义投放渠道](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [电子邮件连接限制](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)


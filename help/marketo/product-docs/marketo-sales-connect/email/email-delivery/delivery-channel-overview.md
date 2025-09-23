---
unique-page-id: 14352407
description: 投放渠道概述 — Marketo文档 — 产品文档
title: 发送渠道概述
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 1%

---

# 发送渠道概述 {#delivery-channel-overview}

Marketo [!DNL Sales Connect]为您提供多种电子邮件发送选项。 本文将介绍您可以利用的投放渠道、如何选择渠道以及何时选择渠道。

## 建议： Gmail或通过电子邮件连接发送[!DNL Exchange] {#recommended-gmail-or-exchange-via-email-connection}

[!DNL Sales Connect]允许通过我们的电子邮件连接服务简化设置和增强可投放性。 [!UICONTROL Email Connection]允许每个用户连接到他们的[Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)或[Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)帐户，以将其用作所有[!DNL Sales Connect]电子邮件的首选传递渠道。[!DNL Sales Connect]

与其他投放渠道选项相比，使用Gmail或[!DNL Exchange]具有一些明显的优势：

* 这是一个久经考验的交付渠道，拥有良好的声誉，有助于保持高可交付性。
* SPF和DKIM等身份验证方法已由IT团队配置和管理，因此无需额外设置。
* 在给定的电子邮件网络内发送电子邮件（即，以[!DNL Exchange]用户身份向通过[!DNL Exchange]接收电子邮件的公司发送电子邮件）可以有助于进一步提高可投放性。

请务必注意，这些投放渠道具有其自身的发送限制，这些限制由Microsoft和Google强制实施。 为了应对这种情况，我们使用限制机制来帮助用户保持在这些限制之内。 在此处了解有关[电子邮件限制的详细信息](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)。

>[!NOTE]
>
>默认情况下，O365插件将始终使用您的Exchange投放渠道，Gmail插件将始终使用Gmail投放渠道从插件投放电子邮件。

**退回跟踪**： MSC可以通过检测发送到发件人收件箱的退回邮件来检测[!DNL Exchange Online]或Gmail用户的退回。 这些退回通知将汇总到用户的模板分析、营销活动分析和实时信息源通知中。 [!DNL Exchange]内部部署客户不支持退回跟踪。

## 通过SMTP自定义投放渠道 {#custom-delivery-channel-via-smtp}

[!DNL Sales Connect]提供了附加选项，用于连接要用作销售团队首选投放渠道的第三方SMTP服务器。

对于电子邮件量是第一优先级的销售团队来说，利用第三方SMTP提供商是一个很好的选择。 SMTP提供商（如[!DNL Sendgrid]和[!DNL Sparkpost]）已针对批量电子邮件投放的需求进行了优化，并且可以扩展以满足那些希望部署大量电子邮件的客户的需求。

此外，第三方SMTP提供商提供了大量功能来帮助支持您团队的可投放性需求（例如电子邮件投放报告和专用IP地址），对于希望获得更精细的控制以及销售电子邮件投放渠道可见度的客户来说，这是一个绝佳选项。

## MSC服务器（旧版） {#msc-servers-legacy}

MSC服务器仅适用于某些旧版ToutApp客户。 这些客户将在电子邮件设置中看到MSC服务器。 所有非传统客户都不会将MSC视为选项，应将其Gmail或[!DNL Outlook]帐户连接到[!DNL Sales Connect]以解锁投放渠道。

MSC服务器不支持DKIM和SPF身份验证方法，这可能会降低投放率。 因此，我们建议所有客户连接到Gmail或[!DNL Outlook]以获得最佳可投放性。

## Marketo服务器 {#marketo-servers}

Marketo电子邮件服务器未与[!DNL Sales Connect]集成。 Marketo服务器针对批量交付进行了优化，以便能够根据营销人员的需求进行扩展。 但是，Gmail和[!DNL Exchange]在1:1销售通信中具有更高的成功率，因此我们建议将这些服务器用于您的销售通信。

>[!MORELIKETHIS]
>
>* Gmail用户的[电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [用户 [!DNL Outlook] 的](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)电子邮件连接
>* [设置自定义投放渠道](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [电子邮件连接限制](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

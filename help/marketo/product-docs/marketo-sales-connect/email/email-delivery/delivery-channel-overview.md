---
unique-page-id: 14352407
description: 投放渠道概述 — Marketo Docs — 产品文档
title: 投放渠道概述
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---


# 投放渠道概述{#delivery-channel-overview}

我们将分解您可以利用的三种不同渠道，如何选择它们，何时选择它们，以及它们周围的细微差别。

>[!NOTE]
>
>仅当您从[Web应用程序](https://toutapp.com/login)发送电子邮件时，此信息才相关。 如果您在Gmail或Outlook中使用Sales Connect，您的电子邮件将通过这些电子邮件服务器发送。

## MSC电子邮件服务器（默认）{#msc-email-servers-default}

默认情况下，将为电子邮件的投放选择此方法。 MSC电子邮件服务器是不使用Gmail或Outlook的用户的绝佳选择。 此外，由于它们是我们的服务器，因此我们能够接收有关弹回或失败投放的任何错误消息，并将它们呈现到“对话”选项卡的“失败投放”部分中。

使用MSC服务器的另一个好处是，当使用[电子邮件标识](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/add-identity.md)时，收件人将看到您创建的标识的电子邮件地址。

使用MSC服务器时，您的收件人可能会看到“via toutapp.com”标记。 这是他们的电子邮件客户端，告知他们电子邮件是使用Sales Connect发送的。

有关详细信息，请查看此[Gmail帮助文章](https://support.google.com/mail/answer/1311182?hl=en)。

>[!NOTE]
>
>我们的MSC服务器没有可用的[DMARC记录](https://dmarc.org/)。 它们不能列在您自己的服务器上的白名单中。

## Gmail服务器{#gmail-server}

如果公司的电子邮件提供商是Gmail，您可以利用现有帐户发送Sales Connect电子邮件。 如果您希望避免“via toutapp.com”信息，并且希望依赖公司域的声誉和交付能力，这是一个不错的选择。 使用Gmail服务器的另一个好处是，从Web应用程序发送的任何内容都将自动添加到您的Gmail发送文件夹。

我们只能正确连接一个Gmail帐户（一个电子邮件地址），该帐户将发送您的Sales Connect电子邮件。 这意味着如果您使用多个电子邮件身份，则查看详细信息时只会显示我们所连接帐户的地址。

在Web应用程序中，您的标识将显示为您已创建的标识（上）。 但是，通过Gmail服务器发送将显示连接帐户的地址。

>[!NOTE]
>
>由于Sales Connect不直接管理您的Gmail服务器，因此我们不会在Web应用程序中记录退回的电子邮件事件。

## 自定义SMTP服务器{#custom-smtp-server}

购买您自己的服务器？ 是否使用Microsoft Exchange环境? 这是您的选择。 请查看[这些说明](https://docs.marketo.com/x/zYTS)，了解如何设置。 与Gmail服务器一样，由于Sales Connect不直接管理您的服务器，因此我们不会在Web应用程序中记录退回的电子邮件事件。

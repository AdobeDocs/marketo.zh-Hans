---
unique-page-id: 14352407
description: 投放渠道概述- Marketo Docs —— 产品文档
title: 投放渠道概述
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---


# 投放渠道概述{#delivery-channel-overview}

我们将分析您可以利用的三个不同渠道、如何选择它们、何时选择它们，以及它们周围的细微差别。

>[!NOTE]
>
>仅当您从[Web应用程序](https://toutapp.com/login)发送电子邮件时，此信息才相关。 如果您在Gmail或Outlook中使用Sales Connect，则您的电子邮件将通过这些电子邮件服务器发送。

## MSC电子邮件服务器（默认）{#msc-email-servers-default}

默认情况下，将为电子邮件的投放选择此方法。 对于未使用Gmail或Outlook的用户来说，MSC电子邮件服务器是一个极好的选择。 此外，由于它们是我们的服务器，因此我们能够接收有关弹回或失败投放的任何错误消息，并在“对话”选项卡的“失败投放”部分将它们呈现给您。

使用MSC服务器的另一个好处是，当使用[电子邮件标识](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/add-identity.md)时，收件人将看到您创建的标识的电子邮件地址。

使用MSC服务器时，收件人可能会看到“via toutapp.com”标记。 这是他们的电子邮件客户端，告知他们电子邮件是使用Sales Connect发送的。

有关详细信息，请查阅此[Gmail帮助文章](https://support.google.com/mail/answer/1311182?hl=en)。

>[!NOTE]
>
>我们的MSC服务器没有提供的[DMARC记录](https://dmarc.org/)。 它们不能列入您自己的服务器的白名单。

## Gmail服务器{#gmail-server}

如果您的公司的电子邮件提供商是Gmail，您可以利用现有帐户发送Sales Connect电子邮件。 如果您希望避免“通过toutapp.com”信息，并且希望依赖公司的域名和交付能力，则这是一个不错的选项。 使用Gmail服务器的另一个好处是，您从Web应用程序发送的任何内容都将自动添加到您的Gmail发送的文件夹。

我们只能正确连接将传送您的Sales Connect电子邮件的单个Gmail帐户（一个电子邮件地址）。 这意味着如果您使用多个电子邮件标识，则查看详细信息时只会显示我们所连接帐户的地址。

在Web应用程序中，您的标识将像您创建的一样显示（上图）。 但是，通过Gmail服务器发送会显示已连接帐户的地址。

>[!NOTE]
>
>由于Sales Connect不直接管理您的Gmail服务器，因此我们不会在Web应用程序中记录退回的电子邮件事件。

## 自定义SMTP服务器{#custom-smtp-server}

购买您自己的服务器？ 是否使用Microsoft Exchange环境? 这是您的选择。 有关设置，请查看[这些说明](http://docs.marketo.com/x/zYTS)。 与Gmail服务器一样，由于Sales Connect不直接管理您的服务器，因此我们不会在Web应用程序中记录退回的电子邮件事件。

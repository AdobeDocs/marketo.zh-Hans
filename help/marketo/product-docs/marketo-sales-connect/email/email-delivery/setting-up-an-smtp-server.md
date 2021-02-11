---
unique-page-id: 14746594
description: 设置SMTP服务器- Marketo Docs —— 产品文档
title: 设置SMTP服务器
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---


# 设置SMTP服务器{#setting-up-an-smtp-server}

## 概述{#overview}

**什么是SMTP服务器？**

**简**&#x200B;单 ****&#x200B;邮 ****&#x200B;件传 ****&#x200B;输协议，这是负责发送出站邮件的服务器。当您从电子邮件客户端发送电子邮件时，您使用的是同一服务来发送电子邮件。

**为什么要使用Sales Connect设置SMTP服务器？**

它允许您利用公司所在域的声誉和交付能力，并且不必依赖他人。 我们的默认MSC服务器是共享IP池的一部分，这意味着从共享信誉发送。 我们强烈建议您的团队使用Sales Connect设置自己的投放渠道。

**Sales Connect如何与我的SMTP服务器一起发送？**

通过执行[这些步骤](http://docs.marketo.com/x/ZgPh)。

![](assets/1.png)

`<pre><em>SMTP Server Setup Page in Sales Connect</em><br> </pre>` **是否需要在我的电子邮件客户端中设置任何内容？**

就投放渠道而言，不。 安装我们的插件后，Sales Connect将利用您为发送电子邮件设置的相同投放渠道。

## 获取SMTP凭据{#getting-the-smtp-credentials}

**如何获取SMTP凭据？**

联系您的IT团队，了解公司用什么投放渠道发送电子邮件以及如何访问您的SMTP凭据。 根据服务器的配置方式，SMTP服务器名称或服务器端口可能具有一些自定义值。 如果您没有专门的IT团队，请联系您的电子邮件提供商。

**如果我的公司使用Office365，我有哪些选择？**

专业人员

* 易于设置
* 具有Office365帐户的任何用户都可以访问此SMTP服务器

图标

* 可能发生限制
* 每个用户必须自行设置
* 更改用户的O365密码将导致连接断开

如果您使用Office365或Exchange Online，则可以使用一组标准凭据连接到SMTP服务器。 请记住，Office365不是批量电子邮件投放服务，但对于发送一次性电子邮件将非常有效。 发送批量电子邮件时，Office365可能会限制您的电子邮件，这可能导致投放失败。 要进一步了解此信息，请查看Microsoft有关如何设置SMTP客户端提交的](http://support.office.com/en-us/article/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-365-69f58e99-c550-4274-ad18-c805d654b4c4)的文章。[

“您只能从一个电子邮件地址发送，除非您的设备可以存储多个Office 365邮箱的登录凭据。 Office 365限制每分钟发送30封邮件，限制每天发送1万收件人。”

如果您决定使用Office365作为投放渠道，则需要输入这些凭据。 团队中不能使用相同的凭据，因为Office365使用用户的电子邮件和密码进行连接。

Microsoft和批量发送

[单](https://technet.microsoft.com/en-us/library/exchange-online-limits.aspx#RecipientLimits) 击此处了解在Office365中批量发送。

需要发送合法批量商业电子邮件（例如，客户新闻稿）的Exchange Online客户应使用专门提供这些服务的第三方提供商。”

**如果我的公司使用Gmail呢？**

如果您的团队希望将Gmail用作Sales Connect的投放渠道，则无需获取任何SMTP凭据。 Sales Connect允许用户通过我们的OAuth集成访问其Gmail投放渠道。 用户可以通过将其Sales Connect帐户与Gmail集成来启用此功能。

![](assets/2.png)

**能否与整个团队共享相同的SMTP凭据？**

这取决于您使用的投放渠道。 例如，Sparkpost等服务允许凭据基于域，因此使用特定域发送的任何人都将通过身份验证通过该服务器发送。 如果是，则可以与团队共享凭据。

如果您正在连接到Office365，则凭据是基于电子邮件地址的。 这意味着只有建立连接的电子邮件地址才会通过身份验证通过该投放渠道发送电子邮件，因此凭据应&#x200B;**不**&#x200B;被共享。

![](assets/3.png)

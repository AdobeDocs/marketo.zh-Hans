---
unique-page-id: 4720710
description: 为电子邮件可投放性设置SPF和DKIM - Marketo文档 — 产品文档
title: 为电子邮件投放能力设置SPF和DKIM
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 为电子邮件投放能力设置SPF和DKIM {#set-up-spf-and-dkim-for-your-email-deliverability}

提高电子邮件投放率的一种快速方法是，将&#x200B;**SPF**（发件人策略框架）和&#x200B;**DKIM**（域名标识邮件）合并到您的DNS设置中。 除了DNS条目之外，您还告诉收件人您已授权Marketo代表您发送电子邮件。 如果没有此更改，则由于电子邮件是从您的域发送，但是是从具有Marketo域的IP地址发送，因此您的电子邮件更有可能被标记为垃圾邮件。

>[!CAUTION]
>
>您需要网络管理员在DNS记录中进行此更改。

## 设置SPF {#set-up-spf}

**如果您的域中没有SPF记录**

请要求网络管理员将以下行添加到您的DNS条目。 将[domain]替换为您网站的主域(例如， “company.com”)和[corpIP]，其中包含您公司电子邮件服务器的IP地址(例如 “255.255.255.255”)。 如果您通过Marketo从多个域发送电子邮件，则应将其添加到每个域（在一行上）。

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**如果您的域上有SPF记录**

如果DNS条目中已有SPF记录，请在其中添加以下内容：

include:mktomail.com

## 设置DKIM {#set-up-dkim}

**什么是DKIM?为什么要设置DKIM?**

DKIM是一种身份验证协议，电子邮件接收者使用该协议来确定电子邮件是否是由声称是由谁发送的。 DKIM通常会提高电子邮件到收件箱的投放能力，因为接收者可以确信该邮件不是伪造的。

**DKIM是如何工作的？**

在您的DNS记录中设置公钥并在“管理员”部分(A)中激活发送域后，我们将为您的传出消息启用自定义DKIM签名，该签名将包含一个加密的数字签名，其中包含我们为您发送的每封电子邮件(B)。 接收器将能够通过在发送域的DNS(C)中查找“公钥”来解密数字签名。 如果电子邮件中的键值与DNS记录中的键值相对应，则接收邮件服务器将更有可能接受代表您发送的电子邮件Marketo。

![](assets/image2015-1-12-13-3a56-3a55.png)

**如何设置DKIM?**

请参阅[设置自定义DKIM签名](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)。

>[!MORELIKETHIS]
>
>* [进一步了解SPF及其工作方式](http://www.open-spf.org/Introduction/)
>* [Marketo的电子邮件投放工具](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [我的SPF设置正确吗？](https://www.kitterman.com/spf/validate.html)
>* [我使用了正确的语法吗？](https://www.open-spf.org/SPF_Record_Syntax/)


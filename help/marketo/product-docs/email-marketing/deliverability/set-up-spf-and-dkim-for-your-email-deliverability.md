---
unique-page-id: 4720710
description: 为电子邮件发送功能设置SPF和DKIM - Marketo文档——产品文档
title: 设置SPF和DKIM以便您的电子邮件发送
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---


# 设置SPF和DKIM以便您的电子邮件发送 {#set-up-spf-and-dkim-for-your-email-deliverability}

提高电子邮件投放率的一种快速方法是 **将SPF** （发送者策略框架）和 **DKIM** （识别的域密钥邮件）合并到DNS设置中。 通过添加此DNS条目，您告诉收件人您已授权Market代表您发送电子邮件。 如果没有此更改，则由于电子邮件是从您的域发送的，但是从具有Marketo域的IP地址发送的，因此您的电子邮件被标记为垃圾邮件的可能性更高。

>[!CAUTION]
>
>您需要网络管理员在DNS记录中进行此更改。

## 设置SPF {#set-up-spf}

**如果域中没有SPF记录**

请让网络管理员向DNS条目中添加以下行。 将 [域] 替换为网站的主域(例如 “公司.com”)和 [corpIP] (含您的公司电子邮件服务器(例如 &quot;255.255.255.255&quot;). 如果您通过Marketo从多个域发送电子邮件，则应将此电子邮件添加到每个域（在一行上）。
[域] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all\
如果您的域上确实有SPF记录

如果您的DNS条目中已有SPF记录，请在其中添加以下内容：

include:mktomail.com

## 设置DKIM {#set-up-dkim}

### 什么是DKIM? 我为什么要设立DKIM? {#what-is-dkim-why-do-i-want-to-set-up-dkim}

DKIM是一种身份验证协议，电子邮件接收者使用它来确定电子邮件是否是由其声称其发送者发送的。 DKIM通常会提高电子邮件发送到收件箱的能力，因为接收者可以确信该邮件不是伪造的。

DKIM是如何工作的？

在您在DNS记录中设置公钥并在“管理”部分(A)激活发送域后，我们将为您的传出消息启用自定义DKIM签名，其中将包括加密数字签名，以及我们为您发送的每封电子邮件(B)。 接收方将能够通过查找发送域的DNS(C)中的“公钥”来解密数字签名。 如果电子邮件中的密钥与DNS记录中的密钥相对应，则接收邮件服务器更有可能接受代表您发送的电子邮件营销人员。

![](assets/image2015-1-12-13-3a56-3a55.png)

如何设置DKIM?

请参阅 [设置自定义DKIM签名](set-up-a-custom-dkim-signature.md)。

>[!MORELIKETHIS]
>
>* [进一步了解SPF及其工作方式](http://www.open-spf.org/Introduction/)
>* [Marketo的电子邮件发送工具](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [我的SPF设置正确吗？](http://www.kitterman.com/spf/validate.html)
>* [我使用正确的语法了吗？](http://www.open-spf.org/SPF_Record_Syntax/)

>




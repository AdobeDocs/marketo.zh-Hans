---
unique-page-id: 4720710
description: 为提高电子邮件送达率设置 SPF 和 DKIM — Marketo 文档 — 产品文档
title: 为提高电子邮件送达率设置 SPF 和 DKIM
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '421'
ht-degree: 100%

---

# 为提高电子邮件送达率设置 SPF 和 DKIM {#set-up-spf-and-dkim-for-your-email-deliverability}

提高电子邮件送达率的一种快捷方法，是在 DNS 设置中加入 **SPF**（Sender Policy Framework，发件人策略框架）和 **DKIM**（Domain Keys Identified Mail，域名密钥识别电子邮件）。通过在 DNS 记录中添加这些配置，您是在向收件方表明：您已授权 Marketo 代表您发送电子邮件。如果未进行此项配置，由于电子邮件显示来自您的域名，但实际是从 Marketo 域名的 IP 地址发送，电子邮件更容易被标记为垃圾电子邮件。

>[!CAUTION]
>
>您需要联系网络管理员，在 DNS 记录中完成此项更改。

## 设置 SPF {#set-up-spf}

**如果您的域名尚未配置 SPF 记录**

请让您的网络管理员在 DNS 记录中添加以下内容。请将[域]替换为您网站的主域名（例如“company.com”），并将 [corpIP] 替换为公司电子邮件服务器的 IP 地址（例如“255.255.255.255”）。如果您通过 Marketo 从多个域名发送电子邮件，则需要为每个域名分别添加此记录（每个域名一行）。

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**如果您的域名已经配置了 SPF 记录**

如果您的 DNS 记录中已存在 SPF 记录，请在其中添加以下内容：

include:mktomail.com

## 设置 DKIM {#set-up-dkim}

**什么是 DKIM？为什么要设置 DKIM？**

DKIM 是一种身份验证协议，供电子邮件接收方用来判断电子邮件是否确实由其声明的发件人发送。由于接收方能够确认电子邮件并非伪造，DKIM 通常可以提升电子邮件成功投递到收件箱的概率。

**DKIM 是如何工作的？**

在您在 DNS 记录中设置公钥，并在“管理员”区域中激活发送域名（A）后，我们将为您的外发电子邮件启用自定义 DKIM 签名。此后，我们代您发送的每封电子邮件都会包含一个加密的数字签名（B）。电子邮件接收方可以通过在发送域名的 DNS 中查找“公钥”来解密该数字签名（C）。如果电子邮件中的密钥与 DNS 记录中的密钥一致，接收电子邮件服务器将更有可能接受 Marketo 代表您发送的电子邮件。

![](assets/image2015-1-12-13-3a56-3a55.png)

**如何设置 DKIM？**

请参阅[设置自定义 DKIM 签名](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}。

>[!MORELIKETHIS]
>
>* 详细了解 SPF 及其工作原理`: http://www.open-spf.org/Introduction/`
>* 我的 SPF 是否配置正确？：`https://www.kitterman.com/spf/validate.html`
>* 我是否使用了正确的语法？：`http://www.open-spf.org/SPF_Record_Syntax/`

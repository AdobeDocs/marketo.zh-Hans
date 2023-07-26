---
unique-page-id: 4720710
description: 为您的电子邮件可投放性设置SPF和DKIM - Marketo文档 — 产品文档
title: 为您的电子邮件可投放性设置SPF和DKIM
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# 为您的电子邮件可投放性设置SPF和DKIM {#set-up-spf-and-dkim-for-your-email-deliverability}

提高电子邮件投放率的一种快速方法是纳入 **SPF** （发件人策略框架）和 **DKIM** （域密钥识别邮件）放入您的DNS设置中。 除了DNS条目之外，您还可以告诉收件人，您已授权Marketo代表您发送电子邮件。 如果没有此更改，则电子邮件被标记为垃圾邮件的可能性会更高，因为电子邮件是从您的域发送的，但却是从具有Marketo域的IP地址发送的。

>[!CAUTION]
>
>您需要网络管理员才能在DNS记录中进行此更改。

## 设置SPF {#set-up-spf}

**如果您的域中没有SPF记录**

要求网络管理员将以下行添加到您的DNS条目。 替换 [域] 包含网站的主域(例如， “company.com”)和 [corpIP] 与企业电子邮件服务器的IP地址一起使用(例如 &quot;255.255.255.255&quot;). 如果您通过Marketo从多个域发送电子邮件，则应将其添加到每个域（在一行中）。

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**如果您的域中确实有SPF记录**

如果您的DNS条目中已有SPF记录，请添加以下内容：

include：mktomail.com

## 设置DKIM {#set-up-dkim}

**什么是DKIM？ 为什么要设置DKIM？**

DKIM是一种身份验证协议，电子邮件接收者使用它来确定电子邮件是否由发送者发送。 DKIM通常可提高将电子邮件传递到收件箱的能力，因为收件人可以确信该消息不是伪造的。

**DKIM的工作原理**

在您在DNS记录中设置公钥并在Admin部分激活发送域后(A)，我们将为传出邮件启用自定义DKIM签名，其中包括我们发送给您的每封电子邮件的加密数字签名(B)。 接收者将通过在发送域的DNS (C)中查找“公钥”来解密数字签名。 如果电子邮件中的密钥与您DNS记录中的密钥相对应，则接收邮件服务器将更有可能接受代表您发送的Marketo电子邮件。

![](assets/image2015-1-12-13-3a56-3a55.png)

**如何设置DKIM？**

请参阅 [设置自定义DKIM签名](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [详细了解SPF及其工作方式](http://www.open-spf.org/Introduction/){target="_blank"}
>* [我的SPF设置是否正确？](https://www.kitterman.com/spf/validate.html){target="_blank"}
>* [我是否使用了正确的语法？](http://www.open-spf.org/SPF_Record_Syntax/){target="_blank"}

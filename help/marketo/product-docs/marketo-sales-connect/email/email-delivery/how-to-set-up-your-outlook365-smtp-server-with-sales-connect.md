---
unique-page-id: 14352600
description: 如何使用Sales Connect设置Outlook365 SMTP服务器- Marketo文档——产品文档
title: 如何通过Sales Connect设置Outlook365 SMTP服务器
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# 如何通过Sales Connect设置Outlook365 SMTP服务器 {#how-to-set-up-your-outlook-smtp-server-with-sales-connect}

>[!NOTE]
>
>如果您的组织使用Outlook，而您正尝试使用Marketo Sales Connect设置电子邮件投放渠道，我们建议使用我们的电子邮件连接功能 [连接到您的Exchange服务器](http://docs.marketo.com/x/Z4AOAQ)。

为了将自定义SMTP服 [务器设置](http://docs.marketo.com/x/zYTS) 为替代投放渠道,ToutApp确实要求您出于安全目的而使用某种形式的身份验证。 可以在SMTP配置页上设置任何 [SMTP服务器](http://toutapp.com/next#settings/email-servers/smtp/configure)。 要设置Office365 SMTP服务器，Microsoft建议进行以下配置：\
**SMTP服务器**:smtp.office365.com\
**服务器端口**:端口587 —— 安全\
**身份验证方法**:登录(SSL/TLS)\
**用户名或登录**:您的Office365电子邮件地址\
**密码**:您的Office365电子邮件密码\
**您的域**:你的公司

如果设置SMTP服务器时仍出现问题，请与Exchange管理员合作，确保使用正确的凭据。

>[!NOTE]
>
>通过Office365 SMTP发送时，Microsoft `limit of 30 messages sent per minute`规定每天最多10,000收件人。 此外， `each member` 希望通过Office365 SMTP服务器发送电子邮件的团队需要在其Sales Connect设置中使用自己的电子邮件地址和密码设置此设置。 根据Microsoft的Office365帐 `Make this deliverability channel to all my team members` 户策略， `" will not work` 选中此配置的设置“”的复选框。


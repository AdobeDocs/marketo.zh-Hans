---
unique-page-id: 4720433
description: 配置Marketo协议- Marketo文档——产品文档
title: 为Marketo配置协议
translation-type: tm+mt
source-git-commit: 0ec525defbefe610f0bd1227b1c8f8e125d8e362
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 1%

---


# 为Marketo配置协议 {#configure-protocols-for-marketo}

您的营销团队正在使用Market创建品牌化的活动登陆页和电子邮件。 为确保这些登陆页和电子邮件能够正常工作，他们需要IT人员提供一些帮助。 请设置以下协议，其中包含您的营销组应通过电子邮件发送给您的信息。

本条应与希望执行这些议定书的公司的IT部门分享。

>[!NOTE]
>
>如果您的IT团队使用程序限制允许列表Web访问，请要求他们添加以下域（包括星号）以允许所有Marketo资源和Web套接字：

* `*.marketo.com`

* `*.marketodesigner.com`

* `*.mktoweb.com`

## 第1步：为登陆页和电子邮件创建DNS记录 {#step-create-dns-records-for-landing-pages-and-email}

**跟踪链接CNAME**

您的营销团队应已向您发送两个请求，请求获得新的CNAME记录。 第一种是登陆页URL，这样登陆页就会显示在反映您的域的URL中，而不是Marketo（实际主机）中。 第二种是跟踪链接，这些链接包含在他们从Marketo发送的电子邮件中。

`1` **为登陆页添加CNAME**

添加他们将您发送给您的登陆页CNAME到您的DNS记录， `[YourLandingPageCNAME]` 以便指向分配给您的Marketo登陆页的唯一帐户字符串。 登录到您的域注册机站点并输入登陆页CNAME和帐户字符串。 通常，这涉及三个字段：

* 别名：输入( `[YourLandingPageCNAME]` 由营销提供)
* 类型：CNAME
* 指向：输入( `[MarketoAccountString].mktoweb.com` 由营销提供)

`2` **为电子邮件跟踪链接添加CNAME**

添加您发送的电子邮件CNAME营销，以 `[YourEmailCNAME]` 便以 [下格式指向MktoTracking]Link（Marketto分配的默认跟踪链接）:\
`[YourEmailCNAME].[YourDomain].com` 在CNAME中 `[MktoTrackingLink]`

例如：

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **通知您的营销团队**

完成此过程后，通知您的营销团队。

## 第2步：允许列表营销IP {#step-allowlist-marketo-ips}

当您的营销组使用Market发送测试电子邮件（在发出电子邮件爆炸之前的最佳实践）时，测试电子邮件有时会被依赖发件人IP地址来验证电子邮件有效的反垃圾邮件系统阻止。 要确保这些测试电子邮件送达，请将Market添加到您的允许列表。

将以下IP地址添加到您的公允许列表司：

199.15.212.0/22\
192.28.144.0/20
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

某些防垃圾邮件系统使用电子邮件返回路径字段而不是IP地址进行分配。 在这些情况下，最好的方允许列表法是“*.mktomail.com”，因为Marketo使用多个邮箱子域。 其他反垃圾邮件系允许列表统基于发件人地址进行。 在这些情况下，请务必包含您的营销组用来与人／潜在客户进行通信的所有发送（“发件人”）域。

>[!NOTE]
>
>Postini采用独特的技术，并需列入允许列表要IP范围。 请参 [列入允许列表阅与Postini](https://nation.marketo.com/docs/DOC-1066)。

## 第3步：设置SPF和DKIM {#step-set-up-spf-and-dkim}

您的营销团队还应向您发送要添加到DNS资源记录的DKIM信息（也如下所示）。 按照以下步骤成功配置DKIM和SPF，然后通知您的营销团队此更新。

1. 要设置SPF，请在DNS条目中添加以下行：

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   包括：mktomail.com ~all

   如果我们的DNS条目中已有SPF记录，只需在其中添加以下内容：\
   包括：mktomail.com

   将CompanyDomain替换为网站的主域(例如：“`(company.com/)`”)和CorpIP，其IP地址为您的公司电子邮件服务器(例如 &quot;255.255.255.255&quot;). 如果您要通过Marketo从多个域发送电子邮件，您应让IT人员为每个域添加此行（在一行中）。

1. 对于DKIM，为要设置的每个域创建DNS资源记录。 以下是我们将为每个域签名的主机记录和TXT值：

   `[DKIMDomain1]`:主机记录 `[HostRecord1]` 为，TXT值为 `[TXTValue1]`。

   `[DKIMDomain2]`:主机记录 `[HostRecord2]` 为，TXT值为 `[TXTValue2]`。

   按照此处的说明，复制您设置的每个DKIMDomain的HostRecord和 [TXTValue](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)。 在您的IT人员完成此步骤后，不要忘记在“管理员”>“电子邮件”>“DKIM”中验证每个域。

## 第4步：为域设置MX记录 {#step-set-up-mx-records-for-your-domain}

MX记录允许您接收来自您发送电子邮件的域的邮件，以处理回复和自动回复。 如果从公司域发送，您可能已配置了此配置。 如果没有，您通常可以设置它以映射到您公司域的MX记录。

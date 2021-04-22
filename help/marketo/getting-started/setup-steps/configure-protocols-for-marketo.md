---
unique-page-id: 4720433
description: 为Marketo配置协议 — Marketo文档 — 产品文档
title: 为Marketo配置协议
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 1%

---

# 为Marketo {#configure-protocols-for-marketo}配置协议

您的营销团队正在使用Marketo创建品牌化活动登陆页和电子邮件。 为确保这些登陆页和电子邮件正常工作，他们需要IT部门的一些帮助。 请设置以下协议，其中包含您的营销组应已通过电子邮件向您发送的信息。

本条应与希望执行这些议定书的公司的IT部门分享。

>[!NOTE]
>
>如果您的IT团队使用程序限制允许列表Web访问，请要求他们添加以下域（包括星号）以允许所有Marketo资源和Web套接字：

* `*.marketo.com`

* `*.marketodesigner.com`

* `*.mktoweb.com`

## 第1步：为登陆页和电子邮件创建DNS记录{#step-create-dns-records-for-landing-pages-and-email}

**跟踪链接CNAME**

您的营销团队应已向您发送了两个请求以获取新CNAME记录。 第一种是登陆页URL，这样登陆页就会显示在反映您的域的URL中，而不是Marketo（实际主机）中。 第二种是跟踪链接，这些链接包含在他们从Marketo发送的电子邮件中。

`1` **为登陆页添加CNAME**

添加他们发送给您的DNS记录的登陆页CNAME，以便`[YourLandingPageCNAME]`指向分配给您的Marketo登陆页的唯一帐户字符串。 登录到域注册机的站点并输入登陆页CNAME和帐户字符串。 通常，这涉及三个字段：

* 别名：输入`[YourLandingPageCNAME]`（由营销提供）
* 类型：CNAME
* 指向：输入`[MarketoAccountString].mktoweb.com`（由营销提供）

`2` **为电子邮件跟踪链接添加CNAME**

添加您发送的电子邮件CNAME营销，以便`[YourEmailCNAME]`指向[MktoTrackingLink](Marketo分配的默认跟踪链接)，格式为：\
`[YourEmailCNAME].[YourDomain].com` 在CNAME中  `[MktoTrackingLink]`

例如：

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **通知您的营销团队**

完成此过程后，通知您的营销团队。

## 第2步：允许列表Marketo IP {#step-allowlist-marketo-ips}

当您的营销组使用Marketo发送测试电子邮件（在发出电子邮件群发之前的最佳实践）时，测试电子邮件有时会被依赖发件人IP地址验证电子邮件有效的反垃圾邮件系统阻止。 要确保这些测试电子邮件送达，请将Marketo添加到您的允许列表。

将以下IP地址添加到您的企允许列表业：

199.15.212.0/22\
192.28.144.0/20
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

某些防垃圾邮件系统会使用电子邮件返回路径字段而不是分配的IP地址。 在这些情况下，最佳方允许列表法是“*.mktomail.com”，因为Marketo使用多个邮箱子域。 其他防垃圾邮件系允许列表统基于发件人地址进行。 在这些情况下，请务必包括您的营销组用来与人/潜在客户通信的所有发送（“发件人”）域。

>[!NOTE]
>
>Postini采用独特的技术，需要列入允许列表的IP范围。 请参阅[列入允许列表使用Postini](https://nation.marketo.com/docs/DOC-1066)进行。

## 第3步：设置SPF和DKIM {#step-set-up-spf-and-dkim}

您的营销团队还应向您发送要添加到您的DNS资源记录的DKIM信息（也如下所示）。 请按照以下步骤成功配置DKIM和SPF，然后通知您的营销团队已更新此更新。

1. 要设置SPF，请在DNS条目中添加以下行：

   `[CompanyDomain]` 在TXT v=spf1 mx ip4中：`[CorpIP]`\
   包括：mktomail.com ~all

   如果我们的DNS条目中已有SPF记录，只需在其中添加以下内容：\
   包括：mktomail.com

   将CompanyDomain替换为网站的主域(例如：“`(company.com/)`”)和CorpIP，其IP地址为您的公司电子邮件服务器(例如 255.255.255.255&quot;)。 如果您要通过Marketo从多个域发送电子邮件，您应让IT人员为每个域添加此行（在一行中）。

1. 对于DKIM，为要设置的每个域创建DNS资源记录。 以下是我们将要签名的每个域的主机记录和TXT值：

   `[DKIMDomain1]`:主机记 `[HostRecord1]` 录为，TXT值为 `[TXTValue1]`。

   `[DKIMDomain2]`:主机记 `[HostRecord2]` 录为，TXT值为 `[TXTValue2]`。

   按照[此处](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)的说明，复制您设置的每个DKIMDomain的HostRecord和TXTValue。 在您的IT员工完成此步骤后，不要忘记在“管理员”>“电子邮件”>“DKIM”中验证每个域。

## 第4步：设置域{#step-set-up-mx-records-for-your-domain}的MX记录

MX记录允许您接收来自您发送电子邮件的域的邮件，以处理回复和自动回复。 如果从公司域发送，您可能已经配置了此配置。 如果没有，您通常可以设置它以映射到公司域的MX记录。

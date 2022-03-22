---
unique-page-id: 4720433
description: 为Marketo配置协议 — Marketo文档 — 产品文档
title: 配置Marketo协议
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
source-git-commit: abfd29468bee24644353df497e1f80e0c05b6b2f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 配置Marketo协议 {#configure-protocols-for-marketo}

如果您或您的组织使用受限的防火墙或代理服务器设置，则您或您的网络管理员可能需要允许列表某些域和IP地址范围，以确保Adobe Marketo Engage按预期运行。

## 品牌营销活动登陆页面和电子邮件 {#branded-campaign-landing-pages-and-emails}

您的营销团队正在使用Marketo创建品牌化的营销活动登陆页面和电子邮件。 要确保这些登陆页面和电子邮件正常工作，他们需要IT团队提供一些帮助。 请设置以下协议，其中包含您的营销组应通过电子邮件向您发送的信息。

本文应与希望实施这些协议的公司IT部门分享。

>[!NOTE]
>
>如果您的IT团队使用限制Web访问允许列表，请要求他们添加以下域（包括星号）以允许使用所有Marketo资源和Web套接字：

* `*.marketo.com`

* `*.marketodesigner.com`

* `*.mktoweb.com`

## 步骤1:为登陆页面和电子邮件创建DNS记录 {#step-create-dns-records-for-landing-pages-and-email}

**跟踪链接CNAME**

您的营销团队应已向您发送了两个请求，以获取新的CNAME记录。 第一个是登陆页面URL，以便登陆页面显示在反映您的域而非Marketo（实际主机）的URL中。 第二个是用于跟踪链接，这些链接包含在从Marketo发送的电子邮件中。

`1` **为登陆页面添加CNAME**

将登陆页面CNAME添加到他们将您发送到DNS记录，以便 `[YourLandingPageCNAME]` 指向分配给您的Marketo登陆页面的唯一帐户字符串。 登录到您的域注册机构的网站，然后输入登陆页面CNAME和帐户字符串。 通常，这涉及三个字段：

* 别名：输入 `[YourLandingPageCNAME]` （由营销提供）
* 类型：CNAME
* 指向：输入 `[MarketoAccountString].mktoweb.com` （由营销提供）

`2` **为电子邮件跟踪链接添加CNAME**

添加您发送的电子邮件CNAME营销，以便 `[YourEmailCNAME]` 指向 [MktoTrackingLink],Marketo分配的默认跟踪链接，格式为：\
`[YourEmailCNAME].[YourDomain].com` 在CNAME中 `[MktoTrackingLink]`

例如：

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **通知您的营销团队**

完成此过程后，通知您的营销团队。

## 步骤2:允许列表Marketo IP {#step-allowlist-marketo-ips}

当您的营销组使用Marketo发送测试电子邮件（发出电子邮件爆炸声之前的最佳实践）时，测试电子邮件有时会被依赖发件人IP地址来验证电子邮件是否有效的防垃圾邮件系统阻止。 要确保这些测试电子邮件送达，请将Marketo添加到您的允许列表。

将这些IP地址添加到您的公司允许列表:

199.15.212.0/22\
192.28.144.0/20 192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

某些防垃圾邮件系统使用电子邮件返回路径字段而不是IP地址进行分配。 在这些情况下，最佳方法是允许列表“*.mktomail.com”，因为Marketo使用多个邮箱子域。 其他反垃圾邮件系统允许列表基于“发件人”地址进行。 在这些情况下，请确保包含营销组用于与人员/潜在客户通信的所有发送（“发件人”）域。

>[!NOTE]
>
>Postini采用一种独特的技术，需要列入允许列表的IP范围。 请参阅 [使列入允许列表用Postini](https://nation.marketo.com/docs/DOC-1066).

## 步骤3:设置SPF和DKIM {#step-set-up-spf-and-dkim}

您的营销团队还应向您发送要添加到DNS资源记录的DKIM信息（如下所示）。 按照步骤成功配置DKIM和SPF，然后通知您的营销团队此信息已更新。

1. 要设置SPF，请将以下行添加到DNS条目中：

   `[CompanyDomain]` 在TXT v=spf1 mx ip4中：`[CorpIP]`\
   包括：mktomail.com ~all

   如果DNS条目中已有SPF记录，只需在其中添加以下内容：\
   包括：mktomail.com

   将CompanyDomain替换为您网站的主域(例如：&quot;`(company.com/)`“)和CorpIP ，其IP地址为您的公司电子邮件服务器(例如 “255.255.255.255”)。 如果您要通过Marketo从多个域发送电子邮件，则应让IT员工为每个域添加此行（在一行中）。

1. 对于DKIM，请为要设置的每个域创建DNS资源记录。 下面是我们将为其签名的每个域的主机记录和TXT值：

   `[DKIMDomain1]`:主机记录为 `[HostRecord1]` 和TXT值为 `[TXTValue1]`.

   `[DKIMDomain2]`:主机记录为 `[HostRecord2]` 和TXT值为 `[TXTValue2]`.

   复制您在 [此处说明](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). 在您的IT员工完成此步骤后，请不要忘记在管理员>电子邮件> DKIM中验证每个域。

## 步骤4:为域设置MX记录 {#step-set-up-mx-records-for-your-domain}

MX记录允许您接收来自的域的邮件，以处理回复和自动应答器。 如果您从公司域发送，则可能已经配置了此设置。 如果没有，您通常可以设置它以映射到您公司域的MX记录。

## 出站IP地址 {#outbound-ip-addresses}

叫客连接是指代表您Marketo Engage到Internet上的服务器的连接。 您与之合作的某些合作伙伴/供应商或您自己的IT组织可能会使用允许列表来限制对服务器的访问。 如果是，则必须向他们提供Marketo Engage出站IP地址块以添加到其允许列表。

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target=&quot;_blank&quot;}是出站集成机制。 当 [调用Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target=&quot;_blank&quot;}流操作作为智能营销活动的一部分执行，将向外部Web服务发出HTTP请求。 如果Web服务发布者在外允许列表部Web服务所在网络的防火墙上使用，则发布者必须将下面列出的IP地址块添加到其中允许列表。

**CRM同步**

Marketo Engage [Salesforce CRM同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target=&quot;_blank&quot;}和 [Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target=&quot;_blank&quot;}是对CRM供应商发布的API发出出站HTTP请求的集成机制。 您必须确保IT组织不会阻止下面的任何IP地址块访问您的CRM供应商API。

**Marketo Engage出站IP地址块**

下表涵盖进行出站调用的所有Marketo Engage服务器。 如果要配置任何IP、服务器、防火墙、访问控允许列表制列表、安全组或第三方服务以从Marketo Engage接收传出连接，则使用此列表。

<table>
 <tbody>
  <tr>
   <th>IP块（CIDR表示法）</th>
  </tr>
  <tr>
   <td>192.28.144.0/20</td>
  </tr>
   <tr>
   <td>192.28.160.0/19</td>
  </tr>
   <tr>
   <td>199.15.212.0/22</td>
  </tr>
 </tbody>
</table>

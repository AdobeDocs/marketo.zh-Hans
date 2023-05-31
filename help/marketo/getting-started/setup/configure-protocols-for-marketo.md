---
unique-page-id: 4720433
description: 为Marketo配置协议 — Marketo文档 — 产品文档
title: 为Marketo配置协议
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
source-git-commit: 5a8fe88dec5f2bf9c94c0a08a5515b87bc6dcaa9
workflow-type: tm+mt
source-wordcount: '1024'
ht-degree: 3%

---

# 为Marketo配置协议 {#configure-protocols-for-marketo}

允许列表如果您或您的组织使用限制性的防火墙或代理服务器设置，则您或您的网络管理员可能需要某些域和IP地址范围，以确保Adobe Marketo Engage按预期工作。

## 品牌营销活动登陆页面和电子邮件 {#branded-campaign-landing-pages-and-emails}

您的营销团队正在使用Marketo创建品牌营销活动登陆页和电子邮件。 为确保这些登陆页面和电子邮件正常工作，他们需要IT部门提供一些帮助。 请设置以下协议，并提供您的营销组应通过电子邮件发送给您的信息。

本文应与希望实施这些协议的公司的IT部门共享。

允许列表如果您的IT团队使用限制Web访问，请让他们添加以下域（包括星号）以允许所有Marketo资源和Web套接字：

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`

## 步骤1：为登陆页面和电子邮件创建DNS记录 {#step-create-dns-records-for-landing-pages-and-email}

**跟踪链接CNAME**

您的营销团队应该向您发送两个新CNAME记录请求。 第一个是用于登陆页面URL，以便登陆页面显示在反映您的域而不是Marketo（实际的主机）的URL中。 第二个用于跟踪他们从Marketo发送的电子邮件中包含的链接。

`1` **为登陆页面添加CNAME**

添加他们发送给您的DNS记录的登陆页面CNAME，以便 `[YourLandingPageCNAME]` 指向分配给Marketo登陆页面的唯一帐户字符串。 登录到域注册器的网站，然后输入登陆页面CNAME和帐户字符串。 通常，这涉及三个字段：

* 别名：输入 `[YourLandingPageCNAME]` （营销提供）
* 类型：CNAME
* 指向：输入 `[MunchkinID].mktoweb.com` （营销提供）

`2` **为电子邮件跟踪链接添加CNAME**

添加营销人员发送给您的电子邮件CNAME，以便 `[YourEmailCNAME]` 指向 [MktoTrackingLink]，Marketo分配的默认跟踪链接，格式为：\
`[YourEmailCNAME].[YourDomain].com` 在CNAME中 `[MktoTrackingLink]`

例如：

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` 必须是默认品牌策略域。

`3` **通知您的营销团队**

完成此流程后，请通知您的营销团队。

`4` **联系人 [Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} 开始配置SSL证书的过程。**

完成此过程最多可能需要3个工作日。

## 步骤2：允许列表Marketo IP {#step-allowlist-marketo-ips}

当您的营销团队使用Marketo发送测试电子邮件（发送电子邮件冲击之前的最佳实践）时，测试电子邮件有时会被反垃圾邮件系统阻止，这些系统依赖发件人IP地址来验证电子邮件是否有效。 要确保收到这些测试电子邮件，请将Marketo添加到您的允许列表。

将这些IP地址添加到您的公司允许列表：

94.236.119.0/26

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

某些反垃圾邮件系统使用电子邮件返回路径字段而不是IP地址进行分配。 在这些情况下，最好的方法是允许列表&#39;&#42;.mktomail.com&#39;，因为Marketo使用多个邮箱子域。 其他反垃圾邮件系统则根据发件人地址进行允许列表。 在这些情况下，请确保包括营销组用于与人员/潜在客户通信的所有发送（“发件人”）域。

>[!NOTE]
>
>Postini采用独特的技术，并要求IP范围列入允许列表。 参见 [使用Postini进行列入允许列表](https://nation.marketo.com/docs/DOC-1066).

## 步骤3：设置SPF和DKIM {#step-set-up-spf-and-dkim}

您的营销团队还应向您发送DKIM信息，以添加到DNS资源记录（也列于下方）。 按照步骤成功配置DKIM和SPF，然后通知您的营销团队该配置已更新。

1. 要设置SPF，请将以下行添加到我们的DNS条目中：

   `[CompanyDomain]` 在TXT中v=spf1 mx ip4：`[CorpIP]`\
   包括： mktomail.com ~all

   如果我们的DNS条目中已有SPF记录，只需将以下内容添加到其中：\
   包括： mktomail.com

   将CompanyDomain替换为您的网站的主域(例如： ”`(company.com/)`“)和CorpIP ，以及您的公司电子邮件服务器的IP地址(例如， &quot;255.255.255.255&quot;). 如果您要通过Marketo从多个域发送电子邮件，则应让IT员工为每个域添加此行（在一行中）。

1. 对于DKIM，请为我们要设置的每个域创建DNS资源记录。 下面是我们要签名的每个域的主机记录和TXT值：

   `[DKIMDomain1]`：主机记录为 `[HostRecord1]` 并且TXT值为 `[TXTValue1]`.

   `[DKIMDomain2]`：主机记录为 `[HostRecord2]` 并且TXT值为 `[TXTValue2]`.

   在执行以下操作后，为已设置的每个DKIMDomain复制HostRecord和TXTValue [此处说明](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. 在您的IT员工完成此步骤后，请不要忘记在“管理员”>“电子邮件”>“DKIM”中验证每个域。

## 步骤4：为您的域设置MX记录 {#step-set-up-mx-records-for-your-domain}

通过MX记录，可接收发往您发送电子邮件的域的邮件，以处理回复和自动回复者。 如果您从公司域发送，则可能已配置此项。 如果不能，则通常可以将其设置为映射到企业域的MX记录。

## 出站IP地址 {#outbound-ip-addresses}

出站连接是指Marketo Engage代表您通过Internet与Server建立的连接。 允许列表与您合作的一些合作伙伴/供应商或您自己的IT部门可能会使用来限制对服务器的访问。 如果是，则必须向他们提供Marketo Engage允许列表出站IP地址块，以将其添加到其中。

**Webhook**

Marketo Engage [Webhook](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} 流程操作作为智能营销活动的一部分执行，会向外部Web服务发出HTTP请求。 允许列表 允许列表如果Web服务发布者在外部Web服务所在网络的防火墙上使用，则发布者必须将下面列出的IP地址块添加到其中。

**CRM同步**

Marketo Engage [Salesforce CRM同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} 是向CRM供应商发布的API发出出站HTTP请求的集成机制。 您必须确保您的IT组织不会阻止下面的任何IP地址块访问您的CRM供应商API。

**Marketo Engage出站IP地址块**

下表介绍了所有发出出站调用的Marketo Engage服务器。 允许列表如果您正在配置任何IP、服务器、防火墙、访问控制列表、安全组或第三方服务来接收来自Marketo Engage的传出连接，请使用以下列表。

<table>
 <tbody>
  <tr>
   <th>IP块（CIDR表示法）</th>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>130.248.244.88/29</td>
  </tr>
  <tr>
   <td>185.28.196.0/22</td>
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

<table>
 <tbody>
  <tr>
   <th>单个IP地址</th>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
   <tr>
   <td>44.235.171.179</td>
  </tr>
   <tr>
   <td>35.165.244.220</td>
  </tr>
   <tr>
   <td>52.20.211.99</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
   <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
   <tr>
   <td>54.220.138.65</td>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
 </tbody>
</table>


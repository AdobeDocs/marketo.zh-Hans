---
unique-page-id: 4720433
description: 为 Marketo Engage 配置协议 — Marketo Engage 文档 — 产品文档
title: 为 Marketo Engage 配置协议
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: ee8b46179d9fe85c4d5f2ebd7c2d31b7fbf516c3
workflow-type: tm+mt
source-wordcount: '2129'
ht-degree: 100%

---

# 为 Marketo Engage 配置协议{#configure-protocols-for-marketo-engage}

如果您或您的组织使用了较为严格的防火墙或代理服务器设置，您或您的网络管理员可能需要将某些域名和 IP 地址范围加入允许列表，以确保 Adobe Marketo Engage 能够正常运行。

如需协助实施以下协议，请将本文分享给您的 IT 部门。如果他们通过允许列表来限制 Web 访问，请务必将以下域名（包括星号）加入允许列表，以放行所有 Marketo Engage 资源和 WebSocket 连接：

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## 步骤 1：为登陆页面和电子邮件创建 DNS 记录 {#step-create-dns-records-for-landing-pages-and-email}

**跟踪链接 CNAME**

您的营销团队应该已经向您发送了两个新的 CNAME 记录请求。第一个用于登陆页面 URL，使登陆页面在 URL 中显示为您的域名，而不是 Marketo Engage（实际主机）。第二个用于 Marketo Engage 发送的电子邮件中所包含的跟踪链接。

`1` **为登陆页面添加 CNAME**

将营销团队提供的着陆页 CNAME 添加到您的 DNS 记录中，使 `[YourLandingPageCNAME]` 指向分配给 Marketo Engage 着陆页的唯一帐户字符串。登录您的域名注册商网站，并输入登陆页面 CNAME 和帐户字符串。通常需要填写以下三个字段：

* 别名：输入 `[YourLandingPageCNAME]`（由营销团队提供）
* 类型：CNAME
* 指向：输入 `[MunchkinID].mktoweb.com`（由营销团队提供）

`2` **为电子邮件跟踪链接添加 CNAME**

将营销团队提供的电子邮件 CNAME 添加到 DNS 中，使 `[YourEmailCNAME]` 指向 Marketo Engage 分配的默认跟踪链接 [MktoTrackingLink]，格式如下：
`[YourEmailCNAME].[YourDomain].com` IN CNAME `[MktoTrackingLink]`

例如：

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` 必须是默认品牌域。

`3` **通知您的营销团队**

完成上述流程后，请通知您的营销团队。

`4` **联系 [Adobe 支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}以启动 SSL 证书的配置流程。**

该流程最多可能需要 3 个工作日完成。

## 步骤 2：将 Marketo Engage 的 IP 地址加入允许列表 {#step-allowlist-marketo-ips}

当您的营销团队使用 Marketo Engage 发送测试电子邮件（这是在大规模群发电子邮件前的最佳做法）时，这些测试电子邮件有时会遭到依赖发件人 IP 地址进行验证的反垃圾系统拦截。为确保测试电子邮件能够成功送达，请将 Marketo Engage 加入允许列表。

请将以下 IP 地址添加到您公司的允许列表中：

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

某些反垃圾系统会使用电子邮件的 Return-Path 字段（而非 IP 地址）进行允许列表校验。在这种情况下，最佳做法是将 &#39;&#42;.mktomail.com&#39; 加入允许列表，因为 Marketo Engage 使用了多个邮件子域。还有一些反垃圾系统会基于发件人地址进行允许列表校验。在这些情况下，请务必将营销团队用于与人员/潜在客户沟通的所有发件人域名加入允许列表。

>[!NOTE]
>
>Postini 使用了一种独特的技术，需要将 IP 地址范围加入允许列表。请参阅[使用 Postini 进行允许列表配置](https://nation.marketo.com/docs/DOC-1066)。

## 步骤 3：设置 SPF 和 DKIM {#step-set-up-spf-and-dkim}

您的营销团队还应已向您发送需要添加到 DNS 资源记录中的 DKIM（Domain Keys Identified Mail）信息（如下所列）。请按照以下步骤成功配置 DKIM 和 SPF（Sender Policy Framework），完成后通知您的营销团队已更新。

1. 要设置 SPF，请在您的 DNS 条目中添加以下内容：

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`
include: mktomail.com ~all

   如果您的 DNS 条目中已存在 SPF 记录，只需在其中添加以下内容即可：
include: mktomail.com

   请将 CompanyDomain 替换为您网站的主域名（例如 “`(company.com/)`”），并将 CorpIP 替换为您公司电子邮件服务器的 IP 地址（例如“255.255.255.255”）。如果您将通过 Marketo Engage 使用多个域名发送电子邮件，请让 IT 人员为每个域名分别添加这一行（每个域名一行）。

1. 对于 DKIM，请为需要配置的每个域创建 DNS 资源记录。以下是将用于签名的各个域的主机记录和 TXT 值：

   `[DKIMDomain1]`：主机记录是 `[HostRecord1]`，TXT 值为 `[TXTValue1]`。

   `[DKIMDomain2]`：主机记录是 `[HostRecord2]`，TXT 值为 `[TXTValue2]`。

   在按照[此处说明](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}完成设置后，请复制每个 DKIMDomain 对应的 HostRecord 和 TXTValue。在 IT 人员完成此步骤后，请务必在“管理员”>“电子邮件”>“DKIM”中验证每个域。

## 步骤 4：设置 DMARC {#set-up-dmarc}

DMARC (Domain-based Message Authentication, Reporting &amp; Conformance) 是一种身份验证协议，用于帮助组织防止其域名在未经授权的情况下使用。DMARC 扩展了现有的身份验证协议（如 SPF 和 DKIM），用于在域名验证失败时告知接收方服务器应采取的处理措施。尽管 DMARC 目前为可选配置，但强烈建议启用，因为它可以更好地保护您组织的品牌与声誉。自 2024 年 2 月起，Google、Yahoo 等主要服务商将要求批量发件人必须使用 DMARC。

为了使 DMARC 正常运行，您必须至少拥有以下 DNS TXT 记录之一：

* 有效的 SPF
* 为您的 FROM 域配置有效的 DKIM 记录（建议用于 Marketo Engage）

此外，您还必须为 FROM 域配置一条 DMARC 专用的 DNS TXT 记录。您还可以选择性地指定一个电子邮件地址，用于接收 DMARC 报告，以便在组织内部进行监控。

作为最佳做法，建议逐步推进 DMARC 的实施：随着您对 DMARC 潜在影响的了解不断加深，将 DMARC 策略从 p=none 逐步升级为 p=quarantine，再到 p=reject，并将 SPF 和 DKIM 的 DMARC 对齐方式设置为宽松对齐。

### DMARC 示例工作流程 {#dmarc-example-workflow}

1. 如果您已配置接收 DMARC 报告，应执行以下操作…

   I. 分析您收到的反馈和报告，并使用（p=none）策略，该策略会告知接收方对未通过验证的电子邮件不采取任何处理措施，但仍会向发件人发送报告。

   II. 如果合法电子邮件未能通过验证，请检查并修复 SPF/DKIM 相关问题。

   III. 确定 SPF 或 DKIM 是否已对齐，并确保所有合法电子邮件均通过身份验证。

   IV. 查看报告，确认结果是否符合您基于 SPF/DKIM 策略的预期。

1. 随后将策略调整为（p=quarantine），该策略会告知接收方电子邮件服务器对未通过验证的电子邮件进行隔离（通常意味着将电子邮件放入垃圾电子邮件文件夹）。

   I. 查看报告，确保结果符合预期。

1. 如果您对 p=quarantine 级别下电子邮件的处理行为感到满意，可以将策略调整为（p=reject）。p=reject 策略会告知接收方完全拒绝（退回）所有未通过验证、来自该域的电子邮件。启用该策略后，只有 100% 通过域验证的电子邮件才有机会进入收件箱。

>[!CAUTION]
>
>请谨慎使用此策略，并确定其是否适合您的组织。

### DMARC 报告 {#dmarc-reporting}

DMARC 提供的功能可以接收关于 SPF/DKIM 验证失败电子邮件的报告。在身份验证过程中，ISP 服务商会生成两种不同类型的报告，发件人可通过 DMARC 策略中的 RUA/RUF 标签接收这些报告。

* 汇总报告（RUA）：不包含任何可能涉及 GDPR（通用数据保护条例）敏感性的个人身份信息（PII）。

* 取证报告（RUF）：包含电子邮件地址，属于 GDPR 敏感信息。在使用前，建议先在组织内部确认如何处理需要符合 GDPR 要求的信息。

这些报告的主要用途是获得那些试图进行欺骗的电子邮件的概述情况。这些报告技术性较强，通常建议借助第三方工具进行分析。

### DMARC 记录示例 {#example-dmarc-records}

* 最低配置记录：`v=DMARC1; p=none`

* 指定接收报告电子邮件地址的记录：`v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### DMARC 标记及其作用 {#dmarc-tags-and-what-they-do}

DMARC 记录有多个名为 DMARC 标记的组件。每个标记都有一个值，用于指定 DMARC 的某个方面。

<table>
<thead>
  <tr>
    <th>标记名称 </th>
    <th>必填/可选 </th>
    <th>函数 </th>
    <th>示例 </th>
    <th>默认值 </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>v</td>
    <td>必需</td>
    <td>此 DMARC 标记用于指定版本。目前仅有一个版本，因此该值固定为 v=DMARC1。</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>必需</td>
    <td>表示所选的 DMARC 策略，并指示接收方对未通过验证的电子邮件进行报告、隔离或拒绝。</td>
    <td>p=none、quarantine 或 reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>可选</td>
    <td>允许域所有者指定报告选项。</td>
    <td>0：仅当所有验证均失败时生成报告
    <br>1：只要任一验证失败即生成报告
    <br>d：当 DKIM 验证失败时生成报告
    <br>s：当 SPF 验证失败时生成报告</td>
    <td>1（建议用于 DMARC 报告）</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>可选</td>
    <td>指定应用筛选策略的电子邮件百分比。</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>可选（推荐）</td>
    <td>指定汇总报告的投递地址。</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>可选（推荐）</td>
    <td>指定取证报告的投递地址。</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>可选</td>
    <td>指定父域名下子域的 DMARC 策略。</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>可选</td>
    <td>可设置为严格（s）或宽松（r）。宽松对齐表示 DKIM 签名中使用的域可以是 From 地址域的子域。严格对齐表示 DKIM 签名中使用的域必须与 From 地址中的域完全一致。</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>可选</td>
    <td>可设置为严格（s）或宽松（r）。宽松对齐表示 ReturnPath 域可以是 From 地址域的子域。严格对齐表示 Return-Path 域必须与 From 地址完全一致。</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

有关 DMARC 及其所有选项的完整详情，请访问 [https://dmarc.org/](https://dmarc.org/){target="_blank"}。

### DMARC 和 Marketo Engage {#dmarc-and-marketo-engage}

DMARC 有两种对齐方式：DKIM 对齐和 SPF 对齐。

>[!NOTE]
>
>对于 Marketo Engage，建议优先采用基于 DKIM 的 DMARC 对齐，而非 SPF 对齐。

* DKIM 对齐的 DMARC——要设置 DKIM 对齐的 DMARC，您必须：

   * 为电子邮件的 FROM 域设置 DKIM。请按照[本文](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}中的说明进行操作。
   * 为先前已配置的 FROM / DKIM 域配置 DMARC。

* SPF 对齐的 DMARC——要通过品牌化 Return-Path 设置 SPF 对齐的 DMARC，您必须：

   * 设置品牌化 Return-Path 域
      * 配置相应的 SPF 记录
      * 将 MX 记录指向发送电子邮件所在数据中心的默认 MX

   * 为品牌化 Return-Path 域配置 DMARC

* 如果您通过专用 IP 从 Marketo Engage 发送电子邮件，且尚未实施品牌化 Return-Path，或不确定是否已实施，请向 [Adobe 支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}提交工单。

* 如果您通过共享 IP 池从 Marketo Engage 发送电子邮件，可[在此申请](https://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}以查看是否符合 Trusted IP 的资格。对于使用 Marketo Engage Trusted IP 发送电子邮件的客户，将免费提供品牌化 Return-Path。如果获批该项目，请联系 Adobe 支持以配置品牌化 Return-Path。

   * Trusted IP：为每月发送量低于 75,000 且不符合专用 IP 条件的低发送量用户预留的共享 IP 池。这些用户还必须符合相关最佳做法要求。

* 如果您通过共享 IP 从 Marketo Engage 发送电子邮件，且不符合 Trusted IP 条件并且每月发送量超过 100,000 封，则需要联系 Adobe 客户团队（您的客户经理）购买专用 IP。

* Marketo Engage 不支持，也不建议使用严格的 SPF 对齐。

## 步骤 5：为您的域设置 MX 记录 {#step-set-up-mx-records-for-your-domain}

MX 记录允许您接收发送电子邮件所使用域名的来信，以处理回复和自动回复。如果您使用公司域名发送电子邮件，通常已经配置了该项。如果尚未配置，通常可以将其设置为映射到公司域名的 MX 记录。

## 出站 IP 地址 {#outbound-ip-addresses}

出站连接是指 Marketo Engage 代表您向互联网上的服务器发起的连接。您合作的一些合作伙伴/供应商，或您自己的 IT 团队，可能会通过允许列表来限制对服务器的访问。如果是这样，您必须向他们提供 Marketo Engage 出站 IP 地址块，以添加到他们的允许列表中。

**Webhook**

Marketo Engage [Webhook](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} 是一种出站集成机制。当在智能营销活动中执行[调用 Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} 的流程操作时，会向外部 Web 服务发起一个 HTTP 请求。如果该外部 Web 服务所在网络的防火墙使用了允许列表，则服务提供方必须将以下 IP 地址段加入其允许列表。

**CRM 同步**

Marketo Engage 的 [Salesforce CRM 同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"}和 [Microsoft Dynamics 同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"}是通过向 CRM 供应商提供的 API 发起出站 HTTP 请求来实现的集成机制。您必须确保 IT 团队不会阻止以下任何 IP 地址段访问您的 CRM 供应商 API。

**Marketo Engage 出站 IP 地址段**

下表列出了所有会发起出站调用的 Marketo Engage 服务器。如果您正在为服务器、防火墙、访问控制列表、安全组或第三方服务配置 IP 允许列表，以接收来自 Marketo Engage 的出站连接，请使用以下列表。

<table>
 <tbody>
  <tr>
   <th>IP 块（CIDR 表示法）</th>
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
   <th>个人 IP 地址</th>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
  <tr>
   <td>35.165.244.220</td>
  </tr>
  <tr>
   <td>44.235.171.179</td>
  </tr>
  <tr>
   <td>52.20.211.99</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
  <tr>
   <td>54.220.138.65</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  <tr>
   <td>124.47.174.193</td>
  </tr>
  <tr>
   <td>130.248.168.16</td>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
  <tr>
   <td>199.15.213.245</td>
  </tr>
  <tr>
   <td>199.15.215.245</td>
  </tr>
 </tbody>
</table>

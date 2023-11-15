---
description: 更新了配置协议文档 — Marketo文档 — 产品文档
title: 更新了“配置协议”文档
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 1152e81462fb77dd23ff57e26ded7f9b3c02c258
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 2%

---

# 更新了“配置协议”文档 {#updated-configure-protocols-doc}

如果您或您的组织使用限制性的防火墙或代理服务器设置，则您或您的网络管理员可能需要允许列表某些域和IP地址范围，以确保Adobe Marketo Engage按预期工作。

为帮助实施以下协议，请与您的IT部门分享本文。 如果他们使用允许列表限制Web访问，请确保他们添加以下域（包括星号）以允许所有Marketo资源和Web套接字：

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## 步骤1：为登陆页面和电子邮件创建DNS记录 {#step-create-dns-records-for-landing-pages-and-email}

**跟踪链接CNAME**

您的营销团队应向您发送两个请求以获取新CNAME记录。 第一个是用于登陆页面URL，这样登陆页面就会显示在反映您域的URL中，而不是显示在Marketo（实际的主机）中。 第二个用于跟踪从Marketo发送的电子邮件中包含的链接。

`1` **为登陆页面添加CNAME**

添加他们发送给您的DNS记录的登陆页面CNAME，以便 `[YourLandingPageCNAME]` 指向分配给Marketo登陆页面的唯一帐户字符串。 登录到域注册器的网站，然后输入登陆页面CNAME和帐户字符串。 通常，这涉及三个字段：

* 别名：输入 `[YourLandingPageCNAME]` （由营销提供）
* 类型：CNAME
* 指向：输入 `[MunchkinID].mktoweb.com` （由营销提供）

`2` **为电子邮件跟踪链接添加CNAME**

添加营销活动发送给您的电子邮件(CNAME)，以便 `[YourEmailCNAME]` 指向 [MktoTrackingLink]，Marketo分配的默认跟踪链接，格式为：\
`[YourEmailCNAME].[YourDomain].com` 在CNAME中 `[MktoTrackingLink]`

例如：

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` 必须是默认品牌策略域。

`3` **通知您的营销团队**

完成此过程后，请通知您的营销团队。

`4` **联系人 [Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} 开始预配SSL证书的进程。**

完成此过程最多可能需要3个工作日。

## 步骤2：允许列表Marketo IP {#step-allowlist-marketo-ips}

当您的营销团队使用Marketo发送测试电子邮件（发送电子邮件冲击之前的最佳实践）时，测试电子邮件有时会被依赖发件人IP地址来验证电子邮件有效的反垃圾邮件系统阻止。 要确保这些测试电子邮件到达，请将Marketo添加到您的允许列表。

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

某些反垃圾邮件系统使用电子邮件返回路径字段而不是IP地址进行分配。 在这些情况下，最好的方法是允许列表&#39;&#42;.mktomail.com&#39;，因为Marketo使用多个邮箱子域。 其他反垃圾邮件系统根据发件人地址进行允许列表。 在这些情况下，请确保包括营销组用于与人员/潜在客户通信的所有发送（“发件人”）域。

>[!NOTE]
>
>Postini采用独特的技术，需要列入允许列表IP范围。 请参阅 [使用Postini进行列入允许列表](https://nation.marketo.com/docs/DOC-1066).

## 步骤3：设置SPF和DKIM {#step-set-up-spf-and-dkim}

您的营销团队还应向您发送要添加到DNS资源记录的DKIM（域密钥识别邮件）信息（也如下所列）。 按照步骤成功配置DKIM和SPF (Sender Policy Framework)，然后通知您的营销团队此策略已更新。

1. 要设置SPF，请将以下行添加到我们的DNS条目中：

   `[CompanyDomain]` 在TXT中v=spf1 mx ip4：`[CorpIP]`\
   include： mktomail.com ~all

   如果我们的DNS条目中已存在现有的SPF记录，只需将以下内容添加到该记录中：\
   包括： mktomail.com

   将CompanyDomain替换为您的网站的主域(例如： ”`(company.com/)`“)和CorpIP ，以及您的公司电子邮件服务器的IP地址(例如 &quot;255.255.255.255&quot;). 如果您要通过Marketo从多个域发送电子邮件，则应让IT员工为每个域添加此行（在一行中）。

1. 对于DKIM，请为要设置的每个域创建DNS资源记录。 以下是我们将签署的每个域的主机记录和TXT值：

   `[DKIMDomain1]`：主机记录为 `[HostRecord1]` 并且TXT值为 `[TXTValue1]`.

   `[DKIMDomain2]`：主机记录为 `[HostRecord2]` 并且TXT值为 `[TXTValue2]`.

   在执行以下操作后，为您设置的每个DKIMDomain复制HostRecord和TXTValue [此处说明](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. 在您的IT员工完成此步骤后，请不要忘记在“管理员”>“电子邮件”>“DKIM”中验证每个域。

## 步骤4：设置DMARC（基于域的消息身份验证、报告和符合性） {#set-up-dmarc}

DMARC是一种身份验证协议，用于帮助组织保护其域免遭未经授权的使用。 DMARC扩展了现有的身份验证协议，如SPF和DKIM，以通知收件人服务器如果在其域上发生身份验证失败他们应该采取的操作。 尽管DMARC目前是可选的，但强烈建议使用，因为它将更好地保护您组织的品牌和声誉。 从2024年2月开始，Google和雅虎等主要提供商将要求批量发送者使用DMARC。

要使DMARC正常工作，您必须至少具有以下DNS TXT记录之一：

* 有效的SPF
* 您的FROM：域的有效DKIM记录(建议进行Marketo Engage)

此外，您的FROM：域必须具有特定于DMARC的DNS TXT记录。 （可选）可以定义您选择的电子邮件地址以指示DMARC报告在您的组织内的放置位置，以便您能够监视报告。

作为最佳实践，建议您逐步推出DMARC实施，方法是将DMARC政策从p=none提升到p=quarantine，再提升到p=reject，以便了解DMARC的潜在影响，并将DMARC政策设置为放松在SPF和DKIM上的协调一致。

### DMARC示例工作流 {#dmarc-example-workflow}

1. 如果您配置为接收DMARC报告，您应该执行以下操作……

   I.分析您收到并使用的反馈和报告(p=none)，这告知接收者不对验证失败的邮件执行任何操作，但仍会向发件人发送电子邮件报告。

   二、 如果合法消息未通过身份验证，请查看并修复SPF/DKIM问题。

   三、 确定SPF或DKIM是否一致，并通过所有合法电子邮件的身份验证。

   四、 审阅报告以确保根据SPF/DKIM策略得出的结果符合您的预期。

1. 继续将策略调整为(p=quarantine)，以告知接收电子邮件服务器隔离身份验证失败的电子邮件（这通常意味着将这些邮件放入垃圾邮件文件夹）。

   一。审查报告，确保结果符合预期。

1. 如果您对处于p=隔离级别的消息的行为感到满意，则可以调整策略为(p=reject)。 p=reject策略告知接收者完全拒绝（退回）验证失败的域的任何电子邮件。 启用此策略后，只有经域验证为100%经过身份验证的电子邮件才有机会放置收件箱。

>[!CAUTION]
>
>请谨慎使用此策略，并确定它是否适合您的组织。

### DMARC报告 {#dmarc-reporting}

DMARC提供接收有关SPF/DKIM失败的电子邮件的报告的功能。 在身份验证过程中，ISP服务生成了两个不同的报告，发件人可以通过其DMARC策略中的RUA/RUF标记接收这些报告。

* 汇总报表(RUA)：不包含任何对GDPR（《通用数据保护条例》）敏感的PII（个人身份信息）。

* 取证报告(RUF)：包含对GDPR敏感的电子邮件地址。 在使用之前，最好在内部检查如何处理需要符合GDPR的信息。

这些报告的主要用途是接收尝试欺骗的电子邮件概述。 这些是技术含量很高的报告，最好通过第三方工具消化。

### 示例DMARC记录 {#example-dmarc-records}

* 最低裸记录： `v=DMARC1; p=none`

* 记录指向接收报告的电子邮件地址： `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### DMARC标记及其用途 {#dmarc-tags-and-what-they-do}

DMARC记录具有多个名为DMARC标记的组件。 每个标记都有一个值，该值指定DMARC的某些方面。

<table>
<thead>
  <tr>
    <th>标记名称 </th>
    <th>必需/可选 </th>
    <th>函数 </th>
    <th>示例 </th>
    <th>默认值 </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>v</td>
    <td>必需</td>
    <td>此DMARC标记指定版本。 目前只有一个版本，因此其固定值为v=DMARC1</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>必需</td>
    <td>显示选定的DMARC策略，并指示接收者报告、隔离或拒绝未通过身份验证检查的邮件。</td>
    <td>p=none、quarantine或reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>可选</td>
    <td>允许域所有者指定报告选项。</td>
    <td>0：如果一切失败，则生成报告 
    <br>1：如果任何操作失败，则生成报表 
    <br>d：如果DKIM失败，则生成报告 
    <br>s：如果SPF失败，则生成报告</td>
    <td>1（建议用于DMARC报表）</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>可选</td>
    <td>告知受过滤的邮件的百分比。</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>可选（推荐）</td>
    <td>标识将提交汇总报表的位置。</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>可选（推荐）</td>
    <td>确定将提交鉴证报告的位置。</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>可选</td>
    <td>为父域的子域指定DMARC策略。</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>可选</td>
    <td>可以是严格(s)或宽松®。 松弛对齐意味着DKIM签名中使用的域可以是“发件人”地址的子域。 严格对齐意味着DKIM签名中使用的域必须与发件人地址中使用的域完全匹配。</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>可选</td>
    <td>可以是严格(s)或宽松®。 宽松的对齐意味着ReturnPath域可以是From Address的子域。 严格对齐意味着Return-Path域必须与From地址完全匹配。</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

有关DMARC及其所有选项的完整详细信息，请访问 [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC和Marketo Engage {#dmarc-and-marketo-engage}

DMARC有两种对齐方式：DKIM对齐和SPF对齐。

>[!NOTE]
>
>建议对Marketo的DKIM与SPF执行DMARC对齐。

* DKIM-aligned DMARC — 要设置DKIM-aligned DMARC，您必须：

   * 为消息的FROM：域设置DKIM。 按照说明操作 [本文内容](help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * 为之前配置的FROM：/DKIM域配置DMARC

* DMARC-aligned SPF — 要通过标记返回路径设置DMARC-aligned SPF，您必须：

   * 设置标记的Return-Path域
      * 配置相应的SPF记录
      * 更改MX记录以指向发送邮件的数据中心的默认MX

   * 为标记的Return-Path域配置DMARC

* 如果您通过专用IP从Marketo发送邮件，并且尚未实现标记返回路径，或者不确定您是否实现了标记返回路径，请打开一个票证，其中包含 [Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* 如果您通过共享IP池从Marketo发送邮件，则可以查看您是否符合受信任IP的条件 [在此处应用](http://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}. 对于从Marketo的受信任IP发送的用户，免费提供品牌化的返回路径。 如果批准此计划，请联系Marketo支持部门以设置标记的return-path。

   * 受信任的IP：为月发送数少于75K且不符合专用IP条件的低容量用户保留的共享IP池。 这些用户还必须满足最佳实践要求。

* 如果您通过共享IP从Marketo发送邮件，但没有资格使用受信任IP，并且每月发送的邮件数超过100,000条，则需要联系Adobe客户团队（您的客户经理）以购买专用IP。

* 在Marketo中，不支持也不建议使用严格的SPF对齐方式。

## 步骤5：为您的域设置MX记录 {#step-set-up-mx-records-for-your-domain}

利用MX记录，可接收发往所发电子邮件之域的邮件，以处理回复和自动回复者。 如果您从公司域发送，则可能已配置此域。 如果没有，则通常可以将其设置为映射到企业域的MX记录。

## 出站IP地址 {#outbound-ip-addresses}

出站连接是指Marketo Engage代表您连接到Internet上的服务器。 列入允许列表与您合作的一些合作伙伴/供应商或您自己的IT部门可能会使用限制对服务器的访问。 如果是，则必须向他们提供Marketo Engage列入允许列表出站IP地址块，以将其添加到其。

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} 流程操作作为智能营销活动的一部分执行，会向外部Web服务发出HTTP请求。 列入允许列表 列入允许列表如果Web服务发布者在外部Web服务所在网络的防火墙上使用，则发布者必须将下面列出的IP地址块添加到其中。

**CRM同步**

Marketo Engage [Salesforce CRM同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} 是向CRM供应商发布的API发出出站HTTP请求的集成机制。 您必须确保您的IT组织不会阻止下面的任何IP地址块访问您的CRM供应商API。

**Marketo Engage出站IP地址块**

下表列出了所有发出出站调用的Marketo Engage服务器。 列入允许列表如果您正在配置任何IP、服务器、防火墙、访问控制列表、安全组或第三方服务来接收来自Marketo Engage的传出连接，请使用下面的列表。

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
  </tr>
   <tr>
   <td>130.248.168.16</td>
  </tr>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
 </tbody>
</table>

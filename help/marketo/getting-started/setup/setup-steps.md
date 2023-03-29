---
unique-page-id: 2949469
description: 设置步骤 — Marketo文档 — 产品文档
title: 设置步骤
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
source-git-commit: 6dc38462b08f9db639d2d5ee005c4bdf5131b701
workflow-type: tm+mt
source-wordcount: '2054'
ht-degree: 0%

---

# 设置步骤 {#setup-steps}

**欢迎使用Marketo Engage!**

在深入研究使用Marketo之前，您需要先完成一些步骤。

这些步骤包括：

* 一些基本帐户设置
* 将登陆页面URL和电子邮件链接品牌化，以提高信任度和投放能力
* 正在同步CRM
* 将跟踪代码添加到公司网站

>[!NOTE]
>
>您只需在公司为 **新Marketo**. 如果没有，则安装程序可能已经完成。

某些步骤需要您的IT团队提供帮助。

>[!TIP]
>
>如果您 [打印此核对清单](/help/marketo/getting-started/setup/setup-checklist.md){target="_blank"}，则可以在完成项目时将其勾选出来。

## 登录并创建其他Marketo用户 {#log-in-and-create-additional-marketo-users}

1. 登录Marketo [此处](https://app.marketo.com/){target="_blank"} 使用您通过电子邮件收到的凭据。

   ![](assets/setup-steps-1.png)

恭喜！你现在在Marketo，可以开始探索。 您可能希望邀请您营销团队的同事加入您。 您可以通过添加新用户来执行此操作。

转到 **管理员** 的上界。

>[!TIP]
>
>在此时，您可以单击 **我的帐户** 更改帐户和位置设置，以及设置新的订阅名称。

![](assets/setup-steps-2.png)

>[!NOTE]
>
>**需要管理员权限**

单击 **用户和角色**.

![](assets/setup-steps-3.png)

单击 **邀请新用户**.

![](assets/setup-steps-4.png)

填写您同事的电子邮件地址、名字和姓氏。 _设置访问过期日期是可选的_. 单击 **下一个**.

![](assets/setup-steps-5.png)

>[!TIP]
>
>对于只需要短暂访问Marketo的短期外部利益相关方或顾问而言，过期日期非常有用。

>[!NOTE]
>
>到达过期日期后，用户会收到过期通知并锁定帐户。

选择角色并单击 **下一个**. 标准用户有权访问除管理员之外的所有区域。

![](assets/setup-steps-6.png)

>[!NOTE]
>
>除了五个内置角色之外，您还可以创建自定义角色。 详细了解 [管理用户角色和权限](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.

请随意调整邀请文本。 单击 **发送**.

![](assets/setup-steps-7.png)

新用户现在列在“用户”选项卡中，应会收到一封包含创建密码和登录链接的电子邮件。 下一步！

![](assets/setup-steps-8.png)

## 设置授权支持联系人 {#set-up-your-authorized-support-contacts}

您可能已收到Marketo支持部门发来的一封电子邮件，声明您是贵公司的Marketo客户支持管理员。 如果是，您可以设置 **授权支持联系人** 为你的团队。 只有授权的支持联系人才能直接通过 [Marketo支持门户](https://support.marketo.com){target="_blank"}.

>[!NOTE]
>
>您可以创建的支持联系人数量取决于您购买的包。 此限制在您来自Marketo支持团队的电子邮件中指定。

授权支持联系文档已移至Marketo社区。 请参阅 [本文](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341){target="_blank"}.

>[!NOTE]
>
>列表中只显示已登录Marketo社区的人员。 如果找不到该人员，请确保他们首先登录到社区。

## 使用CNAME自定义登陆页面URL {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>您是Launch Pack客户吗？ 您可以跳过此步骤。 您的顾问将在您的启动电话会议期间为您提供IT设置说明文档。

>[!NOTE]
>
>**需要管理员权限**

为登陆页面选择CNAME。 一些示例：

    * **开始**。[CompanyDomain].com
    * **ww2**。[CompanyDomain].com
    * **lp**。[CompanyDomain].com

>[!TIP]
>
>保持简短！ 较短的URL更容易记忆。 我们建议将“go”作为域。

第一部分（粗体部分）是 `[LandingPageCNAME]`. 在步骤5中，您将需要它。

要检索将要替换为登陆页面CNAME的Munchkin ID，请转到“管理员”区域。

![](assets/setup-steps-9.png)

单击 **我的帐户**.

![](assets/setup-steps-10.png)

向下滚动到“支持信息”，并复制您的Munchkin ID。

![](assets/setup-steps-11.png)

这是 `[Munchkin ID]`. 保存它。 您需要在步骤5中将其授予IT。

配置域设置，以便登陆页面使用您公司的域，而不是Marketo的域（托管这些域的位置）。

## 确保电子邮件可投放性 {#ensure-email-deliverability}

>[!NOTE]
>
>您是Launch Pack客户吗？ 您可以跳过此步骤。 您的顾问将在您的启动电话会议期间为您提供IT设置说明文档。

您可以采取多种措施来确保电子邮件能够尽可能多地联系您的人员。

* **为您的跟踪链接设置品牌**. 您可以选择一个CNAME，以在包含在Marketo电子邮件中的链接中使用您自己的域(而不是Marketo的域)。 这可增强您的域名品牌，并增加与收件人的信任和投放能力。
* **将Marketo添加到您的公司电子邮件允许列表。** 在向实际人员发送电子邮件之前，向测试帐户发送测试电子邮件是一种常见的最佳实践。 通过列入允许列表Marketo，您可以阻止这些测试电子邮件被阻止或标记为垃圾邮件。
* **设置SPF和DKIM。** 这些技术可确保您的收件人知晓Marketo电子邮件不是垃圾邮件。 要帮助防止收件人的垃圾邮件过滤器拒绝您的Marketo电子邮件，请按照以下步骤操作 [为电子邮件投放能力设置SPF和DKIM](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **为域设置MX记录。** MX记录允许您接收来自的域的邮件，以处理回复和自动回复。 如果您从公司域发送，则可能已经配置了此设置。 如果没有，您通常可以设置为映射到公司域的MX记录。
* **“发件人”地址的推荐设置。** 您必须在所有电子邮件促销活动的“发件人地址”中使用有效、现有且有效的电子邮件域。 配置公司域的子域（而不是从公司域发送）可能会有所帮助。 这将确保来自您公司邮件流的问题不会影响您的Marketo邮件流，反之亦然。 此外，从 `something@nonexistentdomain.com` 会导致过滤或阻止电子邮件。 发件人发件人地址中使用的任何域都必须具有有效且有效的postmaster@和upuse@帐户。

如果您使用Google应用程序托管公司电子邮件，则无法在您的域下创建ubuse@或postmaster@电子邮件。 要解决此问题，您需要创建名为“滥用”和“邮递员”的组。 属于这些组的成员的用户将收到发送到这些地址的电子邮件(例如postmaster@domain.com)。 有关创建群组的详细说明，请参阅 [此处](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

为电子邮件跟踪链接选择CNAME(选择 _不同_ 从登陆页面中选择的CNAME)。 一些示例：

* go2.[CompanyDomain].com
* em.[CompanyDomain].com
* 哇。[CompanyDomain].com

第一部分是电子邮件跟踪CNAME， `[EmailTrackingCNAME]`. 您需要在步骤5中将其授予IT。

>[!CAUTION]
>
>电子邮件和登陆页面CNAME必须不同。 此外，还应避免出现“track”或“link”等CNAME。 它通常被标记为垃圾信息

要查找Marketo跟踪链接，请转到 **管理员** 的上界。

![](assets/setup-steps-12.png)

单击 **电子邮件**.

![](assets/setup-steps-13.png)

从电子邮件设置中复制跟踪链接。

跟踪链接的形式为： `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-14.png)

这是您的 `[MktoTrackingLink]`. 保存它。 您需要在步骤5中将其授予IT。

收集“发件人”域。 列出所有“从”域(如 `[Sender]@[FromDomain].com`)，以便您计划用于从Marketo发送电子邮件。 对大多数人来说，只有一个。

例如，“marketo.com”、“info.marketo.com”。 这些是 `[FromDomain1]`,`[FromDomain2]`等。 救他们。 您需要在步骤5中将其交给IT。

您现在拥有向IT发送请求所需的所有信息！

## 要求IT人员配置协议 {#ask-it-to-configure-protocols}

>[!NOTE]
>
>您是Launch Pack客户吗？ 您可以跳过此步骤。 您的顾问将在您的启动电话会议期间为您提供IT设置说明文档。

收集所有必需信息后，即可向IT发送请求。 您可以将下面的文本用作模板，将粗体文本替换为您自己的信息。

[包括指向本文的链接](/help/marketo/getting-started/setup/configure-protocols-for-marketo.md).

将此文本粘贴到电子邮件中，并替换加粗体的占位符：

>[!NOTE]
>
>请参阅上面的步骤3和4，以确定要替换占位符的文本。 记住 `[LandingPageCNAME]` 和 `[EmailTrackingCNAME]` 必须不同。

`----------------------------------------------`

尊敬的IT管理员：

我们的营销团队现在正在使用Marketo平台与我们的人员进行通信。 为确保电子邮件投放能力卓越，我们需要进行以下更改：

`1)` 对于我们的登陆页面，添加DNS条目(CNAME) **[LandingPageCNAME]**.**[CompanyDomain]**.com，指向 **[蒙奇金ID]**.mktoweb.com。

`2)` 对于电子邮件中的跟踪链接，请为 **[EmailTrackingCNAME]**.**[CompanyDomain]**.com，指向 **[MktoTrackingLink]**.

`3)` 允许列表Marketo。

    *如果在“电子邮件”中使用IP允许列表地址，请添加以下列IP:
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    103.237.104.0/22
    
    94.236.119.0/26

>[!NOTE]
>
>如果您希望Marketo特定于您的环境的简化IP列表，请允许列表联系支持。

    *如果我们的防垃圾邮件系统使用“来自”域，请添加以下内容：

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` 我们需要设置SPF和DKIM，以便Marketo有权代表我们发送已签名的电子邮件。

`a.` 要设置SPF，请在DNS条目中添加以下行：

在TXT中 **[从域]**:v=spf1 mx ip4:**[公司IP]**
<br/>包括：mktomail.com ~all

如果DNS条目中已有SPF记录，只需在其中添加以下内容：

include:mktomail.com

`[`替换 **从域** 与您的域电子邮件(例如：company.com)和 **CorpIP** 的IP地址(例如：255.255.255.255)。  如果您要通过Marketo从多个域发送电子邮件，则应让IT员工为每个域添加此行（在一行中）。`]`

`b.` 对于DKIM，请为要设置的每个域创建DNS资源记录。 下面是我们将为其签名的每个域的主机记录和TXT值：

**`[DKIMDomain1]`**:主机记录为 **`[HostRecord1]`** 和TXT值为 **[TXTValue1]**.

**`[DKIMDomain2]`**:主机记录为 **`[HostRecord2]`** 和TXT值为 **`[TXTValue2]`**.

`[`复制 **HostRecord** 和 **TXTValue** 每个 **DKIMDomain** 在 [此处说明](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). 请不要忘记在 **管理员>电子邮件> DKIM** 在您的IT员工完成此步骤后。`]`

`5)` 我们需要确保FROM域有有效的MX记录 **[FromDomain1]**, **[FromDomain2]**&#x200B;等。 你能确认吗？ 如果没有，请配置以映射到我们的公司域MX记录。 这将确保我们能够处理对Marketo邮件的回复/自动回复。

完成这些步骤后，请告知我，以便我能够使用Marketo完成设置过程。

谢谢！ 你是最棒的！

爱，

**`[Your Name]`**

`----------------------------------------------`

向IT部门发送电子邮件。 我们了解，IT可能需要一些时间才能完成这些任务。 您可以继续执行步骤7，但请记住，您必须返回步骤6才能完成Marketo设置。

## 在IT完成后完成Marketo设置 {#complete-your-marketo-setup-after-it-finishes}

IT完成其任务后，请按照以下步骤添加登陆页面和电子邮件CNAME，并激活DKIM签名。

转到 **管理员** 添加登陆页面CNAME的区域

![](assets/setup-steps-15.png)

选择登陆页面，然后单击 **编辑** 中。

![](assets/setup-steps-16.png)

在登陆页面的域名字段中输入新域名。 该格式应为：

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-17.png)

在回退页面字段中，输入您希望用户在登陆页面不可用时转到的URL。 如果您没有后备页面，则可以使用您的公司主页。 在主页字段中，输入您的公司网站。

![](assets/setup-steps-18.png)

在“管理员”区域中，选择电子邮件以添加您的电子邮件CNAME

![](assets/setup-steps-19.png)

向下滚动到“品牌化域”。 选择您的域并单击 **编辑**.

![](assets/setup-steps-20.png)

在域字段中，输入您的电子邮件跟踪域。 该格式应为：

`[EmailTrackingCNAME].[CompanyDomain].com`. 单击 **保存**.

![](assets/setup-steps-21.png)

## 集成CRM {#integrate-your-crm}

这可能是您设置的最激动人心的步骤 — 是时候让Marketo中包含您存储在CRM中的所有这些潜在客户和联系人了！

根据您的公司使用的CRM，从以下各项中进行选择。

    * [将Marketo与Salesforce.com集成](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [将Marketo与Microsoft Dynamics集成](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>您需要公司CRM管理员的帮助才能完成这些步骤。

## 将跟踪代码添加到您的网站 {#add-tracking-code-to-your-website}

>[!NOTE]
>
>您是Launch Pack客户吗？ 您可以跳过此步骤。 您的顾问将在您的IT设置说明文档中为您提供Munchkin代码说明。

Marketo具有自定义跟踪JavaScript（称为Munchkin），您可以使用它来跟踪任何网页上的人员活动。 需要将您的网站集成到Marketo中。 按照以下步骤操作 [将Munchkin跟踪代码添加到您的网站](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.

>[!NOTE]
>
>添加跟踪代码所需的HTML体验。

## 性能预期 {#performance-expectations}

您对Marketo的表现有什么期待？ 根据营销活动的规模和复杂性，它可能会有所不同。 但是，您可以期望的性能级别与“标准”列中列出的性能级别(位于 [Marketo Engage产品描述](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}. The "Performance" and "Performance Plus" columns refer to performance tier packages that provide [higher performance levels](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}.

所有设置步骤都结束。 剩下的就是深入使用Marketo!

---
description: 设置步骤 — Marketo文档 — 产品文档
title: 设置步骤
feature: Getting Started
exl-id: 5f37da48-b2ed-4e48-a5a2-429149745085
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '1675'
ht-degree: 0%

---

# 设置步骤 {#setup-steps}

**欢迎使用Adobe Marketo Engage！**

在开始使用之前，您需要完成一些步骤。

这些步骤包括：

* 将您的登陆页面URL和电子邮件链接品牌化，以提高信任度和可投放性
* 配置用于Marketo Engage的协议
* 正在同步您的CRM
* 将跟踪代码添加到您的公司网站

>[!NOTE]
>
>仅当您的公司需要 **初次使用Marketo**. 如果没有，则可能已完成设置。

某些步骤需要您的IT团队提供帮助。

## 确保电子邮件可投放性 {#ensure-email-deliverability}

>[!NOTE]
>
>您是Launch Pack客户吗？ 您可以跳过此步骤。 您的顾问将在您的启动电话中为您提供IT设置说明文档。

可以采取多种措施确保电子邮件可送达尽可能多的用户。

* **将您的跟踪链接品牌化**. 您可以在来自Marketo的电子邮件中包含的链接中，选择使用您自己的域(而不是Marketo)的CNAME。 这加强了您的域品牌化，并增加了与收件人的信任和可投放性。
* **将Marketo添加到您的公司电子邮件允许列表**. 通常的最佳做法是，先向测试帐户发送测试电子邮件，然后再向实际用户发送电子邮件。 通过列入允许列表Marketo，您可以防止这些测试电子邮件被阻止或标记为垃圾邮件。
* **设置SPF和DKIM**. 这些技术可确保收件人您的Marketo电子邮件不是垃圾邮件。 要帮助防止收件人的垃圾邮件过滤器拒绝您Marketo电子邮件，请执行以下步骤： [为您的电子邮件可投放性设置SPF和DKIM](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **为您的域设置MX记录。** 利用MX记录，可接收发往您发送电子邮件的域的邮件，以处理回复和自动回复。 如果您从公司域发送，则可能已配置此域。 如果没有，您通常可以设置映射到企业域的MX记录。
* **发件人地址的建议设置。** 您必须在所有电子邮件营销活动的“发件人地址”中使用有效的、现有的和工作电子邮件域。 配置公司域的子域而不是从公司域发送可能很有用。 这将确保公司邮件流中的问题不会影响您的Marketo邮件流，反之亦然。 此外，发送来自 `something@nonexistentdomain.com` 将导致过滤或阻止电子邮件。 发件人的“发件人地址”中使用的任何域都必须具有有效且有效的邮递员@和滥用@帐户。

如果您使用Google Apps托管公司电子邮件，则无法在您的域下创建滥用@或邮递员@电子邮件。 要解决此问题，您需要创建名为“虐待”和“邮递员”的组。 属于这些组成员的用户将收到发送到这些地址的电子邮件(例如，postmaster@domain.com)。 有关创建组的详细说明，请参阅 [此处](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

为电子邮件跟踪链接选择一个CNAME(选择一个 _不同_ （从您在步骤3中选择的登陆页面CNAME中进行更改）。 一些示例：

* go2。[公司域].com
* em.[公司域].com
* 哇！[公司域].com

第一部分是电子邮件跟踪CNAME， `[EmailTrackingCNAME]`. 您需要将它授予IT。

>[!CAUTION]
>
>电子邮件和登陆页面CNAME必须不同。 此外，请避免使用“跟踪”或“链接”等CNAME。 它通常被标记为垃圾邮件

要查找您的Marketo跟踪链接，请转到 **[!UICONTROL 管理员]** 区域。

![](assets/setup-steps-1.png)

单击 **[!UICONTROL 电子邮件]**.

![](assets/setup-steps-2.png)

复制 [!UICONTROL 跟踪链接] 来自您的电子邮件设置。

此 [!UICONTROL 跟踪链接] 采用以下形式： `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-3.png)

这是您的 `[MktoTrackingLink]`. 保存它。 在步骤5中，您需要将它提供给IT。

收集“发件人”域。 将所有“发件人”域列入列表(如所示， `[Sender]@[FromDomain].com`)中，用于从Marketo发送电子邮件的电子邮件收件人。 对大多数人来说，只有一个。

例如，“marketo.com，”“info.marketo.com，”。 这些是 `[FromDomain1]`，`[FromDomain2]`，等等。 保存它们。 在步骤5中，您需要将它们提供给IT。

您现在掌握了向IT发送请求所需的所有信息！

## 使用CNAME自定义登陆页面URL {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>您是Launch Pack客户吗？ 您可以跳过此步骤。 您的顾问将在您的启动电话中为您提供IT设置说明文档。

>[!NOTE]
>
>**需要管理员权限**

为您的登陆页面选择一个CNAME。 一些示例：

    * **开始**。[公司域].com
    * **www2**。[公司域].com
    * **lp**。[公司域].com

>[!TIP]
>
>保持简短！ 较短的URL更容易记忆。 我们建议“开始”作为域。

第一部分（粗体）是 `[LandingPageCNAME]`. 在步骤5中需要它。

要检索要使用登陆页面CNAME替换的Munchkin ID，请转到 **管理员** 区域。

![](assets/setup-steps-4.png)

单击 **我的帐户**.

![](assets/setup-steps-5.png)

复制 [!UICONTROL 帐户字符串] 登陆页面设置中的。

![](assets/setup-steps-6.png)

这是 `[Munchkin ID]`. 保存它。 在步骤5中，您需要将它提供给IT。

配置您的域设置，以便登陆页面使用您公司的域，而不是Marketo的域（这些网页的托管位置）。

## 要求IT配置协议 {#ask-it-to-configure-protocols}

>[!NOTE]
>
>您是Launch Pack客户吗？ 您可以跳过此步骤。 您的顾问将在您的启动电话中为您提供IT设置说明文档。

收集完所有必要信息后，即可向IT部门发送请求。 您可以使用下面的文本作为模板，将粗体文本替换为您自己的信息。

[包含指向本文的链接](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md).

将此文本粘贴到电子邮件中，并替换粗体占位符：

>[!NOTE]
>
>请参阅上面的步骤3和4 ，确定替换占位符的文本。 请记住 `[LandingPageCNAME]` 和 `[EmailTrackingCNAME]` 必须不同。

`----------------------------------------------`

尊敬的IT管理员：

我们的营销团队现在使用Marketo平台与我们的人员沟通。 为确保出色的电子邮件可投放性，我们需要进行以下更改：

`1)` 对于我们的登陆页面，为添加DNS条目(CNAME) **[LandingPageCNAME]**.**[公司域]**.com，指向 **[Munchkin ID]**.mktoweb.com.

`2)` 对于电子邮件中的跟踪链接，为添加一个DNS条目(CNAME) **[EmailTrackingCNAME]**.**[公司域]**.com，指向 **[MktoTrackingLink]**.

`3)` 允许列表Marketo。

    *如果在电子邮件允许列表中使用IP地址，请添加下面列出的IP：
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
>如果您希望获得简略的IP列表，以便Marketo特定于您的环境的IP，请联系列入允许列表支持。

    *如果我们的反垃圾邮件系统使用“发件人”域，请添加以下内容：

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` 我们需要设置SPF和DKIM，以便Marketo有权代表我们发送签名电子邮件。

`a.` 要设置SPF，请在我们的DNS条目中添加以下行：

在TXT中 **[来自域]**： v=spf1 mx ip4：**[公司IP]**
<br/>include： mktomail.com ~all

如果我们的DNS条目中已存在现有的SPF记录，只需将以下内容添加到该记录中：

include：mktomail.com

`[`替换 **来自域** 使用来自域的电子邮件(例如：company.com)和 **公司IP** （例如： 255.255.255.255）。  如果您要通过Marketo从多个域发送电子邮件，则应让IT员工为每个域添加此行（在一行中）。`]`

`b.` 对于DKIM，请为我们要设置的每个域创建DNS资源记录。 以下是我们将签署的每个域的主机记录和TXT值：

**`[DKIMDomain1]`**：主机记录为 **`[HostRecord1]`** 并且TXT值为 **[TXTValue1]**.

**`[DKIMDomain2]`**：主机记录为 **`[HostRecord2]`** 并且TXT值为 **`[TXTValue2]`**.

`[`复制 **Hostrecord** 和 **TXTValue** 每个 **DKIMDomain** 您在完成以下操作后进行了设置 [此处说明](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). 不要忘记验证中的每个域 **管理员>电子邮件> DKIM** 在IT员工完成此步骤之后。`]`

`5)` 我们需要确保我们的FROM域有有效的MX记录 **[FromDomain1]**， **[FromDomain2]**，等等。 你能确认一下吗？ 如果不能，请配置以映射到我们的公司域MX记录。 这将确保我们能够处理对Marketo邮件的回复/自动响应者。

完成这些步骤后，请通知我，以便我可以使用Marketo完成设置过程。

谢谢！ 你是最好的！

致敬，

**`[Your Name]`**

`----------------------------------------------`

向IT发送电子邮件。 我们理解，IT可能需要一些时间才能完成这些任务。 您可以继续执行下一步，但请记住，您必须返回此步骤才能完成Marketo Engage设置。

## 在IT完成后完成您的Marketo设置 {#complete-your-marketo-setup-after-it-finishes}

在IT人员完成其任务后，请按照以下步骤添加登陆页面和电子邮件CNAME，并激活DKIM签名。

转到 **[!UICONTROL 管理员]** 区域以添加您的登陆页面CNAME

![](assets/setup-steps-7.png)

选择登陆页面并单击 **[!UICONTROL 编辑]** 在 [!UICONTROL 设置] 区域。

![](assets/setup-steps-8.png)

在字段中输入新域名 **[!UICONTROL 登陆页面的域名]**. 其形式应为：

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-9.png)

在 **[!UICONTROL 回退]** 字段，输入当登陆页面不可用时用户转到的URL。 如果您没有回退页，则可以使用公司主页。 在 **[!UICONTROL 主页]** 字段中，输入您的公司网站。

![](assets/setup-steps-10.png)

在 [!UICONTROL 管理员] 区域，选择 **[!UICONTROL 电子邮件]** 添加电子邮件CNAME

![](assets/setup-steps-11.png)

向下滚动到 [!UICONTROL 品牌化域]. 选择您的域并单击 **[!UICONTROL 编辑]**.

![](assets/setup-steps-12.png)

在域字段中，输入电子邮件跟踪域。 其形式应为：

`[EmailTrackingCNAME].[CompanyDomain].com`. 单击&#x200B;**[!UICONTROL 保存]**。

![](assets/setup-steps-13.png)

## 集成您的CRM {#integrate-your-crm}

这可能是你设置中最令人兴奋的部分。 您应该在Marketo中填充所有存储在CRM中的潜在客户和联系人！

根据贵公司使用的CRM，从以下内容中进行选择。

* [将Marketo Engage与集成 [!DNL Salesforce.com]](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
* [将Marketo Engage与集成 [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

  >[!NOTE]
  >
  >要完成这些步骤，您需要公司的CRM管理员的帮助。

## 将跟踪代码添加到您的网站 {#add-tracking-code-to-your-website}

>[!NOTE]
>
>您是 [!DNL Launch Pack] 客户？ 您可以跳过此步骤。 您的顾问将提供 [!DNL Munchkin] IT设置说明文档中的代码说明。

Marketo Engage具有自定义跟踪JavaScript(称为 [!DNL Munchkin])，可用于跟踪任何网页上的人员活动。 [!DNL Munchkin] 要将您的网站集成到Marketo，需要使用。 执行以下步骤： [添加 [!DNL Munchkin] 将代码跟踪到您的网站](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.

>[!NOTE]
>
>添加跟踪代码需要具有HTML的体验。

## 性能期望 {#performance-expectations}

从Marketo的性能来看，您可以期待什么？ 具体情况会因营销活动的规模和复杂性而异。 但是，您可以预期在 [Marketo Engage产品描述](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}. The "Performance" and "Performance Plus" columns refer to performance tier packages that provide [higher performance levels](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}.

>[!MORELIKETHIS]
>
>* [配置用于Marketo Engage的协议](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md)
>
>* [用户设置](/help/marketo/getting-started/initial-setup/user-setup.md)

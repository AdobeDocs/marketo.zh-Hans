---
unique-page-id: 11380218
description: 发行说明 — 2016年夏季 — Marketo文档 — 产品文档
title: 发行说明 — 2016年夏季
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# 发行说明：’16年夏季 {#release-notes-summer}

’16年夏季版本包含以下功能。 查看您的Marketo版本以了解功能的可用性。 请单击标题链接以查看每项功能的详细文章。

## [基于帐户的营销](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Marketo基于帐户的营销在一个统一的平台中提供所有基本功能：

* **Target**  — 帐户发现、帐户匹配和命名帐户列表
* **参与**  — 基于帐户的个性化、跨渠道参与和特定于帐户的工作流
* **测量**  — 帐户和列表级别分析、帐户参与度得分以及管道和收入影响

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM可作为Marketo订阅的附加组件提供，因此请联系您的销售代表以实施它。

## [审核记录](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

审核跟踪提供了在Marketo订阅中所做更改的完整历史记录。 它将在用户和管理员之间创建责任关系，帮助确定意外行为的原因，并提供了解谁在做什么和何时做事的安全性。 此信息将在任何时间点提供，并可用于回答以下问题：

* 此资产或设置发生了什么情况，上次更新时是谁？
* X用户做了什么？
* 谁在登录我们的帐户？

![](assets/audit-trail.png)

## [Marketo — 访问SMS LaunchPoint集成](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md) {#marketo-vibes-sms-launchpoint-integration}

在Marketo中轻松创建短信消息。 使用丰富的Marketo数据个性化和定位消息，并使用短信消息仪表板轻松监控其性能。

>[!NOTE]
>
>此功能要求您现有的访客短信帐户。

![](assets/vibes-sms2.png)

## [Email 2.0增强功能](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**模块级变量**

以前，在Email 2.0模板中指定的所有变量在范围中都是“全局”的。 在模块中使用变量时，如果您计划使用模块的多个实例，则并非总是需要此变量。 在此版本中，变量现在可以指定为“模块级别”，这允许您指示用户应当能够为其中使用的每个模块设置唯一值。

![](assets/module-level-variables.png)

**语法更新**

* 现在，您可以对Email 2.0模板中指定的模块使用“mktoAddByDefault”，以指示新电子邮件默认应显示哪些模块。 如果您要构建包含大量模块的电子邮件模板，则这样会方便得多。
* 在图像元素上，您现在可以指定 `<img>` HTML元素的“高度”和“宽度”属性应被锁定或可编辑给最终用户。 mktoLockImgSize=&quot;true&quot;会导致高度/宽度被锁定（即使图像已更改）。 同样， mktoLockImgStyle=&quot;true&quot;也会导致“style”属性被锁定。

**代码搜索**

使用新的搜索功能，高效地查找和替换电子邮件代码中的内容。 电子邮件模板编辑器中也提供了此功能。

![](assets/2nd-screenshot.png)

**图像元素中的令牌支持**

令牌现在可以在插入图像体验的“外部URL”区域中使用！ 如果您已通过 `{{my.tokens}}`，您现在可以在Email Editor 2.0中引用这些令牌。请注意，图像在Email Editor 2.0画布中仍将显示为已损坏。 但是，在发送电子邮件之前，您将看到这些图像在“预览”和“发送示例”中呈现。

## 多品牌域 {#multiple-branding-domains}

电子邮件跟踪链接只能使用单个品牌化域来添加品牌化的日子已经过去。 您现在可以添加多个品牌域来激发消费者信心，创建更加精简的外观以专注于品牌，提高电子邮件投放能力，然后根据每个电子邮件选择要用于每个电子邮件跟踪链接的品牌域。

![](assets/multiple-branding-domains.png)

## [程序令牌](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

我们为程序创建了新的令牌类型。 您现在可以在资产和智能营销策划流程步骤中渲染项目名称、描述和ID。

![](assets/program-tokens.png)

## [企业密钥](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

要求销售团队的每个人员安装我们的Sales Insight Plugin for Outlook可能很繁琐。 我们引入了一种新方法，可使用企业密钥远程安装Outlook插件。 向您的IT团队发送您在“管理员”的“Marketo销售分析”部分中找到的唯一密钥，并让他们执行其余操作。

![](assets/enterprise-key.png)

## [Web个性化促销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

指定Web营销活动在您的网站上做出反应的时间延迟。

![](assets/dialog-campaign-delay.png)

## [内容分析和Recommendations导出](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

脱机查看内容分析和推荐数据。

## [对电子邮件编辑器2.0的API支持](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

以前仅与v1.0电子邮件和模板兼容的预先存在的资产API现在为v2.0电子邮件资产启用了。

## [Marketo开发人员网站](https://developers.marketo.com/) {#marketo-developers-site}

新增和改进！

## [隐私设置](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

营销人员可以使用隐私设置来决定是否使用Munchkin和Web个性化功能跟踪访客。 跟踪级别可使用浏览器的“不跟踪”设置、选择退出Cookie或非特定IP来控制。 这些方法可能会影响Marketo在特定区域的价值和功能，但是，如果营销人员不更改任何内容，则Marketo功能将保持不变。

此功能将在六周内逐步向客户发布。 如果您需要，请立即联系Marketo支持。

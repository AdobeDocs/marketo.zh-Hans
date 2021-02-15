---
unique-page-id: 11380218
description: 发行说明 — 夏季’16 - Marketo Docs — 产品文档
title: 发行说明 — 2016年夏季
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%

---


# 发行说明：’16年夏季{#release-notes-summer}

’16夏季版包含以下功能。 查看您的Marketo版本以了解功能可用性。 请单击标题链接，以视图每种功能的详细文章。

## [基于帐户的营销](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Marketo Account Based Marketing在一个统一的平台中提供所有基本功能：

* **目标**  — 帐户发现、潜在客户到帐户匹配和指定帐户列表
* **参与**  — 基于帐户的个性化、跨渠道互动和特定于帐户的工作流
* **衡量**  — 帐户和列表级别的洞察、帐户参与程度得分以及渠道和收入影响

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM可作为您的Marketo订阅的附加组件提供，因此请联系您的销售代表以实施它。

## [审核跟踪](https://docs.marketo.com/display/docs/audit+trail) {#audit-trail}

审计跟踪提供了在您的营销订阅中所做更改的完整历史记录。 它将在用户和管理员之间创建责任，帮助确定意外行为的原因，并提供了解谁在做什么和何时做什么的安全性。 此信息将随时可用，并可用于回答以下问题：

* 此资产或设置发生了什么情况，谁上次更新了它？
* X用户做了什么？
* 谁在登录我们的账户？

![](assets/audit-trail.png)

## [Marketo-Vibes SMS LaunchPoint集成](https://docs.marketo.com/display/docs/vibes+sms+messages) {#marketo-vibes-sms-launchpoint-integration}

直接在Marketo中轻松创建SMS消息。 使用丰富的Marketo数据个性化和目标您的信息，并使用SMS消息仪表板轻松监控其性能。

>[!NOTE]
>
>此功能要求您拥有现有的Vibes SMS帐户。

![](assets/vibes-sms2.png)

## [电子邮件2.0增强功能](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**模块级变量**

以前，电子邮件2.0模板中指定的所有变量在作用域中都是“全局”变量。 在模块内使用变量时，如果您计划使用模块的多个实例，则这并不总是可取的。 在此版本中，变量现在可指定为“模块级别”，这允许您指示用户应能够为他们使用的每个模块设置唯一值。

![](assets/module-level-variables.png)

**语法更新**

* 现在，您可以对“电子邮件2.0模板”中指定的模块使用“mktoAddByDefault”，以指示默认情况下新电子邮件中应显示哪些模块。 如果您要构建包含大量模块的电子邮件模板，则这种操作要方便得多。
* 在图像元素上，您现在可以指定基础`<img>` HTML元素的“height”和“width”属性应被锁定，还是可编辑给最终用户。 mktoLockImgSize=&quot;true&quot;将导致高度/宽度被锁定（即使图像已更改）。 同样，mktoLockImgStyle=&quot;true&quot;将导致&quot;style&quot;属性被锁定。

**代码搜索**

使用新的搜索功能高效查找和替换电子邮件代码中的内容。 此功能也可在电子邮件模板编辑器中使用。

![](assets/2nd-screenshot.png)

**图像元素中的令牌支持**

现在可在插入图像体验的“外部URL”区域使用令牌！ 如果您已使用`{{my.tokens}}`指定图像，您现在可以在电子邮件编辑器2.0中引用这些令牌。请注意，图像仍将在电子邮件编辑器2.0画布中显示为损坏。 但是，在发出电子邮件之前，您会看到它们在预览和发送示例中呈现。

## [多个品牌域](https://docs.marketo.com/display/docs/add+multiple+branding+domains) {#multiple-branding-domains}

电子邮件跟踪链接只能用单个品牌域进行品牌标识的时代已经一去不复返。 您现在可以添加多个品牌域来激发消费者信心，创建更加流畅的外观以专注于品牌，提高电子邮件的发送能力，并根据每个电子邮件选择要用于每个电子邮件跟踪链接的品牌域。

![](assets/multiple-branding-domains.png)

## [项目令牌](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

我们为项目创建了新的令牌类型。 您现在可以在资产和智能项目流步骤中呈现活动名称、说明和ID。

![](assets/program-tokens.png)

## [企业密钥](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

要求销售团队中的每个人安装Sales Insight Plugin for Outlook可能很繁琐。 我们引入了一种使用企业密钥远程安装Outlook增效工具的新方法。 将您在管理员的Marketo Sales Insight部分找到的唯一密钥发送给您的IT团队，让他们完成其余工作。

![](assets/enterprise-key.png)

## [Web个性化活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

为Web活动指定时间延迟以在您的网站上做出响应。

![](assets/dialog-campaign-delay.png)

## [内容分析和Recommendations导出](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

视图内容分析和推荐数据脱机。

## [电子邮件编辑器2.0的API支持](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

先前仅与v1.0电子邮件和模板兼容的预存资产API现在为v2.0电子邮件资产启用。

## [Marketo开发人员站点](https://developers.marketo.com/) {#marketo-developers-site}

全新改进！

## [隐私设置](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

营销人员可以使用隐私设置决定是否使用Munchkin和Web个性化功能跟踪访客。 通过使用浏览器的“不跟踪”设置、退出Cookie或非特定IP来控制跟踪级别。 这些方法可能会影响Marketo在特定领域的价值和功能，但如果营销人员没有更改任何内容，Marketo功能将保持不变。

此功能将在六周内逐步向客户发布。 如果您需要，请立即联系Marketo支持。

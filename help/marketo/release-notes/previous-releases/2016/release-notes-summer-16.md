---
unique-page-id: 11380218
description: 发行说明 — 2016年夏天 — Marketo文档 — 产品文档
title: 发行说明 — 2016年夏天
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# 发行说明： 2016年夏天 {#release-notes-summer}

2016年夏季版本中包含以下功能。 检查您的Marketo版本以了解功能可用性。 请单击标题链接以查看每个功能的详细文章。

## [基于帐户的营销](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

基于Marketo帐户的营销在一个统一的平台上提供所有必需品：

* **Target**  — 帐户发现、商机帐户匹配和指定帐户列表
* **参与**  — 基于帐户的个性化、跨渠道参与和特定于帐户的工作流
* **衡量**  — 帐户和列表级别的洞察、帐户参与度得分以及管道和收入影响

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM可用作您的Marketo订阅的附加组件，因此请与您的销售代表联系以实施它。

## [审核记录](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

审核记录提供了Marketo订购中所做更改的全面历史记录。 它将创建用户和管理员之间的责任制，帮助识别意外行为的原因，并提供了解谁在做什么以及何时做什么的安全性。 此信息将在任何时间点提供，并可用于回答以下问题：

* 此资源或设置发生了什么变化，谁最后更新了它？
* 用户X的近期活动是怎样的？
* 谁正在登录我们的帐户？

![](assets/audit-trail.png)

## [Marketo-Vibes SMS LaunchPoint集成](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md) {#marketo-vibes-sms-launchpoint-integration}

直接在Marketo中轻松创建短信消息。 使用丰富的Marketo数据个性化和定向消息，并使用SMS消息仪表板轻松监控其性能。

>[!NOTE]
>
>此功能要求您拥有现有的Vibes SMS帐户。

![](assets/vibes-sms2.png)

## [Email 2.0增强](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**模块级变量**

以前，在Email 2.0模板中指定的所有变量在范围中均为“全局”。 在模块中使用变量时，如果您计划使用模块的多个实例，则并不总是希望这样做。 在此版本中，现在可以将变量指定为“模块级别”，这样可让您指示用户应能够为其使用的每个模块设置唯一值。

![](assets/module-level-variables.png)

**语法更新**

* 现在，您可以在Email 2.0模板中指定的模块上使用“mktoAddByDefault”，以指示默认情况下应在新电子邮件中显示哪些模块。 如果您要构建包含大量模块的电子邮件模板，这会方便得多。
* 在图像元素上，您现在可以指定基础 `<img>` HTML元素的“height”和“width”属性应该对最终用户进行锁定或编辑。 mktoLockImgSize=&quot;true&quot;将导致高度/宽度被锁定（即使图像已更改）。 同样，mktoLockImgStyle=&quot;true&quot;将导致锁定&quot;style&quot;属性。

**代码搜索**

使用新的搜索功能高效地查找和替换电子邮件代码中的内容。 电子邮件模板编辑器中也提供了此功能。

![](assets/2nd-screenshot.png)

**图像元素中的令牌支持**

令牌现在可用于插入图像体验的“外部URL”区域！ 如果您已指定图像 `{{my.tokens}}`中，您现在可以在电子邮件编辑器2.0中引用这些令牌。请注意，在电子邮件编辑器2.0画布中，图像仍显示为已损坏。 但是，在发送电子邮件之前，您会在预览和发送示例中看到这些幻灯片。

## 多个品牌化域 {#multiple-branding-domains}

电子邮件跟踪链接只能使用单个品牌域进行标记的日子已经一去不复返了。 您现在可以添加多个品牌域来激发消费者的信心，创建更加简化的外观以重点关注品牌，改进电子邮件投放能力，并根据每封电子邮件选择用于每封电子邮件的跟踪链接的品牌域。

![](assets/multiple-branding-domains.png)

## [项目令牌](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

我们为项目创建了新令牌类型。 您现在可以在资源和智能营销活动流程步骤中呈现项目名称、描述和ID。

![](assets/program-tokens.png)

## [企业密钥](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

要求您的销售团队中的每个人安装我们的Sales Insight Plugin for Outlook可能会非常繁琐。 我们引入了一种使用企业密钥远程安装Outlook插件的新方法。 向IT团队发送您在“管理员”的“Marketo销售分析”部分找到的唯一密钥，然后让他们完成其余工作。

![](assets/enterprise-key.png)

## [Web个性化营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

指定Web营销活动在您的网站上做出反应的时间延迟。

![](assets/dialog-campaign-delay.png)

## [Content Analytics和Recommendations导出](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

脱机查看内容分析和推荐数据。

## [电子邮件编辑器2.0的API支持](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

以前仅与v1.0电子邮件和模板兼容的预先存在的Asset API现在为v2.0电子邮件资产启用。

## [Marketo开发人员网站](https://developers.marketo.com/) {#marketo-developers-site}

新增功能和改进功能！

## [隐私设置](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

营销人员可以使用隐私设置确定是否使用Munchkin和Web个性化功能跟踪访客。 跟踪级别可通过使用浏览器的Do Not Track设置、选择退出Cookie或非特定IP来控制。 这些方法可能会影响Marketo在特定领域中的价值和功能，但是，如果营销人员不更改任何内容，则Marketo功能将保持不变。

该功能将在六周后逐步向客户发布。 如果您需要立即获取帮助，请联系Marketo支持部门。

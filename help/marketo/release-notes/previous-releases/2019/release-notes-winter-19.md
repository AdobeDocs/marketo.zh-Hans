---
unique-page-id: 17727823
description: 发行说明 — 2019年冬季 — Marketo文档 — 产品文档
title: 发行说明 — 2019年冬季
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# 发行说明： 2019年冬季 {#release-notes-winter}

2019年冬季版本中包含以下功能。 查看Marketo版本以了解功能可用性。

请单击标题链接以查看每个功能的详细文章（如果可用）。

>[!NOTE]
>
>facebook现在需要Business Manager帐户才能利用您的自定义受众集成。 您的Facebook LaunchPoint服务 *必须* 与Business Manager帐户相关联或 **2019年1月14日之后，您的集成将不再有效**. 要设置业务经理帐户，请参阅 [facebook帮助](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft正在推动所有在线客户升级到Microsoft Dynamics的最新版本。 如果您要将Marketo实例与Dynamics Online集成，则需要 [升级到最新版本的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) 早于 **2019年1月31** 以确保您的集成能够继续工作。

>[!NOTE]
>
>Marketo正在将GoToWebinar的OAuth版本从1.0升级到2.0。对OAuth 1.0的支持将于2019年1月被弃用。 如果您是GoTo网络研讨会客户，则需要通过以下方式重新验证通过LaunchPoint的登录（在“管理”区域中） **2019年1月31** 以确保您的集成能够继续工作。 有关更多详情，请参阅我们的 [社区页面](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## 核心平台增强功能 {#core-platform-enhancements}

**[Marketo电子邮件的电子邮件抄送](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

在通过Marketo发送的电子邮件中，每个收件人最多包含五个抄送地址。

**API**

* **资产API的多品牌域支持：** 批准和克隆资产会在API和UI中产生相同的结果。
* **资产API的电子邮件抄送支持**：用户通过API克隆、批准和处理电子邮件将保持与UI设置的对等性。

**[Munchkin v155（测试版）](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **仅API模式**：用户现在可以通过允许单页Web应用程序在要记录网页访问时显式调用，而不是依赖Marketo的自动跟踪，来确定何时以及如何跟踪其数据库的成员。
* **选择退出管理**：通过将选择退出Cookie域与Munchkin跟踪Cookie域进行匹配，轻松管理选择退出。
* **域级决策程序参数**：两个字母的域(即&quot; [website.io](https://website.io)&quot;)将自动在Marketo中跟踪，而无需其他设置要求。

## Marketo Sales Engage {#marketo-sales-engage}

* **Salesforce自定义配置文件**：Sales Engage现在支持无限量的自定义用户档案。

* **Salesforce自定义**：通过删除非关键自定义活动字段，用户可以更高效地在CRM平台中设置Sales Engage 。
* **电子邮件服务**：通过连接到Microsoft Outlook（通过Office365或通过“电子邮件连接”选项卡内部部署），享受更好的可投放性，以及改进的回复跟踪、计划电子邮件功能和批量电子邮件功能。
* **新的管理员设置**：添加了两个管理员页面以优化Sales Engage实例

   * _团队管理_ 通过允许管理员编辑订阅和团队，支持无缝的帐户设置过程。
   * _Salesforce管理设置_ 帮助团队以前所未有的速度更轻松地设置SFDC同步。

* **适用于Windows的OWA插件**：通过一个加载项，所有Windows Office365客户端都将在Sales Engage中受支持，从而能够在Outlook中使用Live Feed。 新的插件将显示在Microsoft Store中。
* **活动推送程序**：将Sales Engage同步到核心Marketo平台，以利用实时营销见解。

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Sky的释放更加频繁。 以下功能和增强功能预计将在第4季度末/第1季度初发布。 有关更多详细信息和更新，请查看我们的 [Sky文档](https://help.marketo.com/).

* **可选默认体验**：如果管理员为Marketo用户提供了访问权限，则他们可能会将Marketo Sky设置为默认体验。

* **重新构思我的Marketo**：通过添加小组件来自定义您的体验，这些小组件提供关键信息、通知和最常访问区域的链接。

* **Design Studio列表视图和详细信息页面**：利用电子邮件、登陆页面和表单的可过滤和可搜索列表视图，体验更高级别的组织和准确性。 资产详细信息页面提供有关每个资产的关键信息，包括资产使用哪些程序、使用的代码片段数量等等。

* **全局搜索**：Marketo现在可以在整个平台上提供更快、更强大的全局搜索功能。 现在，搜索查询可在所有可访问的工作区中运行，并且可以搜索资产（活动和已存档）、标签、营销活动和项目。 搜索结果通过叠加提供，每个结果都包括其文件位置跟踪，以指定资产所处的位置。

* **改进了用户界面**：新的图标、模式和按钮，以及新的调色板，以反映我们的品牌更新，并使Marketo Sky更令人惊叹且功能更强大。

* **电子邮件计划可用性增强**：我们继续朝着经典的Marketo商机管理平台和新的Marketo Sky体验之间的电子邮件计划功能对等方向发展。
* **带网络研讨会的活动**：Marketo Sky现在提供事件网络研讨会程序（注意：此版本仅支持GoToWebinar，并且会随着时间的推移建立进一步的集成）。

## Account-Based Marketing {#account-based-marketing}

**[ABM基于角色的分段和过滤](/help/marketo/product-docs/target-account-management/using-personas.md)**

为指定帐户中的特定角色个性化ABM营销活动。 ABM角色功能基于潜在客户细分创建默认职务，并允许配置其他角色分段。

## Analytics {#analytics}

**Bizible**

* **自定义计算字段**：使用任何Bizible属性构建可用于功能板报告和分段的自定义字段。

* **SOC II Type II认证**：新的安全和隐私认证以今年早些时候的I类认证为基础。

## Web个性化 {#web-personalization}

**[在帐户设置中添加子域](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

为了更高效地管理域和子域，用户现在可以将子域添加到其RTP帐户设置中。

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**更新了适用于Android的MME软件开发工具包(SDK)**

我们更新了适用于Android的SDK，使其成为更现代、更稳定且可扩展的框架，其中包含更多灵活性和新的工程功能。 Android应用程序开发人员现在可以直接使用Google的 [Firebase云消息](https://firebase.google.com/docs/cloud-messaging/) (FCM)集成了此新SDK。

* [开发人员说明](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [开发人员常见问题解答](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>应用程序开发人员 **必须** 在2019年3月31日之前更新到新版本。 如果您在2019年3月31日之前未更新您的SDK，则在此日期之后下载您的应用程序的任何新用户都将无法接收推送通知，直到您更新到最新版本的SDK。 SDK更新将不需要您当前现有的移动应用程序用户重新下载应用程序的新版本。

## 其他更新 {#additional-updates}

**可扩展网络研讨会平台**

除了我们的产品发布之外，我们的合作伙伴团队还正在努力研究一个新框架，该框架允许网络研讨会提供商构建并维护他们与Marketo的集成，从而提供更大的灵活性来更新和增强其解决方案，同时使营销人员能够充分利用他们选择的集成。

我们计划根据具体情况，向供应商推出我们的新平台。 欲知更多信息，请参阅我们的 [项目群详细信息](https://www.marketo.com/why-marketo/partners/technology/) 或联系您的Marketo联系人。

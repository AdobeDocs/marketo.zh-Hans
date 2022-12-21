---
unique-page-id: 17727823
description: 发行说明 — 2019年冬季 — Marketo文档 — 产品文档
title: 发行说明 — 2019年冬季
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# 发行说明：’19年冬 {#release-notes-winter}

’19年冬季版本中包含以下功能。 查看您的Marketo版本以了解功能的可用性。

请单击标题链接，以查看每项功能的详细文章（如果可用）。

>[!NOTE]
>
>Facebook现在需要Business Manager帐户才能利用您的自定义受众集成。 您的Facebook LaunchPoint服务 *必须* 与业务经理帐户或 **2019年1月14日后，您的集成将不再有效**. 要设置业务经理帐户，请参阅 [Facebook帮助](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft正在推动所有在线客户升级到最新版的Microsoft Dynamics。 如果您要将Marketo实例与Dynamics Online集成，则需要 [升级到最新版本的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) 之前 **2019年1月31日** 以确保您的集成可以继续运行。

>[!NOTE]
>
>Marketo正在将GoToWebinar的OAuth版本从1.0升级到2.0。2019年1月将弃用对OAuth 1.0的支持。 如果您是GoTo网络研讨会客户，则需要通过LaunchPoint（在“管理员”区域）重新验证登录身份，方法是 **2019年1月31日** 以确保您的集成可以继续运行。 有关更多详细信息，请参阅 [社区页面](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## 核心平台增强功能 {#core-platform-enhancements}

**[电子邮件CC(Marketo电子邮件)](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

对于通过Marketo发送的电子邮件，每个收件人最多包含五个CC地址。

**API**

* **资产API的多品牌域支持：** 批准和克隆资产会在API和UI中产生相同的结果。
* **对资产API的电子邮件抄送支持**:通过API克隆、批准和处理电子邮件的用户将保持与UI设置的对等性。

**[Munchkin v155（Beta版）](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **仅限API模式**:用户现在可以确定何时以及如何跟踪其数据库成员，方法是允许单页Web应用程序在他们要记录网页访问时明确调用，而不是依赖Marketo的自动跟踪。
* **选择退出管理**:通过将选择退出Cookie域与Munchkin跟踪Cookie域相匹配，轻松管理选择退出。
* **域级决策器参数**:双字母域(即&quot; [website.io](https://website.io)“)将在Marketo中自动跟踪，而无需其他设置要求。

## Marketo Sales Engage {#marketo-sales-engage}

* **Salesforce自定义用户档案**:Sales Engage现在支持无限量的自定义用户档案。

* **Salesforce自定义**:通过删除非关键的自定义活动字段，用户可以更高效地设置Sales Engage in the CRM platform。
* **电子邮件服务**:通过连接到Microsoft Outlook（通过Office365或通过“电子邮件连接”选项卡进行内部部署），可享受更好的投放能力以及改进的回复跟踪、计划电子邮件功能和批量电子邮件功能。
* **新管理员设置**:添加了两个管理页面以优化您的销售参与实例

   * _团队管理_ 允许管理员编辑订阅和团队，从而支持无缝的帐户设置流程。
   * _Salesforce管理设置_ 帮助团队以比以往更快、更轻松的速度设置其SFDC同步。

* **适用于Windows的OWA插件**:通过单个插件，Sales Engage将支持所有Windows Office365客户端，从而提供在Outlook中使用实时信息源的功能。 新插件将在Microsoft应用商店中提供。
* **活动推动者**:将销售参与同步到核心Marketo平台，以利用实时营销分析。

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Sky发布的频率更高。 预计第4季度末/第1季度初将发布以下功能和增强功能。 有关更多详细信息和更新，请查看 [天空文档](https://help.marketo.com/).

* **可选的默认体验**:Marketo用户如果已由管理员提供访问权限，则可以将Marketo Sky设置为其默认体验。

* **重新想象我的Marketo**:通过添加小组件来自定义您的体验，这些小组件提供关键信息、通知以及指向您最常访问区域的链接。

* **Design Studio列表视图和详细信息页面**:通过可过滤和可搜索的电子邮件、登陆页面和表单列表视图，享受更高的组织级别和准确性。 资产详细信息页面提供有关每个资产的关键信息，包括资产使用的程序、使用的代码片段数等。

* **全局搜索**:Marketo现在提供了更快、更强大的全局搜索功能。 搜索查询现在可以跨所有可访问的工作区运行，并可以搜索资产（活动和已存档）、标签、促销活动和项目。 搜索结果通过叠加提供，每个结果都包括其文件位置跟踪，以指定资产的居住位置。

* **改进的用户界面**:新的图标、模型和按钮，以及新的调色板，可反映我们的品牌刷新，使Marketo Sky更加美观和实用。

* **电子邮件计划可用性增强**:我们将继续在经典的Marketo潜在客户管理平台与新的Marketo Sky体验之间实现电子邮件计划功能的均等。
* **包含活动的网络研讨会计划**:现在，可以在Marketo Sky中使用包含活动的网络研讨会计划(注意：此版本中仅支持GoTo网络研讨会，并会随着时间的推移建立更多集成)。

## Account-Based Marketing {#account-based-marketing}

**[基于ABM角色的分段和过滤](/help/marketo/product-docs/target-account-management/using-personas.md)**

为指定帐户中的特定角色个性化您的ABM营销活动。 “ABM角色”功能基于潜在客户分段创建默认的工作标题，并允许配置其他角色分段。

## Analytics {#analytics}

**Bizible**

* **自定义计算字段**:使用任何Bizible属性来构建可用于功能板报告和分段的自定义字段。

* **SOC II类认证**:新的安全和隐私认证建立在今年早些时候的I类认证基础之上。

## Web个性化 {#web-personalization}

**[在帐户设置中添加子域](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

为了更有效地管理域和子域，用户现在可以将子域添加到其RTP帐户设置中。

## Marketo Mobile Engagement(MME) {#marketo-mobile-engagement-mme}

**更新了适用于Android的MME软件开发工具包(SDK)**

我们已将适用于Android的SDK更新为更现代、更稳定、更可扩展的框架，该框架包含更多灵活性和新的工程功能。 Android应用程序开发人员现在可以直接使用Google [Firebase Cloud消息传送](https://firebase.google.com/docs/cloud-messaging/) (FCM)与此新SDK一起使用。

* [开发人员说明](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [开发人员常见问题解答](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>应用程序开发人员 **必须** 于2019年3月31日之前更新到新版本。 如果您在2019年3月31日之前未更新SDK，则在此日期之后下载您应用程序的任何新用户将无法接收推送通知，直到您更新到最新版本的SDK为止。 SDK更新将不需要您当前的移动设备应用程序用户重新下载您应用程序的新版本。

## 其他更新 {#additional-updates}

**可扩展网络研讨会平台**

除了我们的产品版本之外，我们的合作伙伴团队还在努力构建一个新框架，该框架允许网络研讨会提供商自行构建并维护与Marketo的集成，从而在更新和增强其解决方案方面提供更大的灵活性，同时让营销人员能够充分利用他们选择的集成。

我们计划与提供商一起逐个案例推出新平台。 有关更多信息，请参阅 [项目详细信息](https://www.marketo.com/why-marketo/partners/technology/) 或联系您的Marketo联系人。

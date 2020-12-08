---
unique-page-id: 17727823
description: 发行说明-Winter '19 - Marketo Docs —— 产品文档
title: 发行说明- 19年冬季
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---


# 发行说明：19年冬季 {#release-notes-winter}

1919年冬季版包含以下功能。 检查您的Marketo版本以了解功能可用性。

请单击标题链接，以视图每个功能的详细文章（如果有）。

>[!NOTE]
>
>Facebook现在需要一个业务经理帐户，以利用您的自定义受众集成。 您的Facebook LaunchPoint *服务必须* 与业务经理帐户关 **联，否则您的集成在2019年1月14日之后将不再有效**。 要设置业务经理帐户，请参阅Facebook [帮助](https://www.facebook.com/business/help/1710077379203657)。

>[!NOTE]
>
>Microsoft正在推动所有在线客户升级到最新版Microsoft Dynamics。 如果您要将Marketo实例与Dynamics Online集成，您需 [要在2019年1月31日之前升级到Marketo](../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md)**解决方案的最新版本** ，以确保您的集成能继续工作。

>[!NOTE]
>
>Marketo正在将GoToWebinar的OAuth版本从1.0升级到2.0。对OAuth 1.0的支持将在2019年1月弃用。 如果您是GoToWebinar客户，您需要在2019年1月31日之前通过LaunchPoint(在“管理” **区域)重新验证登录** ，以确保您的集成能继续工作。 有关详细信息，请参阅我们的 [社区页面](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019)。

## 核心平台增强功能 {#core-platform-enhancements}

**面向 [营销人员的电子邮件](../../product-docs/email-marketing/general/email-cc.md)CC**

对于通过Marketo发送的电子邮件，每个收件人最多可包含五个CC地址。

**API**

* **资产API的多品牌域支持：** 批准和克隆资产会在API和UI中产生相同的结果。
* **针对资产API的电子邮件CC支持**:用户通过API仿制、批准和处理电子邮件将保持与UI设置的对等性。

** [Munchkin v155（测试版）](http://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **仅API模式**:用户现在可以决定何时以及如何跟踪其数据库成员，方法是允许单页Web应用程序在他们希望记录网页访问时明确调用，而不是依赖Marketo的自动跟踪。
* **退出管理**:通过将退出Cookie域与Munchkin跟踪Cookie域进行匹配，轻松管理退出。
* **域级决策器参数**:双字母域(即“ [website.io](http://website.io)”)将在Marketo中自动跟踪，无需其他设置要求。

## 营销人员参与销售 {#marketo-sales-engage}

* **Salesforce自定义用户档案**:Sales Engage现在支持无限制的自定义用户档案。

* **Salesforce自定义**:通过删除非关键的自定义活动字段，用户可以更高效地设置CRM平台中的销售参与。
* **电子邮件服务**:通过连接到Microsoft Outlook（通过Office365或通过“电子邮件连接”选项卡进行预检），享受更好的交付能力以及改进的回复跟踪、定时电子邮件功能和批量电子邮件功能。
* **新管理员设置**:添加了两个管理页面以优化您的销售参与实例

   * *团队管理* 通过允许管理员编辑订阅和团队，支持无缝的帐户设置流程。
   * *Salesforce管理设置* 帮助团队比以往更快、更轻松地设置其SFDC同步。

* **适用于Windows的OWA插件**:只需一个插件，Sales Engage中将支持所有Windows Office365客户端，从而提供在Outlook中使用实时源的功能。 新插件将在Microsoft商店中可用。
* **活动推动者**:将销售参与同步到核心营销平台，以利用实时营销洞察。

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Sky释放以更频繁的节奏进行。 预计在第4季度末／第1季度初发布以下功能和增强功能。 有关更多详细信息和更新，请查 [看Sky文档](https://help.marketo.com/hc/en-us/articles/360012858573)。

* **可选默认体验**:Marketo用户如果已由管理员提供访问权限，则可以将Marketo Sky设置为其默认体验。

* **重塑了我的营销**:通过添加构件来自定义您的体验，这些构件提供关键信息、通知和指向最常访问区域的链接。

* **Design Studio列表视图和详细页**:利用可填写和可搜索的列表视图电子邮件、登陆页和表单，享受更高的组织级别和准确性。 资产详细信息页面提供每个资产的关键信息，包括资产使用的项目、使用的片段数等。

* **全局搜索**:Marketo现在可以跨平台优惠更快、更强大的全局搜索功能。 搜索查询现在可在所有可访问的工作区中运行，并可以搜索资产（活动和归档）、标签、活动和项目。 搜索结果通过叠加提供，并且每个结果都包括其文件位置跟踪，以指定资产所在的位置。

* **改进的用户界面**:新的图标、模型和按钮，以及新的调色板，可反映我们的品牌更新并使Marketo Sky更出色、更实用。

* **电子邮件项目可用性增强**:我们继续在经典的营销人员潜在客户管理平台和新的项目体验之间实现电子邮件Marketo Sky功能的均等。
* **事件网络研讨会项目**:事件在线研讨会项目现在以Marketo Sky形式提供(注意：此版本将仅支持GoToWebinar，并随时间推移进一步建立集成)。

## 基于帐户的营销 {#account-based-marketing}

**基 [于ABM人物的细分和过滤](../../product-docs/account-based-marketing/using-personas.md)**

为指定帐户中的特定角色个性化您的ABM活动。 “ABM人物”功能基于潜在客户细分创建默认职务，并允许配置其他人物细分。

## 分析 {#analytics}

**Bizbile**

* **自定义计算字段**:使用任何Bizible属性构建可用于仪表板报告和分段的自定义字段。

* **SOC II类II认证**:新的安全性和隐私认证基于今年早些时候的I型认证。

## Web个性化 {#web-personalization}

**[在帐户设置中添加子域](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

为了更高效地管理域和子域，用户现在可以将子域添加到其RTP帐户设置中。

## Marketo Mobile Engagement(MME) {#marketo-mobile-engagement-mme}

**更新了适用于Android的MME软件开发工具包(SDK)**

我们已将Android的SDK更新为更新、更稳定、可伸缩的框架，其中包含更多灵活性和新的工程功能。 Android应用程序开发人员现在可以将Google的 [Firebase Cloud Messaging](http://firebase.google.com/docs/cloud-messaging/) (FCM)与此新SDK一起直接使用。

* [开发人员说明](http://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [开发人员常见问题解答](http://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>应用程 **序开发** 人员必须在2019年3月31日之前更新至新版本。 如果您在2019年3月31日之前未更新您的SDK，则在此日期后下载您的应用程序的任何新用户将无法收到推送通知，除非您更新到最新版本的SDK。 SDK更新将不要求您当前的移动应用程序用户重新下载您的应用程序的新版本。

## 其他更新 {#additional-updates}

**可扩展的网络研讨会平台**

除了我们的产品版本，我们的合作伙伴团队还在开发一个新框架，允许网络研讨会提供商构建和维护与Marketo的集成，在更新和增强解决方案方面提供更大的灵活性，同时使营销人员能够充分利用他们选择的集成。

我们计划与提供商一起逐个案例推出我们的新平台。 有关详细信息，请参阅我们 [的项目详](https://www.marketo.com/why-marketo/partners/technology/) 细信息或联系您的营销人员联系。

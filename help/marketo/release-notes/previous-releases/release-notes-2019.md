---
title: 2019
description: 2019 - Marketo文档 — 产品文档
feature: Release Information
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
  - id: de9e3aa9-f002-4fe1-897b-09ee3c55114b
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
  - id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: bbbea26f-9621-49eb-9ab8-e06fb3bbce8c
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 1e70b9383bf3a1cd30715df4379d440c4efb1abd
workflow-type: tm+mt
source-wordcount: 2528
ht-degree: 0%

---

# 2019

## 2019年冬 {#winter}

’19年冬季版本包括以下功能。 检查您的Marketo版本以了解功能可用性。

请单击标题链接以查看每个功能的详细文章（如果可用）。

>[!NOTE]
>
>[!DNL Facebook]现在需要Business Manager帐户才能利用您的自定义受众集成。 您的[!DNL Facebook] LaunchPoint服务&#x200B;*必须*&#x200B;与Business Manager帐户关联，或者&#x200B;**您的集成在2019年1月14日之后将不再有效**。 若要设置Business Manager帐户，请参阅[[!DNL Facebook] 帮助](https://www.facebook.com/business/help/1710077379203657)。

>[!NOTE]
>
>Microsoft正在推送所有在线客户升级到[!DNL Microsoft Dynamics]的最新版本。 如果您正在将Marketo实例与[!DNL Dynamics Online]集成，则需要在&#x200B;**2019年1月31日**&#x200B;之前[升级到Marketo解决方案的最新版本](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)，以确保您的集成能够继续工作。

>[!NOTE]
>
>Marketo正在将GoToWebinar的OAuth版本从1.0升级到2.0。 对OAuth 1.0的支持将于2019年1月弃用。 如果您是GoTo网络研讨会客户，则需要在&#x200B;**2019年1月31日**&#x200B;之前通过LaunchPoint（在管理区域）重新验证您的登录，以确保您的集成继续工作。 有关详细信息，请参阅我们的[社区页面](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019)。

## 核心平台增强功能

**[电子邮件抄送Marketo电子邮件](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

在通过Marketo发送的电子邮件中，每个收件人最多包含五个抄送地址。

**API**

* **资产API的多品牌域支持：**&#x200B;批准和克隆资产会在API和UI中产生相同的结果。
* **资产API的电子邮件CC支持**：用户通过API克隆、批准和处理电子邮件将保持与UI设置的对等性。

**[[!DNL Munchkin] v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **仅限API模式**：用户现在可以通过允许单页Web应用程序在要记录网页访问时显式调用，而不是依赖Marketo的自动跟踪来确定何时以及如何跟踪其数据库的成员。
* **选择退出管理**：通过将选择退出Cookie域与[!DNL Munchkin]跟踪Cookie域进行匹配，轻松管理选择退出。
* **域级决策器参数**：双字母域（即&quot; [website.io](https://website.io)&quot;）将在Marketo中自动跟踪，无需额外的设置要求。

## Marketo Sales Engage

* **[!DNL Salesforce]自定义配置文件**： Sales Engage现在支持无限自定义配置文件。

* **[!DNL Salesforce]自定义**：通过删除非关键自定义活动字段，用户可以更高效地在CRM平台上设置Sales Engage。
* **电子邮件服务**：通过连接到[!DNL Microsoft Outlook]（通过Office365或通过“电子邮件连接”选项卡内部部署）享受更好的可投放性，以及改进的回复跟踪、计划的电子邮件功能和批量电子邮件功能。
* **新管理员设置**：添加了两个管理员页面，以优化您的Sales Engage实例

   * 通过允许管理员编辑订阅和团队，*团队管理*&#x200B;支持无缝的帐户设置过程。
   * *Salesforce管理设置*&#x200B;可帮助团队以前所未有的速度更轻松地设置SFDC同步。

* 适用于&#x200B;[!DNL Windows]&#x200B;**的** OWA插件：通过一个加载项，Sales Engage将支持所有[!DNL Windows Office365]客户端，从而能够在Outlook中使用Live Feed。 新的插件将显示在Microsoft Store中。
* **活动推送器**：将Sales Engage同步到核心Marketo平台，以利用实时营销见解。

## [!DNL Marketo Sky]

>[!NOTE]
>
>[!DNL Marketo Sky]版本发布的频率更高。 以下功能和增强功能预计将在第四季度末/第一季度初发布。 有关更多详细信息和更新，请查看我们的[Sky文档](https://help.marketo.com/)。

* **可选默认体验**：如果管理员向他们提供了访问权限，Marketo用户可以将[!DNL Marketo Sky]设置为其默认体验。

* **重新想像我的Marketo**：通过添加小组件自定义您的体验，这些小组件提供关键信息、通知以及您最常访问区域的链接。

* **Design Studio列表视图和详细信息页面**：利用电子邮件、登陆页面和表单的可过滤和可搜索列表视图，享受更高的组织和准确性级别。 资产详细信息页面提供有关每个资产的关键信息，包括资产使用的程序、使用的代码片段数量等等。

* **全局搜索**：Marketo现在可以在整个平台上提供更快、更可靠的全局搜索功能。 现在，搜索查询可在所有可访问的工作区中运行，并且可以搜索资产（活动和已存档）、标签、营销活动和项目。 搜索结果通过叠加提供，每个结果都包括其文件位置跟踪，以指定资产所在的位置。

* **改进的用户界面**：新增图标、模式和按钮，以及新的调色板，以反映我们的品牌更新并使[!DNL Marketo Sky]更加令人惊叹和功能更强。

* **电子邮件计划可用性增强功能**：我们将继续在经典的Marketo潜在客户管理平台和新的[!DNL Marketo Sky]体验之间实现电子邮件计划功能的对等性。
* **网络研讨会计划**： [!DNL Marketo Sky]中现在提供网络研讨会活动计划（注意：此版本仅支持GoToWebinar，并且会随着时间的推移建立进一步的集成）。

## Account-Based Marketing

**[ABM基于角色的分段和筛选](/help/marketo/product-docs/target-account-management/using-personas.md)**

为指定帐户中的特定角色个性化ABM活动。 ABM角色功能基于潜在客户细分创建默认职务，并允许配置其他角色分段。

## Analytics {#analytics}

**[!DNL Bizible]**

* **自定义计算字段**：使用任何[!DNL Bizible]属性构建可用于仪表板报告和分段的自定义字段。

* **SOC II Type II认证**：新的安全和隐私认证以今年早些时候的Type I认证为基础。

## [!DNL Web Personalization] {#web-personalization}

**[在帐户设置中添加子域](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

为了更有效地管理域和子域，用户现在可以将子域添加到其RTP帐户设置中。

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**已更新Android的MME软件开发工具包(SDK)**

我们已将适用于Android的SDK更新为更现代、更稳定和可扩展的框架，其中包含了更多灵活性和新的工程功能。 Android应用程序开发人员现在可以直接将Google的[Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM)与此新的SDK结合使用。

* [开发人员说明](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [开发人员常见问题解答](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>应用程序开发人员&#x200B;**必须**&#x200B;在2019年3月31日之前更新到新版本。 如果您没有在2019年3月31日之前更新SDK，则在此日期之后下载您的应用程序的任何新用户都将无法接收推送通知，直到您更新到最新版本的SDK。 SDK更新将不需要您当前的移动应用程序用户重新下载应用程序的新版本。

## 其他更新 {#additional-updates}

**可扩展网络研讨会平台**

除了我们的产品发布之外，我们的合作伙伴团队还正在研究一个新的框架，该框架允许网络研讨会提供商构建并维护他们与Marketo的集成，在更新和增强其解决方案方面提供更大的灵活性，同时使营销人员能够充分利用他们所选的集成。

我们计划根据具体情况，向供应商推出我们的新平台。 有关详细信息，请参阅我们的[计划详细信息](https://www.marketo.com/why-marketo/partners/technology/)或联系您的Marketo联系人。

## 2019年春 {#spring}

2019年春季发行版中包含以下功能。 检查您的Marketo版本以了解功能可用性。

请单击标题链接以查看每个功能的详细文章（如果可用）。

***季度发行版_**

以下功能于2019年3月15日发布。

## 核心平台增强功能

* **轮候：**&#x200B;轮候成员的新程序/事件状态，在您想[将其置于保留状态](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)直到空缺打开为止。 这适用于Marketo Classic中与“事件”计划关联的渠道，以及[!DNL Marketo Sky]中与“事件”和“事件”相关的网络研讨会计划。 默认情况下，“轮候”具有与“已注册”相同的步骤值。
* **[自定义通信限制](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md)**：管理员现在可以设置自定义每日或每周通信限制。
* **[Smart Campaign Asset API](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**：通过按更新的日期和ID检索智能营销活动记录，扩充您在Marketo之外的分析。
* **电子邮件的HTTPS跟踪链接：**&#x200B;对于已购买“跟踪链接的安全域”的客户，品牌跟踪链接现在可以作为HTTPS显示在您的电子邮件中。
* **电子邮件可投放性Powerpack更新**：能够标记和评论特定测试结果，通过URL与利益相关者共享结果，以及跟踪更改以查看在利益相关者编辑内容时电子邮件的演变。

Account-Based Marketing

**[AccountAI](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md)**&#x200B;现已正式可用。 AccountAI使用人工智能揭示您应针对ABM策略定向的帐户。

<br> 

**_非季度发行_**

预计将在整个日历季度并在2019年第二季度初发布以下功能。

## [!DNL Marketo Sky]

* **完整的电子邮件计划功能**：发送电子邮件、创建A/B测试并跟踪结果，从而提供用户友好的体验。
* **智能营销活动功能**：在新的用户界面中享受增强的稳定性，因为智能营销活动功能在Sky中继续推出。
* **管理Design Studio Assets**：添加了从Design Studio列表视图批量管理模板、图像、Forms、代码片段、文件、电子邮件和登陆页面的功能。
* **在收件人时区投放，仪表板**：了解客户对使用Sky中的在收件人时区投放，功能发送的电子邮件的报告行为。

## Marketo Sales Engage

* **增强审核**：在实例中新增了对所有人员、电子邮件和[内容的可见性](/help/marketo/product-docs/marketo-sales-connect/templates/view-template-list-as-another-user.md)，该实例添加了由其他用户创建的[结束现有营销活动](/help/marketo/product-docs/marketo-sales-connect/campaigns/view-campaigns-list-as-another-user.md)的功能。
* **[取消订阅管理](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md)**：通过[阻止电子邮件域](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md)的联系功能，最大限度地提高可投放性和合规性。 Marketo还将在发送电子邮件之前交叉引用潜在客户数据库以取消订阅。

## Marketo的[!DNL Bizible]

* **[!DNL Bizible]发现功能增强**：新的功能板分段功能使营销人员能够更好地了解性能。
* **多货币支持**：通过[!DNL Bizible]基于CRM货币表构建的新自动货币兑换功能，在您的公司货币和任何本地货币之间切换。
* **CRM Campaign成本**：能够从CRM营销活动对象自动提取成本数据，从而衡量离线营销活动的支出和ROI。

## 2019 年 6 月 {#june}

2019年6月版本中包含以下功能。 检查您的Marketo版本以了解功能可用性。

**_季度发布_**

以下功能于2019年6月14日发布。

## Marketo核心服务 {#marketo-core-services}

* **批量提取文件校验和**：通过比较文件哈希和已完成提取作业的校验和字符串，验证是否检索到了完整文件。
* **从Email 1.0自动迁移到Email 2.0**： Email 2.0与Email 1.0电子邮件和模板完全兼容。 享受新功能，例如对内容元素（图像、文本等）进行分组的功能 在模块中，在模板中定义字符串、颜色、图像等变量，并利用完全响应的入门级模板。 还包括一个可视电子邮件模板选取器。

>[!CAUTION]
>
>自2019年6月18日起，Email 1.0不再可用。 您可以在[此处](https://nation.marketo.com/docs/DOC-7038)了解有关Email 2.0和Email 1.0弃用的更多信息。

## Account-Based Marketing

* **[!DNL LinkedIn]帐户匹配(BETA)** ：现已推出测试版中的新ABM功能，通过该功能，您可以直接从Marketo将已知和空白帐户列表发送到LinkedIn。 此功能自动包含在所有Marketo ABM客户中。

<br> 

**_在整个季度中发布_**

预计将在整个日历季度以及2019年第三季度初发布以下功能。

## [!DNL Marketo Sky]

* **事件上限**&#x200B;和&#x200B;**事件目标**&#x200B;通常在[!DNL Marketo Sky]的Premium Events加载项下提供。

   * 事件上限：通过注册上限、页面重定向和轮候表功能优化活动和网络研讨会的客户体验。
   * 活动目标：设置活动注册和出勤目标并实时跟踪进度。

* **完整导航链接**：我们已启用导航到所有许可应用程序，如Hootsuite、Calendar等。
* **电子邮件、登录页、代码片段、表单、图像和文件列表视图**：在Design Studio中查看、搜索您的任何资产并对其执行批量操作。
* **图像、文件和代码片段详细信息页面**：使用诸如&#x200B;_创建于/由_&#x200B;创建的元数据以及诸如&#x200B;_删除_&#x200B;和&#x200B;_批准_&#x200B;之类的操作，获取有关您的资源的快速详细信息。
* **社区博客帖子小组件**：访问“我的Marketo”中的社区最近发布的帖子。
* **即将过期的构件**：将“即将过期”构件添加到您的“我的Marketo”仪表板，以查看哪些营销活动和登陆页面将下周过期。
* **更多智能列表信息卡**：使用其他智能列表信息卡（包括“创建任务”流程步骤、CRM智能列表规则等）适当地划分和目标区段。
* **电子邮件冠军/挑战者详细信息页面**：查看您的电子邮件冠军/挑战者测试中的获胜标准、创建时间等数据。

## Marketo [!DNL Sales Connect] {#marketo-sales-connect}

* 在[!DNL Salesforce]自定义项中执行&#x200B;**批量操作**：通过发送电子邮件和通过[!DNL Salesforce]自定义项将联系人批量添加到营销活动，最大限度地提高工作效率。
* **设置 — “管理员和非管理员”的[!DNL Salesforce]页面**：通过与[!DNL Sales Connect]连接的[!DNL Salesforce]实例的清晰视图以及“我的电子邮件至[!DNL Salesforce]更新”来管理您的[!DNL Sales Connect]实例。 未来几个月将发布针对管理员、非管理员和团队范围同步的增强同步设置。
* **设置 — 集成页面**：针对您的所有集成提供一站式服务，以便您能够充分利用我们开放的生态系统。
* **设置 — 配置文件页面**：查看并更新帐户详细信息，更改密码，并在此新的配置文件页面上检查实例的实施状态。

* **系统电子邮件模板**：更新了设计、响应能力和国际化功能。

## Marketo的[!DNL Bizible]

* **对[!DNL Dynamics]**&#x200B;的多货币支持：[!DNL Bizible]现在可适应[!DNL Microsoft Dynamics]货币表，因此您可以轻松地在公司货币和本地货币之间切换。 （注意：对SFDC的支持已于2019年第一季度发布。）
* **漂移集成**：了解漂移对话如何影响客户的历程。 [!DNL Bizible]还将从对话中提取电子邮件地址，以创建新潜在客户或将接触点连接到现有潜在客户。
* **本地化**： [!DNL Bizible]现在提供所有Marketo支持的语言（英语、日语、德语、西班牙语、法语和葡萄牙语）版本。

_&#x200B;**产品发布网络研讨会**&#x200B;_&#x200B;在[此处](https://engage.marketo.com/Marketo-June-Product-Release-2019-On-Demand.html)观看我们2019年6月发布创新网络研讨会的录像。

## 2019年8月 {#august}

2019年8月版本中包含以下功能。 检查您的Marketo版本以了解功能可用性。

**_季度发布_**

以下功能于2019年8月16日发布。

## 核心Marketo Engage {#core-marketo-engage}

* **可扩展的网络研讨会框架**：利用Marketo新的开箱即用网络研讨会框架（在2019年冬季的发行说明中引入）将数据从网络研讨会提供商无缝传递到Marketo，反之亦然，从而节省时间。 现在可在此新框架中使用事件和缩放。
* **Smart Campaign API更新**：在我们完善CRUD（创建、读取、更新、删除）界面时管理Smart Campaign生命周期功能。
* **更新电子邮件标头API更改**：更新电子邮件标头API不再需要电子邮件附加模板来更新标头字段，例如主题行。

**Account-Based Marketing** ![（星级）](assets/yellow-star.png)

* **[!DNL LinkedIn]帐户匹配**（以前为测试版）现已正式可用。
* **AccountAI**&#x200B;正在被正式重新命名为&#x200B;**帐户分析**。

<br> 

**_在整个季度中发布_**

以下功能采用非季度周期，将在整个日历季度以及2019年第4季度初发布。

**[!DNL Marketo Sales Connect]** ![（星形）](assets/yellow-star.png)

* **人员页面布局增强：**&#x200B;通过列表导入和新人员页面布局中的批量操作来管理您的人员和组。

>[!AVAILABILITY]
>
>以星号(![（星号）](assets/yellow-star.png))表示的功能是付费加载项。 请联系您的Marketo代表以了解更多信息。

>[!NOTE]
>
>**TLS 1.0和1.1弃用**：为了符合Adobe的世界级安全标准，我们将从2019年12月13日开始弃用对传输层安全性(TLS) 1.0和1.1的支持。 与Marketo集成的系统如果不符合1.2协议，则可能会失去对Marketo Engage服务的访问权限。
>
>**要保持您的Marketo Engage访问权限，请确保在2019年12月13日之前所有客户端系统都符合TLS 1.2**。 更多详细信息可在[此处](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq)找到。

**_产品发布网络研讨会_** [于8月28日1:00PM PT / 4:00PM ET参加我们](https://engage.marketo.com/August_19_Release_Webinar.html)由我们的产品团队主办的实时网络研讨会，并了解有关此版本中包含的功能的更多信息。


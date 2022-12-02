---
description: 发行说明 — 2021年1月 — Marketo文档 — 产品文档
title: 发行说明 — 2021年1月
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
source-git-commit: 85e04fb8a52a417982014bc4bb101b6044e53f84
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# 发行说明：2021年1月 {#release-notes-jan-21}

’21年1月版中包含以下功能。 查看您的Marketo版本以了解功能的可用性。

>[!AVAILABILITY]
>
>由星(![（星号）](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_**

将在 **2021年1月15日**.

## 新一代用户体验 {#next-generation-user-experience}

* 支持工作区：Marketo Engage的下一代用户体验将Adobe Experience Cloud的外观与体验与生产力创新结合在一起，以帮助营销从业者更快、更智能地工作。 在最新版本中，我们添加了对工作区和分区的完全支持，包括跨工作区共享文件夹的功能。 右侧画布将提供一个切换开关，让您能够在每个功能的旧体验和新体验之间无缝过渡，而不会丢失上下文。 [了解更多](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124) 来自营销国家/地区新一代体验常见问题解答。

## 多渠道个性化 {#multi-channel-personalization}

* **[Adobe Experience Cloud受众同步阶段3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**:现在，现有的Adobe Experience Cloud(AEC)受众同步功能支持从Marketo Engage到其他AEC应用程序(包括Adobe Experience Platform(AEP)产品(如Real-time Customer Data Platform和Adobe Experience Platform Activation)的连续双向B2B受众同步。  在将潜在客户添加到受众区段并将其删除后，Marketo Engage将在连接的AEC应用程序中自动同步更新的受众。 使用它可以在整个AEC技术堆栈中利用Adobe的多渠道编排、重新定位、受众抑制、个性化和报告用例。
* **[连续同步到Google、Facebook和LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**:可以在静态列表上启用与广告网络的连续自动同步，从而随着列表成员资格的改变而更新广告网络，而无需用户干预。
* **[程序成员自定义字段的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**:我们扩展了项目成员自定义字段功能以支持令牌框架。 营销人员可以将项目成员自定义字段令牌插入电子邮件、登陆页、短信消息、推送通知和Web挂钩中。 在促销活动流程操作中使用新令牌来更改数据值、创建任务或关注时刻。

## 登陆页面和Forms {#landing-pages-and-forms}

* **表单API**:从非Marketo表单中提取数据时，可提取潜在客户信息或触发培养型营销活动。 非Marketo表单可以通过REST API与Marketo Engage集成。 新API提供了利用所有相关功能模拟Marketo Engage表单提交的功能。
* **登陆页面API**:使用新的登陆页面预览API简化集成应用程序中的编辑和翻译工作流。 第三方供应商现在无需登录Marketo Engage即可渲染登陆页面的完全个性化预览。  登陆页面预览API支持第三方集成应用程序中的端到端编辑和本地化工作流。

## 电子邮件营销 {#email-marketing}

* **[提高了自定义对象检索限制](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**:电子邮件速度脚本的开发人员可以通过自助覆盖将自定义对象的数量快速增加到100。 营销人员可以通过访问大量第一和第二级自定义对象来提高智能营销活动的有效性。

## Salesforce CRM集成 {#salesforce-crm-integration}

* [Salesforce CRM身份验证](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md):OAuth 2.0协议可用于在Marketo Engage和Salesforce CRM之间同步操作。 对于新订阅者，此选项默认处于启用状态。 当前订阅者可通过联系Marketo支持团队来请求此功能。
* [Salesforce CRM同步功能板](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md):管理员可以从功能板快速查看Salesforce CRM同步状态。 同步性能报表时间跨度已从2小时增加到5天。
* **元数据导出**:增强了支持机会对象属性、命名帐户、程序成员的标准字段和自定义字段。

## 管理 {#administration}

* **更新了“我的帐户”页面**:查看“我的帐户”页面上的基本订阅信息。 具有任何级别访问权限的用户可以查看订阅名称、数据中心标识符和Munchkin ID。

**_在整个季度发布_**

以下功能处于非季度周期，将在未来几个月内发布。

## 销售分析 {#sales-insight}

![（星号）](assets/yellow-star.png)

* **[增强的测试电子邮件工作流(Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**:通过增强的Sales Insight测试电子邮件工作流程，提高您的销售团队的效率。 销售商可先向选定的电子邮件地址发送测试电子邮件，然后再向最多200个收件人发送批量电子邮件。
* **[电子邮件状态分析(Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**:当用户在发送电子邮件之前尝试向无效的电子邮件ID或未订阅的电子邮件地址发送电子邮件时，会看到一条警告消息。  可以在Sales Insight的“电子邮件”选项卡中查看电子邮件投放状态。
* **从发送批量电子邮件 [帐户](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) 和 [机会](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) 面板(Salesforce CRM)**:通过使用新的批量操作功能，提高销售商工作流程的效率，并与整个客户或销售机会联系人列表互动。 使用帐户或机会选项卡中的新下拉选项，而不是使用单个联系人，发送电子邮件或向Marketo Engage活动添加联系人。 将帐户联系人添加到监视列表，以在潜在客户变热时通知。
* **[针对非本机Salesforce CRM集成的Sales Insight](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**:使用自定义Salesforce CRM集成的GA订阅可以安装Sales Insight包，并帮助销售团队排定优先级，并与最有希望的商机和机会进行互动。
* **[最佳增强功能](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**:通过向电子邮件发送或将热门潜在客户添加到Marketo Engage营销活动，快速从“最佳选择”选项卡中联系他们。 在Marketo Engage中查看潜在客户或将其添加到监视列表。 “最佳选择”选项卡上的批量操作和排序选项可节省时间并提高销售团队的效率。

## Sales Connect {#sales-connect}

![（星号）](assets/yellow-star.png)

* **电子邮件连接限制（测试版）**:通过Email Connection Throttling for Sales Connect提高电子邮件投放能力，并扩展您的1:1销售通信。 我们的新限制技术可自动管理电子邮件发送时间，为Exchange和Gmail用户创建无缝体验。 减少或消除第三方批量电子邮件发送应用程序的使用。
* **电子邮件连接跳出跟踪**:通过新的电子邮件退回报表深入了解潜在客户质量和电子邮件模板的性能。 Exchange和Gmail用户可能会选择接收退回通知，这些通知将汇总到实时信息源、电子邮件文件夹、模板分析和促销活动分析。
* **配置文件页面配置**:在新配置文件页面中轻松管理用户首选项。 更改密码、编辑地理位置和语言设置，以及在一个位置查看集成状态。
* **模板管理**:使用新的拖放功能将销售电子邮件模板组织到不同的类别中，以确保快速访问相关模板并缩短搜索时间。
* **Sales Connect用户体验更新**:通过调整列大小和重新排序列，自定义Sales Connect网格布局。 查看首选项会自动保存。

**_公告和弃用_**

* 所有用户必须升级到Sales Insight的最新版本 **2021年1月15日之前**. 如果您尚未完成升级，则在登录到应用程序时，系统会提示您完成升级。 按照说明操作 [在本指南中](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). 更新版本包含针对已识别安全漏洞的修补程序。 修补程序最初于2016年4月6日发布。 注意： **版本1.4363或更高版本** 无需执行升级。
* Form 1.0服务将在 **2021年5月** 版本。 Forms 1.0服务将完全弃用，从而导致任何仍在使用的其余Forms 1.0资产功能丢失。 此外，通过不支持的方法（如将表单POST编程到leadCapture/save和leadCapture/save2端点）提交的表单将会被拒绝。 有关更多信息和补救，请参阅 [我们在营销国家的帖子](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* 2021年，Marketo Engage将更改登陆页面、表单、图像和文件资产的URL结构。 对于现有Marketo Engage订阅，我们将于2021年4月1日开始逐步推出。 有关推出时间轴的更多详细信息将于2021年3月发布。 有关每种受影响的资产类型将如何更改的详细信息，请参阅 [我们在营销国家的帖子](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_产品发行网络研讨会_**

想要了解有关这些功能和增强功能的更多信息？ 一定要 [立即注册](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) 1月21日下午1:00 PT /下午4:00 ET与我们一起参加实时网络研讨会，与我们的产品团队一起深入研究这些创新。

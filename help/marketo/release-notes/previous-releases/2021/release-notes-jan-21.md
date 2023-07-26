---
description: 发行说明 — 2021年1月 — Marketo文档 — 产品文档
title: 发行说明 — 2021年1月
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# 发行说明： 2021年1月 {#release-notes-jan-21}

2021年1月版本中包含以下功能。 检查您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![(star)](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_**

以下功能将发布于 **2021年1月15日**.

## 新一代用户体验 {#next-generation-user-experience}

* 工作区支持：Marketo Engage的新一代用户体验将Adobe Experience Cloud的外观与效果与工作效率创新相结合，帮助营销从业人员更快、更智能地工作。 在最新版本中，我们将添加对工作区和分区的完全支持，包括跨工作区共享文件夹的功能。 右侧画布将提供一个切换开关，允许您在每个功能的新旧体验之间无缝过渡，而不会丢失上下文。 [了解详情](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124) 来自营销国家/地区新一代体验常见问题解答。

## 多渠道个性化 {#multi-channel-personalization}

* **[Adobe Experience Cloud Audience Sync 3阶段](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**：现有Adobe Experience Cloud (AEC) Audience Sync功能现在支持从Marketo Engage到其他AEC应用程序的连续、双向B2B受众同步，包括Adobe Experience Platform (AEP)产品，如Real-time Customer Data Platform和Adobe Experience Platform Activation。  在向受众区段添加和删除潜在客户时，Marketo Engage将自动在连接的AEC应用程序中同步更新的受众。 借助它，您可以在AEC技术栈栈中利用Adobe的多渠道编排、重新定位、受众抑制、个性化和报告用例。
* **[持续将受众同步到Google、Facebook和LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**：可以在静态列表上启用与广告网络的连续自动同步，随着列表成员资格更改来更新广告网络，而无需用户干预。
* **[项目群成员自定义字段的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**：我们扩展了项目成员自定义字段功能以支持令牌框架。 营销人员可以将项目成员自定义字段令牌插入电子邮件、登陆页、短信消息、推送通知和Webhook中。 在营销活动流程操作中使用新令牌来更改数据值、创建任务或有趣的时刻。

## Landing Pages和Forms {#landing-pages-and-forms}

* **表单API**：从非Marketo表单中提取数据时，提取潜在客户信息或触发培养营销活动。 非Marketo表单可以通过REST API与Marketo Engage集成。 利用新API，可模拟具有所有相关功能的Marketo Engage表单提交。
* **登陆页面API**：使用新的登陆页面预览API简化集成应用程序中的编辑和翻译工作流。 第三方供应商现在可以呈现完全个性化的登陆页面预览，而无需登录Marketo Engage。  登陆页面预览API支持在第三方集成应用程序中执行端到端编辑和本地化工作流。

## 电子邮件营销 {#email-marketing}

* **[自定义对象检索限制提高](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**：电子邮件Velocity脚本的开发者可以通过自助覆盖快速将自定义对象数增加到100。 营销人员可以通过访问大量第一级和第二级自定义对象来提高智能营销活动的有效性。

## Salesforce CRM集成 {#salesforce-crm-integration}

* [Salesforce CRM身份验证](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md)： OAuth 2.0协议可用于Marketo Engage与Salesforce CRM之间的同步操作。 对于新订阅者，默认情况下会启用此选项。 当前订阅者可以通过联系Marketo支持来请求此功能。
* [Salesforce CRM同步功能板](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md)：管理员可以从仪表板快速查看Salesforce CRM同步状态。 同步性能报表时间跨度已从2小时增加到5天。
* **元数据导出**：进行了增强，可支持机会对象属性、指定帐户、项目成员的标准和自定义字段。

## 管理 {#administration}

* **更新了“我的帐户”页面**：查看“我的帐户”页面上的基本订阅信息。 具有任何访问级别的用户可以查看订阅名称、数据中心标识符和Munchkin ID。

**_将在整个季度中发布_**

以下功能采用非季度周期，并将在未来几个月发布。

## 销售分析 {#sales-insight}

![(star)](assets/yellow-star.png)

* **[增强测试电子邮件工作流(Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**：通过增强的Sales Insight测试电子邮件工作流提高销售团队的效率。 销售人员可以向选定的电子邮件地址发送测试电子邮件，然后再向最多200个收件人发送批量电子邮件。
* **[电子邮件状态分析(Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**：用户在发送电子邮件之前尝试向无效的电子邮件ID或取消订阅的电子邮件地址发送电子邮件时，会看到警告消息。  可以在Sales Insight的email选项卡中查看电子邮件投放状态。
* **发送批量电子邮件 [帐户](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) 和 [机会](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) 面板(Salesforce CRM)**：通过使用新的批量操作功能，提高卖方工作流的效率并与整个客户或机会联系人列表交互。 通过使用“帐户”或“机会”选项卡中新的下拉选项（而不是与单个联系人合作），发送电子邮件或向Marketo Engage促销活动添加联系人。 将帐户联系人添加到监视列表，以便在潜在客户变得热门时收到通知。
* **[Sales Insight for Non-Native Salesforce CRM集成](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**：具有自定义Salesforce CRM集成的GA订阅可以安装Sales Insight包，并帮助销售团队确定优先顺序并与最有希望的商机和机会交互。
* **[最佳匹配增强功能](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**：通过电子邮件发送或将其添加到Marketo Engage营销活动，从“最佳匹配”选项卡快速联系热门潜在客户。 在Marketo Engage中查看潜在客户或将其添加到您的关注列表。 “最佳匹配”选项卡上的批量操作和排序选项可节省时间并提高销售团队的效率。

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **电子邮件连接限制（测试版）**：通过Sales Connect的Email Connection限制功能改进电子邮件可投放性，并扩展1:1销售通信。 我们的新限制技术可自动管理电子邮件发送时间，为Exchange和Gmail用户创造无缝体验。 减少或消除使用第三方批量电子邮件发送应用程序。
* **电子邮件连接退回跟踪**：通过新的电子邮件退回报告，深入了解商机质量和电子邮件模板性能。 Exchange和Gmail用户可以选择接收将汇总到实时信息源、电子邮件文件夹、模板分析和营销活动分析的退回通知。
* **配置文件页面配置**：在新的配置文件页面中轻松管理用户首选项。 在一个位置更改密码、编辑地理位置和语言设置以及查看集成状态。
* **模板管理**：使用新的拖放功能将销售电子邮件模板整理到不同的类别中，以确保快速访问相关模板并减少搜索时间。
* **Sales Connect用户体验更新**：通过调整列的大小和重新排序列来自定义Sales Connect网格布局。 您的查看首选项会自动保存。

**_公告和弃用_**

* 所有用户都必须升级到最新版本的Sales Insight **2021年1月15日之前**. 如果您尚未完成升级，则在登录应用程序时会提示您完成升级。 按照说明操作 [本指南内容](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). 更新版本包括一个针对已识别安全漏洞的修补程序。 该修补程序最初于2016年4月6日发布。 注意： **版本1.4363或更高版本** 无需执行升级。
* 弃用Form 1.0服务将从 **2021年5月** 释放。 Forms 1.0服务将被完全弃用，从而导致仍在使用的所有其余Forms 1.0资源失去功能。 此外，通过不受支持的方法（如向leadCapture/save和leadCapture/save2端点提供的程序化表单POST ）提交的表单将被拒绝。 有关更多信息和修正，请参阅 [我们在Marketing Nation的帖子](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* 2021年，Marketo Engage将更改登陆页面、表单以及图像和文件资源的URL结构。 对于现有Marketo Engage订购，我们将于2021年4月1日开始逐步推出。 有关推出时间表的更多详细信息将于2021年3月发布。 有关每个受影响的资产类型将如何更改的详细信息，请参阅 [我们在Marketing Nation的帖子](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_产品发布网络研讨会_**

想要详细了解这些功能和增强功能？ 请务必 [立即注册](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) 于1月21日下午1:00 PT / 4:00 PM加入我们，与我们的产品团队一起参加实时网络研讨会，以深入了解这些创新。

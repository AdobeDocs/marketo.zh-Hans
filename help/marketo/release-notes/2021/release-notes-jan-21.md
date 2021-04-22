---
description: 发行说明 — 2021年1月 — Marketo Docs — 产品文档
title: 发行说明 — 2021年1月
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# 发行说明：2021年1月{#release-notes-jan-21}

’21年1月版包含以下功能。 查看您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>由星形(![(star)](assets/star-yellow.svg))表示的特征是付费附加项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度发行_**

以下功能将于2021年1月15日&#x200B;**发布**。

## 下一代用户体验{#next-generation-user-experience}

* 支持工作区：Marketo Engage的下一代用户体验将Adobe Experience Cloud的外观和感觉与工作效率创新结合在一起，从而帮助营销从业者更快、更智能地工作。 在最新版本中，我们添加了对工作区和分区的完全支持，包括跨工作区共享文件夹的功能。 右侧的画布将优惠切换开关，让您能够根据新功能无缝过渡旧体验和新体验，同时不会丢失上下文。 [从](https://nation.marketo.com/t5/The-Next-Generation-Experience/Next-Generation-Experience-FAQ/ba-p/307124) Marketing Nation的下一代体验常见问题解答中进一步了解。

## 多渠道个性化{#multi-channel-personalization}

* **[Adobe Experience Cloud 受众同步阶段3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**:现有的Adobe Experience Cloud(AEC)受众同步功能现在支持从Marketo Engage到其他AEC应用程序(包括Adobe Experience Platform(AEP)产品(如实时客户数据平台和Adobe Experience Platform激活)的连续、双向B2B受众同步。在受众细分中添加和删除潜在客户时，Marketo Engage将在连接的AEC应用程序中自动同步更新的受众。 在您的AEC技术堆栈中利用Adobe的多渠道编排、重定向、受众抑制、个性化和报告使用案例。
* **[连续受众同步到Google、Facebook和LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**:可以在静态列表上启用与广告网络的连续自动同步，随着列表成员资格的变化而更新广告网络，而无需用户干预。
* **[项目成员自定义字段的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**:我们扩展了项目成员自定义字段功能以支持令牌框架。营销人员可以在电子邮件、登陆页、短信、推送通知和网络挂钩中插入项目成员自定义字段令牌。 在活动流动操作中使用新令牌来更改数据值、创建任务或有趣的时刻。

## 登陆页和Forms {#landing-pages-and-forms}

* **表单API**:从非Marketo表单中提取数据时，导入潜在客户信息或触发培养活动。非Marketo表单可以通过REST API与Marketo Engage集成。 新的API能够模拟Marketo Engage表单提交与所有相关功能。
* **登陆页API**:借助新的登陆页 预览 API简化集成应用程序中的编辑和翻译工作流。第三方供应商现在无需登录Marketo Engage即可呈现完全个性化的预览登陆页。  登陆页 预览 API支持第三方集成应用程序中的端到端编辑和本地化工作流。

## 电子邮件营销{#email-marketing}

* **[自定义对象检索限制增加](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**:电子邮件速度脚本的开发人员可以通过自助覆盖将自定义对象的数量快速增加到100个。营销人员可以访问更多的一级和二级自定义对象，从而提高智能活动的有效性。

## Salesforce CRM集成{#salesforce-crm-integration}

* [Salesforce CRM身份验证](/help/marketo/product-docs/crm-sync/salesforce-sync/setting-up-oauth-2-0.md):OAuth 2.0协议可用于在Marketo Engage和Salesforce CRM之间同步操作。对于新订阅者，此选项默认处于启用状态。 当前订阅者可以联系Marketo支持部门来请求此功能。
* [Salesforce CRM同步仪表板](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md):管理员可以从仪表板快速查看Salesforce CRM同步状态。同步性能报告的时间跨度已从2小时增加到5天。
* **元数据导出**:增强功能可支持业务机会对象属性、命名帐户、项目成员的标准字段和自定义字段。

## 管理{#administration}

* **已更新我的帐户页面**:在“我的帐户”页面上查看基本订阅信息。具有任何访问级别的用户都可以视图订阅名称、数据中心标识符和Munchkin ID。

**_在整个季度内发布_**

以下功能按非季度周期发布，将在未来几个月发布。

## 销售分析{#sales-insight}

![（星号）](assets/star-yellow.svg)

* **[增强的测试电子邮件工作流(Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**:通过增强的Sales Insight测试电子邮件工作流，提高销售团队的效率。销售者可以在向多达200位收件人发送批量电子邮件之前，将测试电子邮件发送到选定的电子邮件地址。
* **[对电子邮件状态(Salesforce CRM)的洞察](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**:当用户尝试在发送电子邮件之前向无效的电子邮件ID或未订阅的电子邮件地址发送电子邮件时，会看到一条警告消息。 电子邮件投放状态可在Sales Insight的“电子邮件”选项卡中进行查看。
* **从Account和OpportunityPanels( [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) Salesforce  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) CRM)发送批量电子邮件**:通过使用新的批量操作功能，提高销售商工作流程的效率并与整个帐户或机会联系列表互动。使用帐户或业务机会选项卡中的新下拉选项（而不是使用单个联系人），可以发送电子邮件或向Marketo Engage活动添加联系人。 将帐户联系人添加到观察列表，以便在潜在客户变得热门时通知。
* **[针对非本机Salesforce CRM集成的Sales Insight](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**:具有自定义Salesforce CRM集成的GA订阅可以安装Sales Insight包，并帮助销售团队排定优先级并与最有前途的潜在客户和机会互动。
* **[最佳增强](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**:通过向Marketo Engage活动发送电子邮件或将热门潜在客户添加到“最佳选择”选项卡，快速与他们联系。视图Marketo Engage中的潜在客户或将其添加到监视列表。 “最佳下注”选项卡上的批量操作和排序选项可节省时间并提高销售团队的效率。

## Sales Connect {#sales-connect}

![（星号）](assets/star-yellow.svg)

* **电子邮件连接限制（测试版）**:使用Sales Connect的Email Connection Throttling（电子邮件连接限制）提高电子邮件的发送能力并调整您的一对一销售通信。我们的新节流技术可自动管理电子邮件发送时间，为Exchange和Gmail用户创建无缝体验。 减少或消除第三方批量电子邮件发送应用程序的使用。
* **电子邮件连接跳出跟踪**:利用新的电子邮件跳出报表深入了解潜在客户质量和电子邮件模板性能。Exchange和Gmail用户可能会选择接收跳出通知，这些通知将汇总到“实时信息源”、“电子邮件文件夹”、“模板分析”和“活动分析”。
* **用户档案页配置**:在新的用户档案页面中轻松管理用户首选项。更改密码，编辑地理位置和语言设置，并在一个位置查看集成状态。
* **模板管理**:使用新增的拖放功能将销售电子邮件模板组织到类别中，以确保快速访问相关模板并缩短搜索时间。
* **Sales Connect用户体验更新**:通过调整列的大小和重新排序，自定义Sales Connect网格布局。您的查看首选项将自动保存。

**_公告和弃用_**

* 所有用户必须在2021年1月15日之前升级到最新版Sales Insight **。**&#x200B;如果您尚未完成升级，则登录应用程序时将提示您完成升级。 按照本指南](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md)中的说明[操作。 更新版本包含针对已识别安全漏洞的修补程序。 修补程序最初于2016年4月6日发布。 注意：**版本1.4363或更高版本**&#x200B;无需执行升级。
* 表1.0服务的弃用将在&#x200B;**2021年5月**&#x200B;版本中生效。 Forms 1.0服务将完全弃用，导致仍在使用的任何剩余Forms 1.0资源功能丢失。 此外，通过不受支持的方法（如将表单POST程序化到leadCapture/save和leadCapture/save2端点）提交的表单将被拒绝。 有关详细信息和补救，请参阅[我们在Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631)中的帖子。
* 在2021年，Marketo Engage将更改登陆页、表单、图像和文件资源的URL结构。 对于现有Marketo Engage订阅，我们将于2021年4月1日开始逐步推出。 有关转出时间线的更多详细信息将于2021年3月发布。 有关每种受影响的资产类型将如何更改的详细信息，请参阅我们在Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632)中的帖子。[

**_产品发布网络研讨会_**

想了解有关这些功能和增强功能的更多信息吗？ 请务必[立即注册](https://engage.marketo.com/January_21_Release_Webinar_Registration.html)，于1月21日下午1:00 PT/下午4:00加入我们，与我们的产品团队一起参加实时网络研讨会，以更深入地了解这些创新。

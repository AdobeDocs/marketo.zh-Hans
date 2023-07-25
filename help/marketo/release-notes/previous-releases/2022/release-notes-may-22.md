---
description: 发行说明 — 2022年5月 — Marketo文档 — 产品文档
title: 发行说明 — 2022年5月
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# 发行说明： 2022年5月 {#release-notes-may-22}

在下方，您会找到2022年5月版本中包含的所有功能。 查看Adobe Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![星形](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_**

以下功能将开始发布 **2022年5月6日**，在接下来的几周内分阶段推出剩余的功能（除非另有说明）。

## 本机CRM集成 {#native-crm-integration}

**[本机Veeva CRM集成](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} （限量发布）**：通过本机集成在Veeva CRM和Marketo Engage之间同步活动，从而改善与医疗保健专业人员的互动。 此集成允许营销人员为医疗保健专业人员创建更加个性化且无缝的跨渠道体验。 如果您有兴趣参与，请联系Adobe客户团队（您的客户经理）。

## 跨渠道编排 {#cross-channel-orchestration}

**适用于Dynamic Chat的聊天机器人事件**：利用更详细的Web访客行为数据（如页面逗留时间、网站逗留时间和页面滚动百分比）来定义应何时显示聊天对话框。

**为Dynamic Chat嵌入PDF**：通过将PDF嵌入聊天对话框并通过参与活动跟踪衡量内容性能，提高参与度并共享有意义的内容。

**对Dynamic Chat的扩展语言支持**：Dynamic Chat用户界面现在还提供法语、德语、日语、葡萄牙语和西班牙语版本。 也可以用这些语言配置聊天对话框。

**排除Dynamic Chat的URL**：控制您的Web页面Dynamic Chat显示在哪一个上，并能够从定位标准中排除特定URL。

**[电子邮件机器人活动筛选增强功能](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**：除了现有的IAB列表匹配识别之外，还能根据隐藏的链接、用户代理或IP和邻近模式识别机器人行为，继续保护数据库的健康状况。 查看机器人活动统计信息，以便您了解针对每种类型识别的机器人活动数量。

**[电子邮件跟踪链接的STS标头](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**：符合安全最佳实践，能够应用Secure Transport Security标头，以确保到跟踪链接的流量始终安全。

## 新一代体验 {#modern-ux}

**切换切换默认使用下一代体验**：切换开关将在所有可用屏幕中默认使用新体验，使用户更轻松地发现更新的设计和可用性增强。

**更新了下一代体验中的屏幕**：

我们在Design Studio中提供了新一代体验中的电子邮件模板详细信息视图，提供了更新的设计和可用性增强功能，可通过切换开关进行访问。

## 体验自动化 {#experience-automation}

**自助服务流程步骤（续测试版）**：扩展Marketo Engage与栈栈其余部分之间的连接，并能够创作自定义的流量步骤以用于Smart Campaigns。 Marketo Engage用户和合作伙伴都可以利用此功能，允许在触发、批量和可执行的营销活动中使用外部Web服务（与只能在触发营销活动中使用的Webhook不同）。

## API增强功能 {#api-enhancements}

* **为启用了CRM的订阅扩展了API访问权限**：我们正在扩展已启用CRM同步的订阅的API访问权限，以便用户能够从Marketo Engage中检索公司、商机和销售人员。
* **在Forms中支持“隐藏”数据类型**：提供通过API管理隐藏表单字段的功能。
* **通过Rules支持isNot Form的多个比较值**：根据另一个字段的值是否不是给定列表中的值之一来管理表单字段的可见性。
* **允许分别设置选择列表中的显示值和提交值**：在字段中分别设置显示值和提交的值。 例如，显示酒店的名称，但向后端提交内部ID。
* **允许设置禁用创建或更新电子邮件时的打开跟踪**：创建禁用了打开跟踪的电子邮件。

## 公告 {#announcements}

**电子邮件验证和唯一性**：从4月开始，电子邮件验证将开始推出。 此时，Marketo Engage用户电子邮件地址将需要验证和唯一性（这不适用于仅API用户）。 当目录服务验证的用户订阅启用电子邮件验证时，这些用户将自动验证其电子邮件。

使用“在邀请用户对话框中登录”功能或者只有一封电子邮件与多个用户关联的订阅的电子邮件验证将与5月版本一致。 对于与多个用户关联的单封电子邮件的订阅，将使用电子邮件验证来启用，并将要求这些用户解决冲突并为每个用户使用唯一的电子邮件。 启用“登录邀请用户对话框”功能后，通过此功能邀请的用户将需要拥有唯一的电子邮件地址。 对于通过此功能邀请的仅API用户，电子邮件地址不需要是唯一的。

**存档文件夹行为更改**：在此版本中，在存档文件夹中创建新资产的功能将不再从树上下文菜单中可用。 所有资源都将隐藏用于创建新资源的菜单选项。 [在此处了解详情](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_产品发布网络研讨会_**

[2022年3月和5月Marketo Engage发布网络研讨会](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

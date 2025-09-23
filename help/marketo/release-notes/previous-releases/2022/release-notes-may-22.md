---
description: 发行说明 — 2022年5月 — Marketo文档 — 产品文档
title: 发行说明 - 2022 年 5 月
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 4%

---

# 发行说明：2022 年 5 月 {#release-notes-may-22}

在下方，您会找到2022年5月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。请联系您的 Marketo Engage 代表了解更多信息。

**_季度发布_**

以下功能将于&#x200B;**2022年5月6日**&#x200B;开始发布，并在接下来的几周内分阶段推出剩余功能（除非另有说明）。

## 本机CRM集成 {#native-crm-integration}

**[本机Veeva CRM集成](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} （限量发布）**：通过本机集成在Veeva CRM和Marketo Engage之间同步活动，从而改善与医疗保健专业人员的互动。 此集成允许营销人员为医疗保健专业人员创建更加个性化且无缝的跨渠道体验。 如果您有兴趣参与，请联系您的客户成功经理。

## 跨渠道编排 {#cross-channel-orchestration}

**针对[!DNL Dynamic Chat]**&#x200B;的聊天机器人事件：利用更详细的Web访客行为数据（如页面逗留时间、网站逗留时间和页面滚动百分比）来定义何时应显示聊天对话框。

**PDF为[!DNL Dynamic Chat]**&#x200B;嵌入：通过将PDF嵌入聊天对话框以及通过参与活动跟踪衡量内容性能，提高参与度并共享有意义的内容。

**针对[!DNL Dynamic Chat]**&#x200B;的扩展语言支持： [!DNL Dynamic Chat]用户界面现在还将提供法语、德语、日语、葡萄牙语和西班牙语版本。 也可以用这些语言配置聊天对话框。

**排除[!DNL Dynamic Chat]**&#x200B;的URL：控制您的网页[!DNL Dynamic Chat]中的哪些网页能够排除定位条件中的特定URL。

**[电子邮件机器人活动过滤增强功能](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**：除了现有的IAB列表匹配标识之外，还能够基于隐藏链接用户代理或IP和邻近关系模式来识别机器人行为，继续保护数据库的运行状况。 查看机器人活动统计信息，以便您了解针对每种类型标识的机器人活动数。

电子邮件跟踪链接的&#x200B;**[STS标头](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**：符合安全最佳实践，能够应用Secure Transport Security标头，以确保跟踪链接的流量始终安全。

## 新一代体验 {#modern-ux}

**切换开关默认为新一代体验**：切换开关将在所有可用屏幕中都默认为新体验，使用户更容易发现更新的设计和可用性增强功能。

**更新了下一代体验中的屏幕**：

我们在[!UICONTROL Design Studio]内提供了新一代体验中的电子邮件模板详细信息视图，提供了更新的设计和可用性增强功能，可通过切换开关访问。

## 体验自动化 {#experience-automation}

**自助服务流程步骤（继续测试版）**：扩展Marketo Engage与栈栈其他部分之间的连接，并能够创作自定义流程步骤以用于Smart Campaigns。 Marketo Engage用户和合作伙伴都可以利用此功能，允许在触发、批量和可执行的营销活动中使用外部Web服务（与只能在触发营销活动中使用的Webhook不同）。

## API增强功能 {#api-enhancements}

* **为启用了CRM的订阅扩展API访问**：我们正在为启用了CRM同步的订阅扩展API访问，以允许用户从Marketo Engage检索公司、商机和销售人员。
* **支持Forms中的“隐藏”数据类型**：提供通过API管理隐藏表单字段的功能。
* **通过Rules支持isNot表单的多个比较值**：根据另一个字段的值是否不是给定列表中的值之一来管理表单字段的可见性。
* **允许单独设置选择列表中的显示值和提交值**：单独设置字段中的显示值和提交值。 例如，显示酒店的名称，但向后端提交内部ID。
* **允许在“创建或更新电子邮件”时禁用“打开跟踪”设置**：创建禁用了打开跟踪的电子邮件。

## 公告 {#announcements}

**电子邮件验证和唯一性**：从4月开始，将开始推出电子邮件验证。 届时，Marketo Engage用户电子邮件地址将需要验证和唯一性（这不适用于仅API用户）。 当目录服务认证用户的订阅启用了电子邮件验证时，该用户将自动验证其电子邮件。

使用&quot;[!UICONTROL Login in Invite User Dialog]&quot;功能订阅的电子邮件验证或只有一封电子邮件与多个用户关联的订阅的电子邮件验证将与5月版本一致。 如果订阅只有一个与多个用户关联的电子邮件，则会启用电子邮件验证，并将要求这些用户解决冲突并为每个用户使用唯一的电子邮件。 启用“在邀请用户对话框中登录”功能后，通过此功能邀请的用户将需要具有唯一的电子邮件地址。 对于通过此功能邀请的仅API用户，电子邮件地址不需要是唯一的。

**存档文件夹行为更改**：在此版本中，将无法再从树上下文菜单中使用在存档文件夹中创建新资源的功能。 用于创建新资产的菜单选项将对所有资产隐藏。 [在此了解详情](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}。

**_产品发布网络研讨会_**

[2022年3月和5月Marketo Engage发布网络研讨会](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

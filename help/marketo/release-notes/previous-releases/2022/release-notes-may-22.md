---
description: 发行说明 — 2022年5月 — Marketo文档 — 产品文档
title: 发行说明 — 2022年5月
source-git-commit: d9ace2b00707c605dda94ec4fc21937d8b36d137
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# 发行说明：2022年5月 {#release-notes-may-22}

下面将显示’22年5月版中包含的所有功能。 查看您的Adobe Marketo Engage版本以了解功能的可用性。

>[!AVAILABILITY]
>
>由星(![星星](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_**

将在 **2022年5月6日**，并在随后的几周内分阶段推出其余功能（除非另有指定）。

## 本机CRM集成 {#native-crm-integration}

**[本机Veeva CRM集成](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target=&quot;_blank&quot;}（可用性有限）**:通过本机集成在Veeva CRM和Marketo Engage之间同步活动，提高与医疗保健专业人士的参与度。 此集成允许营销人员为医疗保健专业人士创建更个性化、更无缝的跨渠道体验。 如果您有兴趣参与，请联系您的客户成功经理。

## 跨渠道编排 {#cross-channel-orchestration}

**用于动态聊天的聊天机器人事件**:利用Web访客的更详细的行为数据（如页面逗留时间、网站逗留时间和页面滚动百分比）来定义何时应显示聊天对话框。

**PDF嵌入到动态聊天**:通过将PDF嵌入聊天对话框来提高参与度并共享有意义的内容，并通过参与活动跟踪来衡量内容的性能。

**动态聊天的扩展语言支持**:现在，动态聊天用户界面还将提供法语、德语、日语、葡萄牙语和西班牙语版本。 聊天对话框也可以配置这些语言。

**排除动态聊天的URL**:控制动态聊天在上显示哪些网页，并能够从定位标准中排除特定URL。

**[电子邮件机器人活动筛选增强功能](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target=&quot;_blank&quot;}**:除了现有的IAB列表匹配标识之外，还能够根据隐藏的链接用户代理或IP和邻近模式识别机器人行为，从而继续保护数据库的运行状况。 查看机器人活动统计资料，以便您了解针对每种类型标识的机器人活动数量。

**[电子邮件跟踪链接的STS标头](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target=&quot;_blank&quot;}**:通过应用安全传输安全标头来确保跟踪链接的流量始终安全，从而满足安全最佳实践。

## 新一代体验 {#next-generation-experience}

**将默认的开关切换到下一代体验**：切换开关将默认显示所有可用屏幕中的新体验，从而更便于用户发现更新的设计和可用性增强。

**下一代体验中的更新屏幕**:

我们将在Design Studio中提供电子邮件模板详细信息视图，以提供可通过切换开关访问的更新设计和可用性增强功能。

## 体验自动化 {#experience-automation}

**自助服务流程步骤（续测试版）**:通过创作自定义流程步骤以在智能促销活动中使用，扩展Marketo Engage与堆栈其余部分之间的连接。 Marketo Engage用户和合作伙伴都可以利用此功能在触发器、批量活动和可执行活动中使用外部Web服务（与只能在触发活动中使用的Web挂钩相反）。

## API增强功能 {#api-enhancements}

* **针对支持CRM的订阅的扩展API访问**:我们正在扩展对启用了CRM同步的订阅的API访问，以允许用户从Marketo Engage中检索公司、机会和销售人员。
* **在Forms中支持“隐藏”数据类型**:提供通过API管理隐藏的表单字段的功能。
* **通过规则支持isNot表单的多个比较值**:根据另一个字段的值是否不是给定列表中的值之一，管理表单字段的可见性。
* **允许在选择列表中单独设置显示值和提交值**:在字段中分别设置显示值和提交值。 例如，显示酒店名称，但向后端提交内部ID。
* **允许在创建或更新电子邮件时禁用打开跟踪**:创建禁用打开跟踪的电子邮件。

## 公告 {#announcements}

**电子邮件验证和唯一性**:从4月开始，电子邮件验证将开始推出。 此时，Marketo Engage用户电子邮件地址将需要验证和唯一性（这不适用于仅API用户）。 通过“电子邮件验证”启用订阅后，经目录服务验证的用户将自动验证其电子邮件。

使用“在邀请用户对话框中登录”功能或者具有一封与多个用户关联的电子邮件的订阅电子邮件验证将与5月版本同时发布。 如果订阅有一封与多个用户关联的电子邮件，则将启用电子邮件验证，并要求这些用户解决冲突，并为每个用户使用唯一的电子邮件。 启用“在邀请用户对话框中登录”功能后，通过此功能邀请的用户将需要具有唯一的电子邮件地址。 对于通过此功能邀请的仅限API的用户，电子邮件地址不必是唯一的。

**存档文件夹行为更改**:在此版本中，树上下文菜单中将不再提供在存档文件夹中创建新资产的功能。 用于创建新资产的菜单选项将在所有资产中都处于隐藏状态。 [在此处了解更多](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target=&quot;_blank&quot;}。

**_产品发行网络研讨会_**

[2022年3月和5月版Marketo Engage网络研讨会](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target=&quot;_blank&quot;}
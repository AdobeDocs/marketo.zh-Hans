---
unique-page-id: 11370952
description: 发行说明 — Spring '16 - Marketo Docs — 产品文档
title: 发行说明 — 2016年春
exl-id: 0ca26acf-2ac2-418e-bc4e-9820f483fa71
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# 发行说明：春季’16 {#release-notes-spring}

’16春季版包含以下功能。 请单击标题链接，以视图每种功能的详细文章。

## [电子邮件洞察](/help/marketo/product-docs/reporting/email-insights/email-insights-overview.md) {#email-insights}

Email Insights是一种全新的历史聚合数据电子邮件分析体验 — 作为Project Orion的一部分，重新设计了端对端功能，实现了闪电般的性能。 它采用了经过优化的全新用户界面设计，以满足电子邮件营销人员的需求和工作流程。

>[!NOTE]
>
>从6月3日开始，我们将批量向客户发布电子邮件洞察。 我们的目标是在未来几个月完成这项工作。 启用后，我们会通过电子邮件通知您。

![](assets/two.png)

## [电子邮件模板选取器](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-picker-overview.md) {#email-template-picker}

使用我们新的入门模板创建精美的电子邮件！ 此外，还可以从模板的实时缩览图中快速找到模板。

>[!NOTE]
>
>电子邮件编辑器2.0（使用模板选取器）将从6月3日开始逐步推出。 我们将在6月30日前完成推广。 与电子邮件分析不同，您在有权访问时不会收到通知。 要查看是否这样做，请按照[本文](/help/marketo/product-docs/email-marketing/general/email-editor-2/transitioning-to-email-editor-2-0.md)中的步骤操作。

![](assets/5-29-home-starter-templates.png)

## [电子邮件编辑 — 改良设计](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-editing-re-imagined}

没错，是全新的电子邮件编辑！ 使用轻量拖放功能添加和重新排序内容。 包括图像、视频、变量和模块在内的新元素肯定会增强您的编辑体验。 另请查看更新的代码编辑器、预查看器和预标题支持。

![](assets/17a-29-modules-next.png)

## [移动应用内消息](/help/marketo/product-docs/mobile-marketing/in-app-messages/understanding-in-app-messages.md) {#mobile-in-app-messages}

直接在Marketo中为您的应用程序创建令人赞叹的应用程序内消息。 使用应用程序内消息项目准确定义应查看内容的人员及时间。 使用项目仪表板轻松监控性能。

![](assets/pasted-image-at-2016-05-24-09-45-am.png)

## [无草稿片段](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/enable-no-draft-for-snippets.md) {#no-draft-snippets}

每次更新代码片断时，您必须重新批准所有内容的日子已经过去了！ 使用“无草稿”时，所有使用代码片段的电子邮件和登陆页都将获取代码片段更新并保持其先前的状态。 每次批准代码片断时，您都可以选择运行“无草稿”并更新所有内容，或创建草稿。 由你决定！ “无草稿”将对所有客户可用，并由“管理员”中的新权限控制。

![](assets/image2016-5-16-15-3a41-3a17.png)

## [登陆页、登陆页模板和表单API](https://developers.marketo.com/blog/spring-2016-updates/) {#landing-page-landing-page-template-and-form-apis}

Marketo REST API现在支持对Marketo登陆页、登陆页模板和表单的控制。 用户现在可以直接通过Marketo REST API创建、更新内容、批准和删除这些资产。

## [IP列入允许列表访问API](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md) {#ip-allowlisting-for-api-access}

与Marketo用户登列入允许列表录的IP功能类似，Marketo管理员现在可以设置一允许列表个IP地址，以访问Marketo SOAP和REST API，从而阻止来自未授权IP地址的访问。 这为您的Marketo实例增加了一层安全性，并确保API访问只能从组织的网络中进行。 有关如何设置的详细信息，请参阅[Marketo文档站点](/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md)。

## [全新高速Microsoft Dynamics同步连接器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#new-high-speed-microsoft-dynamics-sync-connector}

新的高速动态连接器以Orion架构为构建基础，为初始同步提供了高达20倍的速度，为增量同步提供了高达5倍的速度。 所有新客户将在发布日期加入此连接器，我们将在夏季发布时间范围内逐步将其推广给现有客户。

**刷新新字段的数据**:现在，您可以在任何时间点启用新的同步字段，该字段的所有数据值都将从Dynamics CRM刷新到Marketo。不必再担心在初始设置期间必须选择所有字段。 如果您禁用现有同步字段并稍后重新启用它，则该字段的所有数据值都将从Dynamics CRM刷新到Marketo中。

**以联系人身份同步潜在客户**:“将潜在客户同步到Microsoft流”操作具有新选项，可以作为潜在客户或联系人进行同步。

![](assets/image2016-5-19-8-3a59-3a9.png)

**“同步错误管理”选项卡**:浏览、搜索或导出未能与操作、方向、错误代码和错误消息等详细信息同步的潜在客户（和其他对象）。

![](assets/sync-errors.png)

**Microsoft Dynamics 2016**:Connector经过充分认证，支持Dynamics 2016在线和内部部署版本。

**增效工具更新现在有文档说** 明：请 [参阅增效工具更新文档文章](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md)。

## [友好实例名称](/help/marketo/product-docs/administration/settings/edit-subscription-settings.md) {#friendly-instance-name}

如今，很难区分Marketo实例，例如沙箱和生产实例。 此功能可让您了解当前正在处理的实例。

![](assets/image2016-5-16-15-3a57-3a14.png)

## [限时访问订阅](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md) {#limited-time-access-for-subscriptions}

今天，用户将被邀请无限期使用Marketo 订阅。 此功能使管理员能够邀请用户在有限的时间段内访问订阅，例如，2周或1个月。

![](assets/image2016-5-16-15-3a59-3a52.png)

## [自定义对象网格](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) {#custom-objects-grid}

现在，您可以视图所有已发布自定义对象的记录和字段数。

![](assets/custom-objects-grid.png)

## 自定义活动{#custom-activities}

Marketo管理员现在可以通过Marketo自定义活动定义建模器定义和管理其自定义活动类型。 与Marketo自定义对象建模器相似（并与它一起），管理员现在可以扩展数据模型以满足其确切业务需求。 有关如何使用此功能的详细信息，请访问[Marketo文档站点](/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md)。

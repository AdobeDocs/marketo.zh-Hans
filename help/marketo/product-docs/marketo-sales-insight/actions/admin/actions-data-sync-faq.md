---
description: 操作数据同步常见问题解答 — Marketo文档 — 产品文档
title: 操作数据同步常见问题解答
feature: Sales Insight Actions
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 1%

---

# 操作数据同步常见问题解答 {#actions-data-sync-faq}

[!DNL Sales Insight Actions]的数据统一字段同步使系统能够将人员信息从Marketo Engage数据库提取到[!DNL Sales Insight Actions]数据库中。

这将提供[!DNL Sales Insight Actions] Web应用中的最新人员数据，并允许系统收集Marketo中相应人员记录的唯一ID以及[!DNL Salesforce]中的潜在客户/联系人/帐户/机会记录，以便能够正确引用记录以记录数据。

可以从Marketo Engage的“管理员”部分的“[!DNL Sales Insight Actions]”配置选项卡启用此同步。 有关详细信息，请查看[启动数据同步](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)。

![](assets/actions-data-sync-faq-1.png)

上图显示了人员活动和任务数据如何在系统之间同步。 需要注意以下几点：

* 人员记录已从Marketo Engage同步到[!DNL Sales Insight Actions]，从而使Marketo Engage成为[!DNL Sales Insight Actions]人员数据的真实来源
* Marketo Engage和[!DNL Sales Insight Actions] [都有一个机制](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)，用于收集取消订阅状态并将其同步到[!DNL Salesforce]
* 取消订阅状态不会从Sales Actions同步到Marketo Engage，但[!DNL Sales Insight Actions]可以配置为先检查人员的Marketo取消订阅状态，然后再允许销售人员发送包含[Marketo取消订阅检查](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)的电子邮件。

以下是有关数据统一同步如何工作的一些常见问题。

## 哪些潜在客户/联系人已同步到[!DNL Sales Insight Actions]？ {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

分配给销售负责人的销售线索和联系人将同步到Sales Actions。

您可以通过查看存在的标准所有者字段来查看潜在客户/联系人在[!DNL Salesforce]中是否有销售所有者。

销售负责人不必是Marketo同步用户或任何特定的[!DNL Salesforce]或销售用户。 我们只需在[!DNL Salesforce]中列出的潜在客户所有者和联系人所有者字段中列出一个用户，以便我们可以将其识别为销售潜在客户并将其同步到[!DNL Sales Insight Actions]中。 在[!DNL Sales Insight Actions]中还将检测到并更新与我们同步的字段的任何更新。

## Sales Insight智能网格中显示的活动数据源自何处？ {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

电子邮件、电话、有趣的时刻和Web等活动数据均源自Marketo Engage的数据库。 Sales Insight智能网格会向Marketo Engage实例发出请求，以便在每次销售用户加载Sales Insight面板时检索此内容。

![](assets/actions-data-sync-faq-4.png)

为确保所有活动数据均可来自Marketo Engage，[!DNL Sales Insight Actions]将所有活动数据同步到Marketo Engage。

## 哪些与从Marketo Engage同步到[!DNL Sales Insight Actions]的人员记录相关的字段？ {#what-fields-sync}

有11个字段从Marketo Engage同步到[!DNL Sales Insight Actions]：

* 名字
* 姓氏
* [!DNL Salesforce]联系人标识
* [!DNL Salesforce]潜在客户ID
* [!DNL Salesforce]帐户标识
* [!DNL Salesforce]机会ID
* Marketo ID
* 公司
* 标题
* 电子邮件
* 电话号码
* [!DNL Linkedin] URL
* 来源

## 在Marketo Engage和[!DNL Sales Insight Actions]之间同步的字段是否可以配置？ {#are-the-fields-that-sync-configurable}

无法配置同步到[!DNL Sales Insight Actions]的Marketo Engage字段，也无法映射字段。 从Marketo同步会自动将标准Marketo字段映射到销售活动实例中的标准字段。

## 为什么[!DNL Sales Insight Actions]有自己的数据库？ {#why-does-actions-have-its-own-database}

[!DNL Sales Insight Actions]拥有自己的Web应用程序，该应用程序具有专用的人员和活动数据库，可提供专为销售团队构建和设计的优化工作区。 这使销售经理和销售人员能够腾出空间来构建和管理他们的参与策略   无需授予主Marketo Engage工作区的访问权限或特权，该工作区已针对营销操作专家进行了优化。

## 如何处理重复项？ {#how-are-duplicates-handled}

您的Sales Actions数据库将成为Marketo Engage数据库中存在的合格人员（具有销售负责人的潜在客户/联系人）的副本。 这意味着，如果在Marketo中创建了具有相同电子邮件地址的两个记录，则在Sales Actions中将创建一个重复的记录。

## 完成初始同步需要多长时间？ {#how-long-initial-sync}

将所有销售线索数据同步到新[!DNL Sales Insight Actions]实例的初始流程通常每1-2分钟处理大约1,000人。 这只是个估计值，可能会有所不同。

执行初始同步并将所有潜在销售客户填充到您的[!DNL Sales Insight Actions] Web应用程序实例后，每次更新受支持的字段之一时都会运行增量同步。

## [!DNL Sales Insight Actions]用户能否从“操作”Web应用程序中编辑人员数据？ {#can-actions-users-edit-people-data}

不能，在“操作”Web应用程序的用户和管理员都不能创建和编辑“操作”中的人员记录。 必须在[!DNL Salesforce]或Marketo Engage中创建和编辑人员。 [!DNL Sales Insight Actions]通过持续同步新数据使用Marketo作为人员数据的真实来源，因此，如果在Marketo中通过Marketo中的工作流或从[!DNL Salesforce]同步了某个人员或创建了某个人员，则这些更新将传递到[!DNL Sales Insight Actions] Web应用程序数据库。

## 销售活动是否记录到Marketo？ {#do-sales-activities-log-to-marketo}

是，销售参与活动将作为本机活动登录到Marketo。 这些活动还包括本机过滤器，可与约束一起使用，以根据销售活动属性定位潜在客户。

![](assets/actions-data-sync-faq-5.png)

以下是登录到Marketo的活动列表：

* 发送销售电子邮件
* 打开销售电子邮件
* 点击销售电子邮件
* 已回复销售电子邮件
* 销售电子邮件已退回
* 已收到的销售电话
* 添加到销售活动
* 已从销售活动中移除

## 销售活动是否记录到[!DNL Salesforce]？ {#do-sales-activities-log-to-salesforce}

是，销售参与活动将作为本机任务登录到[!DNL Salesforce]。 然后，这些任务可以在[!DNL Salesforce]报表中使用，以便支持跟踪销售活动的团队功能板。

[!DNL Sales Insight Actions]允许管理员配置哪些销售活动记录到[!DNL Salesforce]。 这些活动包括电子邮件、呼叫和打开提醒任务。

![](assets/actions-data-sync-faq-6.png)

上图显示了记录到[!DNL Salesforce]的信息。 电子邮件和呼叫等活动在[!DNL Salesforce]单向同步[中记录到](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)。 [取消订阅](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)和[提醒任务](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)通过双向同步保持最新。 每个数据同步都可以从[!DNL Sales Insight Actions] Web应用程序界面进行配置。

>[!MORELIKETHIS]
>
>* [正在与 [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)同步取消订阅
>* [Marketo取消订阅检查](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [[!DNL Salesforce] 同步设置](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [提醒任务与 [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)同步
>* [启动数据同步](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)

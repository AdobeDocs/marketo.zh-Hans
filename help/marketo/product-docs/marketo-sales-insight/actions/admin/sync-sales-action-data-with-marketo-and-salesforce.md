---
description: 将Sales Action数据与Marketo和Salesforce同步 — Marketo文档 — 产品文档
title: 将销售活动数据与Marketo和Salesforce同步
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 1%

---

# 将销售活动数据与Marketo和Salesforce同步 {#sync-sales-action-data-with-marketo-and-salesforce}

Sales Insight Actions的数据统一字段同步使系统可以将Marketo Engage数据库中的人员信息提取到Sales Insight Actions数据库中。

这样可在Sales Insight Actions Web应用程序中提供最新的人员数据，并允许系统为Marketo中的相应人员记录和Salesforce中的潜在客户/联系人/客户/机会记录收集唯一ID，以便可以正确引用记录以供记录数据使用。

可以从Marketo Engage的“管理员”部分的“销售分析操作配置”选项卡中启用此同步。 有关详细信息，请查看 [启动数据同步](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

上图显示了人员活动和任务数据如何在系统之间同步。 需要注意以下几点：

* 人员记录从Marketo Engage同步到Sales Insight Actions ，使Marketo Engage成为Sales Insight Actions人员数据的真实来源
* Marketo Engage和销售分析操作 [有一个机制](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) 用于收集取消订阅状态并将其同步到Salesforce
* 取消订阅状态不会从Sales Actions同步到Marketo Engage，但Sales Insight Actions可以配置为在允许销售者发送电子邮件之前检查人员的Marketo取消订阅状态 [Marketo取消订阅检查](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

以下是一些与数据统一同步的工作方式相关的常见问题。

## 哪些潜在客户/联系人同步到Sales Insight Actions？ {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

为其分配了销售负责人的潜在客户和联系人将同步到Sales Actions中。

通过查看现有的标准责任人字段，您可以查看潜在客户/联系人在Salesforce中是否有销售责任人。

销售负责人不必是Marketo同步用户或任何特定的Salesforce或sales用户。 我们只需在Salesforce中列出的“销售线索所有者”和“联系人所有者”字段中列出一个用户，这样我们就可以将该用户标识为销售线索，并将其同步到Sales Insight Actions中。 与我们同步的字段的任何更新也将在Sales Insight Actions中检测和更新。

## Sales Insight智能网格中显示的活动数据源自何处？ {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

电子邮件、通话、趣味时刻、Web等活动数据均源自Marketo Engage的数据库。 Sales Insight Smart Grid向Marketo Engage实例发出请求，以便在每次销售User加载Sales Insight面板时检索此项。

![](assets/actions-data-sync-faq-4.png)

为确保所有活动数据都源自Marketo Engage， Sales Insight Actions会将所有活动数据同步到Marketo Engage。

## 与Marketo Engage记录同步到Sales Insight Actions的人员记录相关的字段有哪些？ {#what-fields-sync}

有11个字段可从Marketo Engage同步到Sales Insight Actions ：

* 名字
* 姓氏
* Salesforce联系人ID
* Salesforce潜在客户ID
* Salesforce帐户ID
* Salesforce机会ID
* Marketo ID
* 公司
* 标题
* 电子邮件
* 电话号码
* Linkedin URL
* 源

## 在Marketo Engage和Sales Insight Actions之间同步的字段是否可以配置？ {#are-the-fields-that-sync-configurable}

无法配置同步到Sales Insight Actions的Marketo Engage字段，也无法映射字段。 从Marketo同步会自动将标准Marketo字段映射到销售操作实例中的标准字段。

## 为什么Sales Insight Actions有它自己的数据库？ {#why-does-actions-have-its-own-database}

Sales Insight Actions拥有自己的Web应用程序，该应用程序具有专用的人员和活动数据库，可提供专为销售团队构建和设计的优化工作区。 这使销售经理和销售人员能够有一个空间来构建和管理他们的参与策略，而无需授予主Marketo Engage工作区的访问权限或特权，而主营销工作区是为营销运营专家而优化的。

## 如何处理重复项？ {#how-are-duplicates-handled}

您的Sales Actions数据库将是您的Marketo Engage数据库中存在的合格人员（具有销售负责人的潜在客户/联系人）的副本。 这意味着，如果在Marketo中创建了具有相同电子邮件地址的两个记录，则在Sales Actions中将创建一个重复的记录。

## 完成初始同步需要多长时间？ {#how-long-initial-sync}

将所有销售线索数据同步到新的Sales Insight Actions实例的初始过程通常每1-2分钟处理大约1,000人。 这只是一个估计值，可能会有所不同。

执行初始同步并将您的所有销售线索填充到您的Sales Insight Actions Web应用程序实例后，将会有一个增量同步，每次更新已同步的某个受支持字段时都会运行该同步。

## Sales Insight Actions用户能否从Actions Web应用程序中编辑人员数据？ {#can-actions-users-edit-people-data}

不能，在“操作”中创建和编辑人员记录的功能不适用于“操作”Web应用程序的用户和管理员。 必须在Salesforce或Marketo Engage中创建和编辑人员。 Sales Insight Actions通过不断同步新数据来使用Marketo作为人员数据的真实来源，因此，如果在Marketo中通过Marketo中的工作流或通过Salesforce同步人员来更新或创建人员，这些更新将传递到Sales Insight Actions Web应用程序数据库。

## 销售活动是否记录到Marketo？ {#do-sales-activities-log-to-marketo}

是，销售参与活动将作为本机活动登录到Marketo。 这些活动还包括本机过滤器，它们可与约束一起使用，以根据销售活动属性定位潜在客户。

![](assets/actions-data-sync-faq-5.png)

以下是登录到Marketo的活动列表：

* 发送销售电子邮件
* 打开销售电子邮件
* 单击销售电子邮件
* 已回复销售电子邮件
* 销售电子邮件已退回
* 已接的销售电话
* 添加到促销活动
* 已从销售活动中移除

## 销售活动是否记录到Salesforce？ {#do-sales-activities-log-to-salesforce}

是，销售参与活动将作为本机任务登录到Salesforce。 然后，这些任务可以在Salesforce报表中使用，以支持跟踪销售活动的团队功能板。

Sales Insight Actions允许管理员配置哪些销售活动记录到Salesforce。 这些活动包括电子邮件、呼叫和打开提醒任务。

![](assets/actions-data-sync-faq-6.png)

上图显示了哪些信息记录到Salesforce。 电子邮件和呼叫等活动记录到Salesforce中的 [单向同步](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md). [取消订阅](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) 和 [提醒任务](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) 通过双向同步保持最新。 其中每个数据同步都可以从Sales Insight Actions Web应用程序界面进行配置。

>[!MORELIKETHIS]
>
>* [正在与Salesforce同步取消订阅](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Marketo取消订阅检查](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [将Sales Activities同步到Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [与Salesforce同步提醒任务](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [启动数据同步](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)

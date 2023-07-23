---
description: Salesforce同步设置 — Marketo文档 — 产品文档
title: Salesforce同步设置
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 350490c93d8f2bcc278f9f3e82018a1db91a1146
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Salesforce同步设置 {#salesforce-sync-settings}

## 通过API将电子邮件活动记录到Salesforce {#logging-email-activity-to-salesforce-via-api}

此功能要求您使用Enterprise/Unlimited版的Salesforce，或者使用Professional版（如果您通过Web服务API购买了集成）。

>[!PREREQUISITES]
>
>必须连接Salesforce和Sales Insight Actions。

1. 在销售分析操作中，单击齿轮图标并选择 **设置**.

   ![](assets/salesforce-sync-settings-1.png)

1. 在“管理员设置”（如果您不是管理员，则为“我的帐户”）下，单击 **Salesforce**.

   ![](assets/salesforce-sync-settings-2.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/salesforce-sync-settings-3.png)

1. 单击“将电子邮件活动记录到Salesforce”旁边的箭头。

   ![](assets/salesforce-sync-settings-4.png)

1. 单击 **Salesforce API** 选项卡。 在此信息卡中，您可以设置用于将信息记录到Salesforce的首选项。 单击 **保存** 完成时。

   ![](assets/salesforce-sync-settings-5.png)

## 通过电子邮件将Email Activity记录到Salesforce (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

激活“Email to Salesforce (BCC)”后，您将收到销售电子邮件的密件抄送，并且您的电子邮件将记录为有关机会、潜在客户和联系人的活动。

>[!PREREQUISITES]
>
>必须连接Salesforce和Sales Insight Actions。

**通过电子邮件（密件抄送）在Salesforce中记录电子邮件**

1. 在Marketo Sales中，单击齿轮图标并选择 **设置**.

   ![](assets/salesforce-sync-settings-6.png)

1. 在“管理员设置”（如果您不是管理员，则为“我的帐户”）下，单击 **Salesforce**.

   ![](assets/salesforce-sync-settings-7.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/salesforce-sync-settings-8.png)

1. 单击 **发送电子邮件至Salesforce （密件抄送）** 选项卡，然后单击 **激活**.

   ![](assets/salesforce-sync-settings-9.png)

如果由于某种原因，您的Email to Salesforce地址未拉入，请按照以下步骤在Salesforce帐户中激活密件抄送功能：

1. 登录到Salesforce实例。
1. 在右上角找到您的用户名，然后选择下拉栏。
1. 选择 **我的设置**.
1. 选择 **电子邮件**.
1. 选择 **我给Salesforce的电子邮件**.
1. 在此页面上，您将看到一个标记为“Email to Salesforce Address”的字段。 如果旁边未填充任何内容，请向下滚动到“我的可接受电子邮件地址”。
1. 输入您希望进行密件抄送的电子邮件地址。
1. 单击 **保存更改**.

**在“我的设置”中找不到发送给Salesforce的电子邮件**

如果您在“设置”下未看到“我发送到Salesforce的电子邮件”，则可能是您的管理员未启用它。 如果您的团队不熟悉Salesforce，或者您的团队从未使用Salesforce提供的密件抄送地址，则可能发生这种情况。

>[!NOTE]
>
>您需要具有管理员权限才能进行此设置。

1. 单击 **设置**.
1. 单击 **电子邮件管理**.
1. 单击 **发送电子邮件至Salesforce**.
1. 单击 **编辑**.
1. 选中“活动”旁边的框。
1. 单击 **保存**.

## 将Sales Insight Actions任务/提醒同步到Salesforce任务 {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. 在销售分析操作中，单击齿轮图标并选择 **设置**.

   ![](assets/salesforce-sync-settings-10.png)

1. 在“管理员设置”（如果您不是管理员，则为“我的帐户”）下，单击 **Salesforce**.

   ![](assets/salesforce-sync-settings-11.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/salesforce-sync-settings-12.png)

1. 单击“将Marketo Sales Tasks/提醒同步到Salesforce Tasks”旁边的箭头。

   ![](assets/salesforce-sync-settings-13.png)

1. 选择所需的选项（默认情况下选中“不同步到Salesforce任务”）。

   ![](assets/salesforce-sync-settings-14.png)

## 首次将Sales Insight Actions任务与Salesforce同步 {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

当您首次打开Sales Insight Actions与Salesforce任务之间的同步时，我们会导入您的Salesforce任务。 我们不会将您在Sales Insight Actions中拥有的任何当前任务推送到Salesforce。 为了减少杂乱和重复项，从Sales Insight Actions同步到Salesforce中的唯一任务是在您将Sales Insight Actions与SFDC同步之后创建的任务。

以下是同步Sales Insight Actions和SFDC任务时会发生的情况：

在同步任务时单击“保存”后，它们就会开始进行同步。 这最初需要一些时间。

过去24小时内已更新或创建的任何提醒都将从SFDC拉入到Sales Insight Actions。 同步基于到期日期，所有这些任务将在后端进行同步，但在指挥中心，您只能看到今天和明天到期的任务。

如果以前启用了同步，并且您删除了SFDC中的任何任务，则过去15天内删除的任何任务都将从命令中心删除。

只要启用同步，我们就会不断在Sales Insight Actions和SFDC之间同步任务。

初次同步后，您在Sales Insight Actions中创建、编辑、完成或删除的任何任务都将同步到Salesforce中的任务列表。 在Salesforce中创建、编辑、完成或删除的任何内容，都将在Sales Insight Actions中更新您的任务列表。

要打开此同步，只需选中Web应用程序的“设置”页面中的同步框即可。

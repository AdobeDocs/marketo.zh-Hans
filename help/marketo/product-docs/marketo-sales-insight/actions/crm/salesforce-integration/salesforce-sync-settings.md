---
description: Salesforce同步设置 — Marketo文档 — 产品文档
title: Salesforce同步设置
hide: true
hidefromtoc: true
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
source-git-commit: 1db88a95777df43c3cef7ee5cabada2464329661
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Salesforce同步设置 {#salesforce-sync-settings}

## 通过API将电子邮件活动记录到Salesforce {#logging-email-activity-to-salesforce-via-api}

如果您已通过Web服务API购买了集成，则此功能要求您使用Salesforce的Enterprise/Unlimited版本，或Professional版本。

>[!PREREQUISITES]
>
>必须关联Salesforce和Sales Insight Actions。

1. 在Sales Insight Actions中，单击齿轮图标，然后选择 **设置**.

   ![](assets/salesforce-sync-settings-1.png)

1. 在“管理员设置”(或“我的帐户”（如果您不是管理员）下，单击 **Salesforce**.

   ![](assets/salesforce-sync-settings-2.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/salesforce-sync-settings-3.png)

1. 单击将电子邮件活动记录到Salesforce旁边的箭头。

   ![](assets/salesforce-sync-settings-4.png)

1. 单击 **Salesforce API** 选项卡。 在此卡中，您可以设置将信息记录到Salesforce的首选项。 单击 **保存** 完成时。

   ![](assets/salesforce-sync-settings-5.png)

## 通过电子邮件将电子邮件活动记录到Salesforce（密送） {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

激活“Email to Salesforce(BCC)”后，您将收到销售电子邮件的密件抄送，而您的电子邮件将作为活动记录在商机、潜在客户和联系人中。

>[!PREREQUISITES]
>
>必须关联Salesforce和Sales Insight Actions。

**通过电子邮件（密件抄送）在Salesforce中记录电子邮件**

1. 在Marketo Sales中，单击齿轮图标，然后选择 **设置**.

   ![](assets/salesforce-sync-settings-6.png)

1. 在“管理员设置”(或“我的帐户”（如果您不是管理员）下，单击 **Salesforce**.

   ![](assets/salesforce-sync-settings-7.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/salesforce-sync-settings-8.png)

1. 单击 **发送电子邮件至Salesforce（密送）** 选项卡，单击 **激活**.

   ![](assets/salesforce-sync-settings-9.png)

如果由于某些原因您的Email to Salesforce地址未提取，请按照以下步骤在您的Salesforce帐户中激活密送功能：

1. 登录到您的Salesforce实例。
1. 在右上角查找您的用户名，然后选择下拉栏。
1. 选择 **我的设置**.
1. 选择 **电子邮件**.
1. 选择 **我发送给Salesforce的电子邮件**.
1. 在此页面上，您将看到一个标有“Email to Salesforce Address”的字段。 如果其旁边未填充任何内容，请向下滚动到“我可接受的电子邮件地址”。
1. 输入要密件抄送的电子邮件地址。
1. 单击 **保存更改**.

**在“我的设置”中找不到我发送给Salesforce的电子邮件**

如果您在“设置”下未看到“我向Salesforce发送的电子邮件”，则您的管理员可能尚未启用该设置。 如果您的团队是Salesforce的新团队，或者您的团队从未使用Salesforce提供的密件抄送地址，则可能会发生这种情况。

>[!NOTE]
>
>您需要管理员权限才能设置此设置。

1. 单击 **设置**.
1. 单击 **电子邮件管理**.
1. 单击 **发送电子邮件至Salesforce**.
1. 单击 **编辑**.
1. 选中“活动”旁边的复选框。
1. 单击 **保存**.

## 将Sales Insight操作任务/提醒同步到Salesforce任务 {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. 在Sales Insight Actions中，单击齿轮图标，然后选择 **设置**.

   ![](assets/salesforce-sync-settings-10.png)

1. 在“管理员设置”(或“我的帐户”（如果您不是管理员）下，单击 **Salesforce**.

   ![](assets/salesforce-sync-settings-11.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/salesforce-sync-settings-12.png)

1. 单击将Marketo Sales Tasks/Rements同步到Salesforce Tasks旁边的箭头。

   ![](assets/salesforce-sync-settings-13.png)

1. 选择所需的选项（默认情况下选中“不同步到Salesforce任务”）。

   ![](assets/salesforce-sync-settings-14.png)

## 首次将销售分析操作任务与Salesforce同步 {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

首次打开Sales Insight Actions和Salesforce任务之间的同步时，我们会导入您的Salesforce任务。 我们不会将您在Sales Insight Actions中拥有的任何当前任务推送到Salesforce。 为了减少混乱和重复项，从Sales Insight Actions同步到Salesforce中的唯一任务是在将Sales Insight Actions与SFDC同步之后创建的任务。

以下是同步Sales Insight操作和SFDC任务时发生的情况：

单击“保存任务”同步后，这些任务即开始同步。 这最初需要一些时间。

在过去24小时内更新或创建的任何提醒都将从SFDC提取到Sales Insight Actions。 同步基于到期日期，所有这些任务都将在后端同步，但在命令中心，您将只看到今天和明天到期的任务。

如果之前已打开同步，并且您删除了SFDC中的任何任务，则过去15天内删除的任何任务都将从命令中心删除。

只要启用了同步，我们就会在Sales Insight Actions和SFDC之间不断同步任务。

在初始同步之后，您在Sales Insight Actions中创建、编辑、完成或删除的任何任务都将同步到Salesforce中的任务列表。 而且，在Salesforce中创建、编辑、完成或删除的任何内容都将更新Sales Insight Actions中的任务列表。

要打开此同步，只需在Web应用程序的“设置”页面中选中同步框。

---
description: Salesforce同步设置 — Marketo文档 — 产品文档
title: Salesforce同步设置
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 1%

---

# [!DNL Salesforce]同步设置 {#salesforce-sync-settings}

## 通过API将电子邮件活动记录到[!DNL Salesforce] {#logging-email-activity-to-salesforce-via-api}

此功能要求您使用[!DNL Salesforce]的Enterprise/Unlimited版本，或者是Professional版本（如果您已通过Web服务API购买集成）。

>[!PREREQUISITES]
>
>[!DNL Salesforce]和[!DNL Sales Insight Actions]必须连接。

1. 在[!DNL Sales Insight Actions]中，单击齿轮图标并选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/salesforce-sync-settings-1.png)

1. 在[!UICONTROL Admin Settings]（如果您不是管理员，则单击“[!UICONTROL My Account]”）下，单击&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/salesforce-sync-settings-2.png)

1. 单击&#x200B;**[!UICONTROL Sync Settings]**&#x200B;选项卡。

   ![](assets/salesforce-sync-settings-3.png)

1. 单击[!UICONTROL Log Email Activity]到[!DNL Salesforce]旁边的箭头。

   ![](assets/salesforce-sync-settings-4.png)

1. 单击&#x200B;**[!UICONTROL Salesforce API]**&#x200B;选项卡。 在此信息卡中，您可以设置用于将信息记录到[!DNL Salesforce]的首选项。 完成后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/salesforce-sync-settings-5.png)

## 通过电子邮件将电子邮件活动记录到[!DNL Salesforce]，发送电子邮件给[!DNL Salesforce] （密件抄送） {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

激活“[!UICONTROL Email to Salesforce (BCC)]”后，您将收到销售电子邮件的“密件抄送”，您的电子邮件将记录为商机、潜在客户和联系人的活动。

>[!PREREQUISITES]
>
>[!DNL Salesforce]和[!DNL Sales Insight Actions]必须连接。

**通过电子邮件在[!DNL Salesforce]中记录电子邮件（密件抄送）**

1. 在Marketo Sales中，单击齿轮图标并选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/salesforce-sync-settings-6.png)

1. 在[!UICONTROL Admin Settings]（如果您不是管理员，则单击“[!UICONTROL My Account]”）下，单击&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/salesforce-sync-settings-7.png)

1. 单击&#x200B;**[!UICONTROL Sync Settings]**&#x200B;选项卡。

   ![](assets/salesforce-sync-settings-8.png)

1. 单击&#x200B;**[!UICONTROL Email to Salesforce (BCC)]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL Activate]**。

   ![](assets/salesforce-sync-settings-9.png)

如果由于某种原因导致您发送到[!DNL Salesforce]的电子邮件地址无法提取，请按照以下步骤在您的[!DNL Salesforce]帐户中激活密件抄送功能：

1. 登录到您的[!DNL Salesforce]实例。
1. 在右上角找到您的用户名，然后选择下拉栏。
1. 选择 **[!UICONTROL My Settings]**。
1. 选择 **[!UICONTROL Email]**。
1. 选择 **[!UICONTROL My Email to Salesforce]**。
1. 在此页面上，您将看到一个标记为“[!UICONTROL Email to Salesforce Address]”的字段。 如果旁边未填充任何内容，请向下滚动到“[!UICONTROL My Acceptable Email Addresses]”。
1. 输入您希望密件抄送的电子邮件地址。
1. 单击 **[!UICONTROL Save Changes]**。

**在“我的设置”中找不到我发送给[!DNL Salesforce]的电子邮件**

如果在您的“设置”下未看到“我的发送至[!DNL Salesforce]的电子邮件”，则可能是您的管理员未启用它。 如果您的团队是[!DNL Salesforce]的新用户，或者您的团队从未使用[!DNL Salesforce]提供的密件抄送地址，则可能发生这种情况。

>[!NOTE]
>
>您需要管理员权限才能设置此项。

1. 单击 **[!UICONTROL Setup]**。
1. 单击 **[!UICONTROL Email Administration]**。
1. 单击 **[!UICONTROL Email to Salesforce]**。
1. 单击 **[!UICONTROL Edit]**。
1. 选中“活动”旁边的框。
1. 单击 **[!UICONTROL Save]**。

## 将[!DNL Sales Insight Actions]任务/提醒同步到[!DNL Salesforce]任务 {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. 在[!DNL Sales Insight Actions]中，单击齿轮图标并选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/salesforce-sync-settings-10.png)

1. 在[!UICONTROL Admin Settings]（如果您不是管理员，则单击“[!UICONTROL My Account]”）下，单击&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/salesforce-sync-settings-11.png)

1. 单击&#x200B;**[!UICONTROL Sync Settings]**&#x200B;选项卡。

   ![](assets/salesforce-sync-settings-12.png)

1. 单击“将Marketo销售任务/提醒同步到[!DNL Salesforce]任务”旁边的箭头。

   ![](assets/salesforce-sync-settings-13.png)

1. 选择所需的选项（默认情况下选中“不同步到[!DNL Salesforce]任务”）。

   ![](assets/salesforce-sync-settings-14.png)

## 首次将[!DNL Sales Insight Actions]任务与[!DNL Salesforce]同步 {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

当您首次打开[!DNL Sales Insight Actions]和[!DNL Salesforce]任务之间的同步时，我们会导入您的[!DNL Salesforce]任务。 我们不会将您在[!DNL Sales Insight Actions]中拥有的任何当前任务推送到[!DNL Salesforce]。 为了减少杂乱和重复项，从[!DNL Sales Insight Actions]同步到[!DNL Salesforce]的任务只包括在您与SFDC同步[!DNL Sales Insight Actions]之后创建的任务。

以下是同步[!DNL Sales Insight Actions]和SFDC任务时发生的情况：

在同步的任务上单击“保存”后，它们就会开始进行同步。 这最初将需要一些时间。

过去24小时内已更新或创建的任何提醒都将从SFDC拉入[!DNL Sales Insight Actions]。 同步基于到期日期，所有这些任务将在后端进行同步，但在命令中心，您只能看到今天和明天到期的任务。

如果以前启用了同步，并且您删除了SFDC中的任何任务，则过去15天内删除的任何任务都将从命令中心删除。

只要已启用同步，我们就会一直在[!DNL Sales Insight Actions]和SFDC之间同步任务。

初始同步后，您在[!DNL Sales Insight Actions]中创建、编辑、完成或删除的任何任务都将同步到[!DNL Salesforce]中的任务列表。 在[!DNL Salesforce]中创建、编辑、完成或删除的任何内容都将在[!DNL Sales Insight Actions]中更新您的任务列表。

要打开此同步，只需选中Web应用程序中[!UICONTROL Settings]页面中的同步框。

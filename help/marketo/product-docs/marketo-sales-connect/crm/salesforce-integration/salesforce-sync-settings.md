---
unique-page-id: 18317669
description: Salesforce同步设置 — Marketo文档 — 产品文档
title: Salesforce 同步设置
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 5%

---

# Salesforce 同步设置 {#salesforce-sync-settings}

## 通过API将电子邮件活动记录到Salesforce {#logging-email-activity-to-salesforce-via-api}

此功能要求您使用Salesforce的Enterprise/Unlimited版本或Professional版本（如果您已通过Web服务API购买集成）。

>[!PREREQUISITES]
>
>必须连接Salesforce和Sales Connect。

1. 在[!DNL Sales Connect]中，单击右上角的齿轮图标，然后选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/one-2.png)

1. 在[!UICONTROL My Account] ([!UICONTROL Admin Settings]（如果您是管理员）)下，单击&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/two-2.png)

1. 单击&#x200B;**[!UICONTROL Sync Settings]**&#x200B;选项卡。

   ![](assets/three-1.png)

1. 单击“将电子邮件活动记录到[!DNL Salesforce]”旁边的箭头。

   ![](assets/four-1.png)

1. 单击 **[!UICONTROL Salesforce API]** 选项卡。在此信息卡中，您可以设置用于将信息记录到[!DNL Salesforce]的首选项。 完成后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/five.png)

## 通过电子邮件将电子邮件活动记录到Salesforce到Salesforce （密送） {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

激活“发送电子邮件至Salesforce （密送）”后，您将收到销售电子邮件的密送，并且您的电子邮件将记录为有关机会、潜在客户和联系人的活动。

>[!PREREQUISITES]
>
>[!DNL Salesforce]和[!DNL Sales Connect]必须连接。

**通过电子邮件在Salesforce中记录电子邮件（密件抄送）**

1. 在[!UICONTROL Sales Connect]中，单击右上角的齿轮图标，然后选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/one-3.png)

1. 在[!UICONTROL My Account] ([!UICONTROL Admin Settings]（如果您是管理员）)下，单击&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/two-3.png)

1. 单击&#x200B;**[!UICONTROL Sync Settings]**&#x200B;选项卡。

   ![](assets/three-1.png)

1. 单击&#x200B;**[!UICONTROL Email to Salesforce (BCC)]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL Activate]**。

   ![](assets/six-2.png)

如果由于某种原因导致您发送到[!DNL Salesforce]的电子邮件地址无法提取，请按照以下步骤在您的[!DNL Salesforce]帐户中激活密件抄送功能：

1. 登录到您的[!DNL Salesforce]实例。
1. 在右上角找到您的用户名，然后选择下拉栏。
1. 选择 **[!UICONTROL My Settings]**。
1. 选择 **[!UICONTROL Email]**。
1. 选择 **[!UICONTROL My Email to Salesforce]**。
1. 在此页面上，您将看到一个标记为“发送到Salesforce地址的电子邮件”的字段。 如果旁边未填充任何内容，请向下滚动到“我的可接受电子邮件地址”。
1. 输入您希望密件抄送的电子邮件地址。
1. 单击 **[!UICONTROL Save Changes]**。

**在“我的设置”中找不到我发送给[!DNL Salesforce]的电子邮件**

如果在“设置”下未看到“我发送到Salesforce的电子邮件”，则可能是因为管理员未启用它。 如果您的团队是[!DNL Salesforce]的新用户，或者您的团队从未使用[!DNL Salesforce]提供的密件抄送地址，则可能发生这种情况。

>[!NOTE]
>
>您需要管理员权限才能设置此项。

1. 单击 **[!UICONTROL Setup]**。
1. 单击 **[!UICONTROL Email Administration]**。
1. 单击 **[!UICONTROL Email to Salesforce]**。
1. 单击 **[!UICONTROL Edit]**。
1. 选中“[!UICONTROL Active]”旁边的框。
1. 单击 **[!UICONTROL Save]**。

## 将Sales Connect任务/提醒同步到[!DNL Salesforce]任务 {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. 单击右上角的齿轮图标并选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/one-3.png)

1. 在[!UICONTROL My Account] ([!UICONTROL Admin Settings]（如果您是管理员）)下，单击&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/two-2.png)

1. 单击&#x200B;**[!UICONTROL Sync Settings]**&#x200B;选项卡。

   ![](assets/three-1.png)

1. 单击[!UICONTROL Sync Sales Engage Tasks/Reminders to Salesforce Tasks]旁边的箭头。

   ![](assets/seven-2.png)

1. 选择所需的选项（默认情况下已选中“[!UICONTROL Do not sync to Salesforce tasks]”）。

   ![](assets/eight.png)

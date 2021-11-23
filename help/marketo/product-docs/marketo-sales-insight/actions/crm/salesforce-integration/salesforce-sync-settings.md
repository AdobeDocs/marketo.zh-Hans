---
description: Salesforce同步设置 — Marketo文档 — 产品文档
title: Salesforce同步设置
hide: true
hidefromtoc: true
source-git-commit: d3e8e85bd8b428b2490a44e44fdab9d58784843d
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Salesforce同步设置 {#salesforce-sync-settings}

## 通过API将电子邮件活动记录到Salesforce {#logging-email-activity-to-salesforce-via-api}

如果您已通过Web服务API购买了集成，则此功能要求您使用Salesforce的Enterprise/Unlimited版本，或Professional版本。

>[!PREREQUISITES]
>
>必须连接Salesforce和Marketo Sales。

1. 在Marketo Sales中，单击齿轮图标，然后选择 **设置**.

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
>必须连接Salesforce和Marketo Sales。

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

## 将Marketo销售任务/提醒同步到Salesforce任务 {#sync-marketo-sales-tasks-reminders-to-salesforce-tasks}

1. 在Marketo Sales中，单击齿轮图标，然后选择 **设置**.

   ![](assets/salesforce-sync-settings-10.png)

1. 在“管理员设置”(或“我的帐户”（如果您不是管理员）下，单击 **Salesforce**.

   ![](assets/salesforce-sync-settings-11.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/salesforce-sync-settings-12.png)

1. 单击将Marketo Sales Tasks/Rements同步到Salesforce Tasks旁边的箭头。

   ![](assets/salesforce-sync-settings-13.png)

1. 选择所需的选项（默认情况下选中“不同步到Salesforce任务”）。

   ![](assets/salesforce-sync-settings-14.png)

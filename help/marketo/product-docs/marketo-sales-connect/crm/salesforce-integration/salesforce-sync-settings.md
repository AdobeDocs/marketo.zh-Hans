---
unique-page-id: 18317669
description: Salesforce同步设置 — Marketo文档 — 产品文档
title: Salesforce同步设置
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
source-git-commit: 56db82ef98d774f8ac56c1401ef7ef275862d1dc
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Salesforce同步设置 {#salesforce-sync-settings}

## 通过API将电子邮件活动记录到Salesforce {#logging-email-activity-to-salesforce-via-api}

如果您已通过Web服务API购买了集成，则此功能要求您使用Salesforce的Enterprise/Unlimited版本，或Professional版本。

>[!PREREQUISITES]
>
>必须连接Salesforce和Sales Connect。

1. 在Sales Connect中，单击右上角的齿轮图标，然后选择 **设置**.

   ![](assets/one-2.png)

1. 在“我的帐户”（如果您是管理员，请单击“管理员设置”）下 **Salesforce**.

   ![](assets/two-2.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/three-1.png)

1. 单击将电子邮件活动记录到Salesforce旁边的箭头。

   ![](assets/four-1.png)

1. 单击 **Salesforce API** 选项卡。 在此卡中，您可以设置将信息记录到Salesforce的首选项。 单击 **保存** 完成时。

   ![](assets/five.png)

## 通过电子邮件将电子邮件活动记录到Salesforce（密送） {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

激活“Email to Salesforce(BCC)”后，您将收到销售电子邮件的密件抄送，而您的电子邮件将作为活动记录在商机、潜在客户和联系人中。

>[!PREREQUISITES]
>
>必须连接Salesforce和Sales Connect。

**通过电子邮件（密件抄送）在Salesforce中记录电子邮件**

1. 在Sales Connect中，单击右上角的齿轮图标，然后选择 **设置**.

   ![](assets/one-3.png)

1. 在“我的帐户”（如果您是管理员，请单击“管理员设置”）下 **Salesforce**.

   ![](assets/two-3.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/three-1.png)

1. 单击 **发送电子邮件至Salesforce（密送）** 选项卡，单击 **激活**.

   ![](assets/six-2.png)

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

## 将Sales Connect任务/提醒同步到Salesforce任务 {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. 单击右上角的齿轮图标，然后选择 **设置**.

   ![](assets/one-3.png)

1. 在“我的帐户”（如果您是管理员，请单击“管理员设置”）下 **Salesforce**.

   ![](assets/two-2.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/three-1.png)

1. 单击将Sales Connect Tasks/Rements（销售连接任务/提醒）与Salesforce Tasks（Salesforce任务）同步旁边的箭头。

   ![](assets/seven-2.png)

1. 选择所需的选项（默认情况下选中“不同步到Salesforce任务”）。

   ![](assets/eight.png)

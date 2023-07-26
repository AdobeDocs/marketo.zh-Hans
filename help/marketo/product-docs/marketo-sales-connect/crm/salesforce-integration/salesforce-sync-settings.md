---
unique-page-id: 18317669
description: Salesforce同步设置 — Marketo文档 — 产品文档
title: Salesforce同步设置
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Salesforce同步设置 {#salesforce-sync-settings}

## 通过API将电子邮件活动记录到Salesforce {#logging-email-activity-to-salesforce-via-api}

此功能要求您使用Enterprise/Unlimited版的Salesforce，或者是Professional版（如果您通过Web Services API购买了集成）。

>[!PREREQUISITES]
>
>Salesforce和Sales Connect必须连接。

1. 在Sales Connect中，单击右上角的齿轮图标，然后选择 **设置**.

   ![](assets/one-2.png)

1. 在“我的帐户（管理员设置，如果您是管理员）”下，单击 **Salesforce**.

   ![](assets/two-2.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/three-1.png)

1. 单击“将电子邮件活动记录到Salesforce”旁边的箭头。

   ![](assets/four-1.png)

1. 单击 **Salesforce API** 选项卡。 在此信息卡中，您可以设置用于将信息记录到Salesforce的首选项。 单击 **保存** 完成时。

   ![](assets/five.png)

## 通过电子邮件将Email Activity记录到Salesforce (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

激活“发送电子邮件至Salesforce （密件抄送）”后，您将收到销售电子邮件的密件抄送，并且您的电子邮件将记录为有关机会、潜在客户和联系人的活动。

>[!PREREQUISITES]
>
>Salesforce和Sales Connect必须连接。

**通过电子邮件在Salesforce中记录电子邮件（密送）**

1. 在Sales Connect中，单击右上角的齿轮图标，然后选择 **设置**.

   ![](assets/one-3.png)

1. 在“我的帐户（管理员设置，如果您是管理员）”下，单击 **Salesforce**.

   ![](assets/two-3.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/three-1.png)

1. 单击 **发送到Salesforce的电子邮件（密件抄送）** 选项卡，然后单击 **激活**.

   ![](assets/six-2.png)

如果由于某种原因导致您发送到Salesforce的电子邮件地址无法提取，请按照以下步骤在Salesforce帐户中激活密件抄送功能：

1. 登录到Salesforce实例。
1. 在右上角找到您的用户名，然后选择下拉栏。
1. 选择 **我的设置**.
1. 选择 **电子邮件**.
1. 选择 **发送给Salesforce的电子邮件**.
1. 在此页面上，您将看到一个标记为“Email to Salesforce Address”的字段。 如果旁边未填充任何内容，请向下滚动到“我的可接受电子邮件地址”。
1. 输入您希望密件抄送的电子邮件地址。
1. 单击 **保存更改**.

**在“我的设置”中找不到发送给Salesforce的电子邮件**

如果在您的“设置”下未看到“我发送到Salesforce的电子邮件”，则可能是管理员未启用它。 如果您的团队不熟悉Salesforce，或者您的团队从未使用Salesforce提供的密件抄送地址，则可能会发生这种情况。

>[!NOTE]
>
>您需要管理员权限才能设置此项。

1. 单击 **设置**.
1. 单击 **电子邮件管理**.
1. 单击 **发送电子邮件至Salesforce**.
1. 单击 **编辑**.
1. 选中“活动”旁边的框。
1. 单击 **保存**.

## 将Sales Connect任务/提醒同步到Salesforce任务 {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. 单击右上角的齿轮图标并选择 **设置**.

   ![](assets/one-3.png)

1. 在“我的帐户（管理员设置，如果您是管理员）”下，单击 **Salesforce**.

   ![](assets/two-2.png)

1. 单击 **同步设置** 选项卡。

   ![](assets/three-1.png)

1. 单击Sync Sales Connect Tasks/Reminders to Salesforce Tasks旁边的箭头。

   ![](assets/seven-2.png)

1. 选择所需的选项（默认情况下选中“不同步到Salesforce任务”）。

   ![](assets/eight.png)

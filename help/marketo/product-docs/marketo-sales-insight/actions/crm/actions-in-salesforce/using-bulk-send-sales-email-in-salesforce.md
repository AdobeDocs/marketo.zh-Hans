---
description: 在Salesforce中使用批量发送销售电子邮件 — Marketo文档 — 产品文档
title: 在Salesforce中使用批量发送销售电子邮件
exl-id: eac77a64-7eaa-48eb-820c-c8e188a234dd
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# 在Salesforce中使用批量发送销售电子邮件 {#using-bulk-send-sales-email-in-salesforce}

了解如何在Salesforce中发送批量电子邮件，以帮助使用Sales Actions扩展出站通信。

>[!NOTE]
>
>Salesforce强制实施一次可选择200条记录的限制。

>[!PREREQUISITES]
>
>确保您已安装 [最新的Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} to your Salesforce instance and have configured the [Action buttons](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/add-action-buttons-to-salesforce-list-view.md){target="_blank"} Salesforce中的联系人和潜在客户列表视图。

## 使用Salesforce Lightning发送批量电子邮件 {#sending-bulk-email-in-salesforce-lightning}

1. 在Salesforce中，通过单击 **潜在客户/联系人** 选项卡。

   ![](assets/using-bulk-send-sales-email-in-salesforce-1.png)

1. 在“视图”下拉列表中，选择要通过电子邮件发送的潜在客户/联系人所需视图。

   >[!TIP]
   >
   >您可以创建新视图，方法是单击右侧的齿轮图标并选择 **新建**. 为视图指定新名称并保存它后，您可以单击右侧的过滤器图标以帮助向下过滤到要通过电子邮件发送的潜在客户/联系人集。

1. 选择所需的潜在客户或联系人列表，然后单击 **发送销售电子邮件** 按钮。

   ![](assets/using-bulk-send-sales-email-in-salesforce-2.png)

1. 系统将导航到“操作撰写”窗口，并添加您选定的人员。

1. 选择要插入到操作撰写窗口编辑器中的模板或编写自定义电子邮件。

   >[!TIP]
   >
   >使用 [固定类别](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} 更轻松地访问您喜爱的电子邮件模板。

   **可选步骤**：通过单击 **预览动态字段** 按钮。

   >[!TIP]
   >
   >如果要为所有收件人自定义模板，请单击批量撰写侧边栏中的所有收件人选项，以便同时编辑所有收件人电子邮件。 如果要更改特定电子邮件，请在批量撰写侧边栏中单击收件人的姓名或电子邮件。 请注意，如果您在选择“所有收件人”时更改了单个电子邮件，那么对“所有收件人”所做的更改将覆盖对单个电子邮件所做的更改。

1. 选择 **发送** 立即发送电子邮件，或者 **设置计划** 设置发送电子邮件的日期和时间。

   ![](assets/using-bulk-send-sales-email-in-salesforce-3.png)

## 在Salesforce Classic中发送批量电子邮件 {#sending-bulk-email-in-salesforce-classic}

1. 在Salesforce中，单击 **潜在客户/联系人** 选项卡。

1. 在“视图”下拉列表中，选择要通过电子邮件发送的潜在客户/联系人所需视图，然后单击 **开始**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-4.png)

   >[!TIP]
   >
   >您可以创建新视图，方法是单击创建新视图并配置可用过滤器，以缩小要添加到促销活动中的人员列表。

1. 选择所需的潜在客户或联系人列表，然后单击 **发送销售电子邮件** 按钮。

   ![](assets/using-bulk-send-sales-email-in-salesforce-5.png)

1. 系统将导航到操作撰写窗口，其中包含您在撰写窗口中选择的收件人。

1. 选择要插入到操作撰写窗口编辑器中的模板，或编写自定义电子邮件。

   ![](assets/using-bulk-send-sales-email-in-salesforce-6.png)

   >[!TIP]
   >
   >使用 [固定类别](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} 更轻松地访问您喜爱的电子邮件模板。

   **可选步骤**：通过单击 **预览动态字段** 按钮。

   >[!TIP]
   >
   >如果要为所有收件人自定义模板，请单击批量撰写侧边栏中的所有收件人选项，以便同时编辑所有收件人电子邮件。 如果要更改特定电子邮件，请在批量撰写侧边栏中单击收件人的姓名或电子邮件。 请注意，如果您在选择“所有收件人”时更改了单个电子邮件，那么对“所有收件人”所做的更改将覆盖对单个电子邮件所做的更改。

1. 选择 **发送** 立即发送电子邮件，或者 **设置计划** 设置发送电子邮件的日期和时间。

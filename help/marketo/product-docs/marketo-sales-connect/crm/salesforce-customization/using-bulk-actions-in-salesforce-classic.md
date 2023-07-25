---
unique-page-id: 42762794
description: Salesforce Classic中的批量操作 — Marketo文档 — 产品文档
title: 在Salesforce Classic中使用批量操作
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# 在Salesforce Classic中使用批量操作 {#using-bulk-actions-in-salesforce-classic}

了解如何执行批量操作，如将潜在客户添加到营销活动、发送批量电子邮件或将潜在客户从Salesforce推送到Sales Connect。

>[!PREREQUISITES]
>
>请更新到Sales Connect软件包的最新版本，并在潜在客户/联系人视图上安装批量操作按钮。 [单击此处获取说明](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>在执行以下列出的步骤之前，请确保已登录到您的Marketo Sales Connect帐户。

## 批量电子邮件 {#bulk-email}

1. 在Salesforce中，单击 **潜在客户** 选项卡，然后 **开始** 按钮。

   ![](assets/one-5.png)

1. 选择所需的潜在客户，然后单击 **使用MSC (Classic)发送电子邮件** 按钮。

   ![](assets/two-5.png)

1. 此时会弹出一个MSC电子邮件。 它包括以下功能：

   答：“至”字段显示“所有接收” — 这与您在“销售线索列表视图”中选择的销售线索列表相对应\
   b.此列表显示在名为“批量撰写”的左侧面板中 — 您可以在此处添加/删除收件人\
   c.您可以选择模板或创建自己的电子邮件\
   d.您可以预览将在电子邮件中填充的动态字段\
   e.您可以立即发送电子邮件，也可以安排在以后发送

   ![](assets/three-4.png)

## 添加到营销活动 {#add-to-campaign}

1. 在Salesforce中，单击 **潜在客户** 选项卡，然后 **开始** 按钮。

   ![](assets/four-3.png)

1. 选择所需的潜在客户，然后单击 **添加到MSC Campaign (Classic)** 按钮。

   ![](assets/five-3.png)

1. 此时将显示“将人员添加到您的营销活动”弹出窗口。 单击 **下一个** 并完成典型促销活动流程以触发MSC促销活动。

   ![](assets/six.png)

## 推送到Marketo Sales Connect {#push-to-marketo-sales-connect}

1. 在Salesforce中，单击 **潜在客户** 选项卡，然后 **开始** 按钮。

   ![](assets/seven-1.png)

1. 选择所需的潜在客户，然后单击 **推送到MSC（经典）** 按钮。

   ![](assets/eight-1.png)

1. 将打开一个名为“Salesforce Bridge”的新选项卡。 单击 **转到组→** 按钮。

   ![](assets/nine-1.png)

1. 系统会将您发送到您的MSC帐户，您将在其中看到一个使用日期/时间戳创建的组。 同步完成后，您将收到通知，该组将包括从Salesforce同步的潜在客户。

   ![](assets/ten.png)

>[!NOTE]
>
>您也可以按照与在“联系人列表”视图中使用批量操作相同的步骤进行操作。

>[!MORELIKETHIS]
>
>* [通过群电子邮件发送电子邮件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [使用“选择并发送”撰写批量电子邮件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)

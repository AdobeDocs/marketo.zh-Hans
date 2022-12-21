---
unique-page-id: 42762825
description: 在Salesforce Lightning中使用批量操作 — Marketo文档 — 产品文档
title: 在Salesforce闪电中使用批量操作
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 在Salesforce闪电中使用批量操作 {#using-bulk-actions-in-salesforce-lightning}

了解如何执行批量操作，例如向营销活动添加潜在客户、发送批量电子邮件或将潜在客户从Salesforce推送到Sales Connect。

>[!PREREQUISITES]
>
>更新至Sales Connect软件包的最新版本，并在潜在客户/联系人视图中安装批量操作按钮。 [单击此处获取相关说明](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf).

>[!NOTE]
>
>在执行以下步骤之前，请确保您已登录到Marketo Sales Connect帐户。

## 批量电子邮件 {#bulk-email}

1. 在Salesforce中，单击 **潜在客户** ，然后选择所需潜在客户的列表。

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >如果您已经在将要使用的列表上，则必须再次执行该列表，方法是从下拉列表中选择该列表，以确保MSC批量操作按钮显示。 这是无法更改的Salesforce行为。

1. 单击箭头下拉菜单（位于屏幕的最右侧），然后选择 **使用MSC发送电子邮件**.

   ![](assets/two-6.png)

1. 将弹出MSC电子邮件。 它包括以下功能：

   a.“收件人”字段显示“所有收据” — 此字段对应于您在“潜在客户列表视图”中选择的潜在客户列表\
   b.此列表显示在名为“批量撰写”的左侧面板上 — 您可以在此处添加/删除收件人\
   c.您可以选择模板或创建自己的电子邮件\
   d.您可以立即发送电子邮件，也可以安排稍后发送

   ![](assets/three-5.png)

## 添加到Campaign {#add-to-campaign}

1. 在Salesforce中，单击 **潜在客户** ，然后选择所需潜在客户的列表。

   ![](assets/four-4.png)

1. 单击箭头下拉菜单（位于屏幕的最右侧），然后选择 **添加到MSC Campaign**.

   ![](assets/five-4.png)

1. 将显示“将人员添加到您的营销活动”弹出窗口。 单击 **下一个** 并浏览典型的营销活动流程以触发MSC营销活动。

   ![](assets/six-1.png)

## 推送到Marketo Sales Connect {#push-to-marketo-sales-connect}

1. 在Salesforce中，单击 **潜在客户** ，然后选择所需潜在客户的列表。

   ![](assets/seven-2.png)

1. 单击箭头下拉菜单（位于屏幕的最右侧），然后选择 **推送到MSC**.

   ![](assets/eight-2.png)

1. 将打开一个名为“Salesforce桥”的新选项卡。 单击 **进入组→** 按钮。

   ![](assets/nine-2.png)

1. 您将被发送到您的MSC帐户，在该帐户中，您将看到创建的组具有日期/时间戳。 同步完成后，您将收到通知，并且组将包含从Salesforce同步的潜在客户。

   ![](assets/ten-1.png)

>[!NOTE]
>
>也可以按照相同的步骤在“联系人列表视图”中使用批量操作。

>[!MORELIKETHIS]
>
>* [通过群组电子邮件发送电子邮件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [使用选择并发送来合成批量电子邮件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)


---
unique-page-id: 13795727
description: 中止使用收件人时区计划的电子邮件程序的交付 — Marketo文档 — 产品文档
title: 中止使用收件人时区计划的电子邮件程序的发送
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# 中止使用收件人时区计划的电子邮件程序的发送 {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

在紧急情况下，您可以中止已在启用“收件人时区”的情况下开始运行的电子邮件程序的投放。

由于与收件人时区一起计划的电子邮件程序最长可以运行24小时，因此中止程序的交付将取消该时间点之后的任何后续发送。

1. 选择要取消的电子邮件程序，然后单击 **中止投放** 在“控制面板”的“批准”拼贴下。

   ![](assets/ptz-abortdelivery.png)

1. 单击 **中止**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. 取消后， **结果** 您电子邮件程序的网格将类似于下面的内容。 任何后续发送都将被取消，并且会在 **活动类型** 列。

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >取消的电子邮件将 **not** 显示为软退回 *直到* 最初计划在各自时区内交付的时间。 在此之前，它们仍显示为“发送电子邮件”。

1. 在网格中，您可以单击任何电子邮件以查看活动详细信息。 对于已取消的发送，详细信息弹出窗口将如下所示：

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [了解收件人时区](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [使用收件人时区计划电子邮件程序](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)


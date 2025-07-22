---
unique-page-id: 13795727
description: 中止按收件人时区计划的电子邮件项目投放 — Marketo文档 — 产品文档
title: 中止按收件人时区计划的电子邮件项目投放
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# 中止按收件人时区计划的电子邮件项目投放 {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

在紧急情况下，您可以中止已在启用收件人时区的情况下开始运行的电子邮件程序的投放。

由于使用收件人时区计划的电子邮件程序最多可以运行24小时，因此中止程序的交付将取消在该时间点之后发送的任何后续发送。

1. 选择要取消的电子邮件程序，然后单击控制面板中&#x200B;**[!UICONTROL Abort Delivery]**&#x200B;拼贴下的[!UICONTROL Approval]。

   ![](assets/ptz-abortdelivery.png)

1. 单击&#x200B;**[!UICONTROL Abort]**&#x200B;确认您要取消投放。

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. 取消后，您的电子邮件程序的&#x200B;**[!UICONTROL Results]**&#x200B;网格将类似于下面的网格。 任何后续发送均被取消，并将在&#x200B;**[!UICONTROL Activity Type]**&#x200B;列中显示为“电子邮件软退回”。

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >取消的电子邮件&#x200B;**在**&#x200B;到&#x200B;*之前不会显示为软退回*，而原计划电子邮件将在各自的时区中发送。 在此之前，它们仍将显示为“发送电子邮件”。

1. 在网格中，您可以单击任意电子邮件以查看活动详细信息。 对于已取消的发送，详细信息弹出窗口将如下所示：

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [了解收件人时区](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [计划具有收件人时区的电子邮件程序](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)

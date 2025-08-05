---
unique-page-id: 12982903
description: 按收件人时区计划电子邮件程序 — Marketo文档 — 产品文档
title: 按收件人时区计划电子邮件程序
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
feature: Email Programs
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# 按收件人时区计划电子邮件程序 {#schedule-email-programs-with-recipient-time-zone}

在启用“收件人时区”的情况下计划电子邮件程序时，可能会出现以下两种情况：

1. 正在安排程序在接下来的25小时内运行&#x200B;****
1. 计划程序在未来25小时（即下周）内运行&#x200B;**个以上**

## 场景1:25小时内 {#scenario-within-hours}

假设您批准启用了收件人时区的电子邮件计划，并计划在未来25小时内完成投放。 您的智能列表中可能包含居住在已过计划时间的时区的人员。

在此场景中，我们允许您决定如何处理此合格人员的子集。 单击电子邮件程序&#x200B;**[!UICONTROL Recipient Time Zone]**&#x200B;拼贴中&#x200B;**[!UICONTROL Schedule]**&#x200B;旁边的齿轮图标。

![](assets/image2017-12-5-10-3a46-3a42.png)

这为您提供了两个选项：

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**定义**
>
>* **[!UICONTROL Deliver the following day in recipient’s time zone]**：如果电子邮件计划在星期二9:00am发出，则居住在已超过计划时间的时区的合格人员将在&#x200B;*星期三*&#x200B;的9:00am收到电子邮件。
>
>* **[!UICONTROL Deliver using the program's default set time]**：如果电子邮件计划在星期二9:00am发出，则居住在已过计划时间的时区的合格人员将根据您的订阅时区设置&#x200B;*收到电子邮件*。 因此，如果您的[订阅时区设置](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md)设置为PDT America/Los Angeles，这些收件人仍将在星期二的9:00am PDT（无论时间位于他们自己的时区）收到电子邮件。

>[!NOTE]
>
>[了解有关Marketo如何计算收件人时区的更多信息](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone)。

让我们更详细地考虑此方案。 假设您位于San Francisco，计划发送一封电子邮件（地址为7:00am）**9:00am**。 您的智能列表中包含来自以下区域的人员：

* 旧金山
* 得克萨斯州
* 纽约
* 意大利

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00am已在纽约和意大利通过，因此这两个时区的合格人员将根据&#x200B;**时区设置**&#x200B;接收电子邮件：

* **[!UICONTROL Deliver the following day in recipient’s time zone]：**&#x200B;星期三9:00am，在各自的时区，**或**

* **[!UICONTROL Deliver using the program's default set time]**：星期二的9:00am PDT（纽约 — 12:00pm EDT和意大利 — 6:00pm CET）。

批准程序后，它将在15分钟内开始运行。

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>尽管程序将在15分钟内启动发送电子邮件的&#x200B;*进程*，但此时电子邮件将不是&#x200B;*已投放*。 收件人仍将收到基于您选择的&#x200B;**[!UICONTROL Time Zone Settings]**&#x200B;的电子邮件。

## 场景2：超过25小时 {#scenario-more-than-hours}

在第二种方案中，您批准启用了&#x200B;**[!UICONTROL Recipient Time Zone]**&#x200B;且计划投放时间在未来超过25小时的电子邮件计划。 在这种情况下，程序将在世界上&#x200B;**最早**&#x200B;时区的计划时间开始运行(UTC + 14:00)。 全球每个时区都可能有符合您的智能列表资格的人员，因此从最早的时区开始，我们便可以在计划日期/时间将电子邮件投放给各自时区中的所有收件人。

**头开始**

现在，让我们讨论[[!UICONTROL Head Start]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)如何与&#x200B;**[!UICONTROL Recipient Time Zone]**&#x200B;一起使用。 我们现有的先发制人功能要求项目至少提前12小时计划。 那么这对收件人时区意味着什么？ 请记住，启用收件人时区后，我们将在最早时区(UTC +14:00)的计划时间开始运行电子邮件程序。 因此，要同时启用&#x200B;****&#x200B;开头和收件人时区，电子邮件程序需要在UTC +14 **的预定时间之前:00至少提前12小时计划。**

这意味着如果您在美国/洛杉矶并且想要同时启用开头和收件人时区，则需要提前&#x200B;**34小时**&#x200B;计划该计划。 我们怎么找到这个号码的？

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

简而言之，使用收件人时区计划的电子邮件程序需要在最早时区的计划时间开始运行（即首先到达午夜），以适应每个时区。 因此，如果您计划电子邮件程序……

* **交付时间为&#x200B;*在* 25小时内**，程序将在15分钟内开始运行。 已超过计划时间的收件人将根据您选择的时区设置接收电子邮件。
* **在未来&#x200B;*超过* 25小时之后**，程序将在最早时区(UTC +14:00)的计划时间开始运行。
* **如果开始时间为**，则程序将在最早时区(UTC +14:00)中比计划时间早12小时开始处理。

>[!CAUTION]
>
>在您开始发送电子邮件与实际发送电子邮件之间取消订阅的任何人，仍将收到该电子邮件。 我们建议调整您的取消订阅通知，以反映取消订阅可能需要1 - 2个工作日才能处理。

>[!MORELIKETHIS]
>
>* [了解收件人时区](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* 电子邮件程序的[开端](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [中止按收件人时区计划的电子邮件项目投放](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

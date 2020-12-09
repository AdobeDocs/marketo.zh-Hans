---
unique-page-id: 12982903
description: 计划电子邮件项目,收件人时区——营销文档——产品文档
title: 计划电子邮件项目(带收件人时区)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---


# 计划电子邮件项目(带收件人时区) {#schedule-email-programs-with-recipient-time-zone}

启用收件人时区时，计划电子邮件项目时，可能会出现两种情况：

1. 计划项目在 **后** 25小时内运行
1. 将项目安 **排** 在将来运行25小时以上（即，下周）

## 方案1:25小时内 {#scenario-within-hours}

假设您批准启用了收件人时区并计划在25小时内投递时间的电子邮件项目。 您的智能列表中可能有人居住在计划时间已过去的时区。

在此情况下，我们允许您决定如何处理这一部分合格人员。 在电子邮件收件人的 **计划拼贴中** ，单 **击“项目时** 区”旁边的齿轮图标。

![](assets/image2017-12-5-10-3a46-3a42.png)

这为您提供两个选项：

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**定义**
>
>* **在收件人的时区提供第二天**:如果电子邮件计划在周二上午9点发出，那么居住在预定时间已经过的时区的合格用户将在周三上午9 *点* 收到该电子邮件。
   >
   >
* **使用项目的默认设置时间交付**:如果电子邮件计划在星期二上午9:00发出，则符合条件的居住在时间已经过预定时间的时区的人员将根据您的订阅时 *区设置收到该电子邮件*。 因此，如果您 [的订](../../../../../product-docs/administration/settings/select-your-language-locale-and-time-zone.md) 阅时区设置 [设为PDT America/Los Angeles](../../../../../product-docs/administration/settings/set-default-location-settings-for-a-subscription.md) ，这些收件人仍将在星期二上午9点（无论他们所在时区的时间如何）收到电子邮件。

>



>[!NOTE]
>
>[进一步了解](https://docs.marketo.com/display/DOCS/Understanding+Recipient+Time+Zone#UnderstandingRecipientTimeZone-CalculatingTimeZone) Marketo如何为收件人计算时区。

让我们更详细地考虑这一情况。 假设您在旧金山，安排早上7点发送电子邮件， **发送时间为** 9点。 在您的智能列表中，有来自以下地区的人员：

* 旧金山
* 德克萨斯州
* 纽约
* 意大利

![](assets/image2017-12-6-10-3a52-3a41.png)

纽约和意大利早上9:00已经过，因此这两个时区的合格用户将根据“时区设置”收 **到电子邮件**:

* **在收件人的时区提供第二天：** 周三上午9点，在各自的时区， **或**

* **使用项目的默认设置时间交付**:星期二上午9:00（美国东部夏令时间下午12:00和意大利东部时间下午6:00）。

批准项目后，将在15分钟内运行该开始。

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>尽管项目将在15分 *钟内* 开始发送电子邮件的过程，但当时不会 *发送电* 子邮件。 收件人仍会根据您选择的时 **区设置收** 到电子邮件。

## 方案2:超过25小时 {#scenario-more-than-hours}

在第二种情况下，您批准启用了 **收件人时区的** 电子邮件项目，并且预定的发送时间将超过25小时。 在这种情况下，项目将在世界上最早的时 **区** (UTC + 14:00)按预定时间开始运行。 在全球的每个时区，都可能有人有资格获得您的智能列表，因此，从最早的时区开始，我们可以在预定的日期／时间将电子邮件发送给其各自时区的所有收件人。

头开始

现在，我们来谈谈头开始 [如何与](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)**收件人时区协作**。 我们现有的头部开始功能要求项目至少提前12小时预定。 那对收件人时区意味着什么？ 请记住，启用收件人时区后，我们开始在最早时区(UTC +14:00)的预定时间运行电子邮件项目。 因此，要同时启 **用头开始** 和收件人时区 **，电子邮件项目需要提前至少12小时（以UTC +14:00表示）预定。**

这意味着，如果您在美国／洛杉矶，并且要同时启用“开始”和“收件人时区”，您需要提前34 **小时计划项目** 。 我们怎么得到这个号码的？

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

简而言之，与收件人时区一起计划的电子邮件项目需要在最早时区（即最早到达午夜的时区）的预定时间运行开始，以便适应每个时区。 所以，如果您计划电子邮件项目...

* **投放时间 *在* 25小时内**,项目开始在15分钟内运行。 已经过预定时间的收件人将根据您选择的时区设置收到电子邮件。
* **投放时 *间* 超过 *25* 小时后**,项目开始在最早时区(UTC +14:00)中的预定时间运行。
* **使用头开始**,项目开始在最早时区的预定时间前12小时处理(UTC +14:00)。

>[!CAUTION]
>
>在您开始电子邮件发送时间和实际发送时间之间取消订阅的任何人仍会收到该电子邮件。 我们建议调整您的取消订阅通知，以反映可能需要1-2个工作日才能处理取消订阅。

>[!MORELIKETHIS]
>
>* [了解收件人时区](understanding-recipient-time-zone.md)
>* [电子邮件开始主管](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [中止投放使用收件人时区计划的电子邮件项目](abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

>




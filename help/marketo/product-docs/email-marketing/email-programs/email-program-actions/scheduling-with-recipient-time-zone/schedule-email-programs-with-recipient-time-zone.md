---
unique-page-id: 12982903
description: 使用收件人时区计划电子邮件计划 — Marketo文档 — 产品文档
title: 使用收件人时区计划电子邮件程序
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# 使用收件人时区计划电子邮件程序 {#schedule-email-programs-with-recipient-time-zone}

在启用“收件人时区”的情况下计划电子邮件程序时，可能会出现两种情况：

1. 计划程序运行 **within** 接下来的25小时
1. 计划程序运行 **更多** 超过25小时（即下周）

## 场景1:25小时内 {#scenario-within-hours}

假设您批准启用了收件人时区的电子邮件计划，并计划在未来25小时内发送该计划。 您的智能列表中可能有人居住在计划时间已经过的时区。

在此情景中，我们允许您决定如何处理此合格人员子集。 单击旁边的齿轮图标 **收件人时区** 在 **计划** 电子邮件程序的拼贴。

![](assets/image2017-12-5-10-3a46-3a42.png)

这为您提供了两个选项：

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**条件**
>
>* **以收件人的时区为后一天提供内容**:如果电子邮件计划在星期二上午9:00发出，则居住在计划时间已经过的时区的合格用户将收到电子邮件 *星期三* 早上9点。
>
>* **使用程序的默认设置时间交付**:如果电子邮件计划在星期二上午9:00发出，则居住在计划时间已经过的时区的合格用户将收到电子邮件 _根据您的订阅时区设置_. 如果你 [订阅时区设置](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) 设置为“太平洋夏季时间”(PDT America/Los Angeles)时，这些收件人仍将在太平洋夏季时间周二上午9点（无论其所在时区的时间如何）收到电子邮件。


>[!NOTE]
>
>[了解更多](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) 关于Marketo如何计算收件人的时区。

让我们更详细地考虑此方案。 假设您在旧金山，早上7:00发电子邮件 **上午9:00** 发送。 在您的智能列表中，有来自以下地区的人员：

* 旧金山
* 德克萨斯
* 纽约
* 意大利

![](assets/image2017-12-6-10-3a52-3a41.png)

早上9:00已经在纽约和意大利传递，因此这两个时区的合格用户将根据 **时区设置**:

* **以收件人的时区为后一天提供信息：** 周三早上9点，在各自的时区， **或**

* **使用程序的默认设置时间交付**:星期二，太平洋夏季时间上午9:00（美国东部时间中午12:00，意大利东部时间下午6:00）。

批准程序后，该程序将在15分钟内开始运行。

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>尽管该程序将启动 _过程_ 在15分钟内发送电子邮件时，电子邮件将不会 _交付_ 那时。 收件人仍将根据 **时区设置** 你选。

## 场景2:超过25小时 {#scenario-more-than-hours}

在第二种情况中，您批准使用 **收件人时区** 启用，并且计划的提交时间会在将来超过25小时。 在这种情况下，该程序将在 **最早** 世界时区(UTC + 14:00)。 全球各地的每个时区都可能有符合您智能列表资格的人员，因此从最早时区开始，我们可以在计划的日期/时间向各自时区的所有收件人发送电子邮件。

**开始前**

现在，我们谈谈 [开始前](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) 与 **收件人时区**. 我们现有的“开始前”功能要求该计划至少提前12小时进行计划。 那么，这对收件人时区意味着什么？ 请记住，启用“收件人时区”后，我们会在最早时区(UTC +14:00)的计划时间开始运行电子邮件程序。 因此，要启用 **both** 开始前和收件人时区，需要计划电子邮件程序 **世界协调时(UTC)+14:00，比预定时间至少提前12小时。**

这意味着如果您在美国/洛杉矶，并且要同时启用“开始时间”和“收件人时区”，则需要计划计划 **34小时** 提前。 我们怎么得到这个号码的？

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

简言之，与收件人时区一起计划的电子邮件程序需要在最早时区（即，到达午夜之前）的计划时间开始运行，以便适应每个时区。 所以，如果你计划一个电子邮件程序……

* **投放时间 _within_ 25小时**，则程序将在15分钟内开始运行。 已超过计划时间的收件人将根据您选择的时区设置收到电子邮件。
* **投放时间 _大于_ 未来25小时**，该程序将在最早时区的计划时间开始运行(UTC +14:00)。
* **开头**，该程序会在最早时区的计划时间之前12小时开始处理(UTC +14:00)。

>[!CAUTION]
>
>在您开始发送电子邮件到实际发送电子邮件之间取消订阅的任何人仍将收到该电子邮件。 我们建议调整您的取消订阅通知，以反映取消订阅可能需要1-2个工作日才能处理。

>[!MORELIKETHIS]
>
>* [了解收件人时区](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [电子邮件程序开始使用](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [中止使用收件人时区计划的电子邮件程序的发送](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)


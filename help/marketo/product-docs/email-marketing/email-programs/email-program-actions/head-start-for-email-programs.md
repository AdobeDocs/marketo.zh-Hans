---
unique-page-id: 10097202
description: 电子邮件计划入门 — Marketo文档 — 产品文档
title: 电子邮件程序开始使用
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# 电子邮件程序开始使用 {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[创建电子邮件程序](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

当您为电子邮件程序选择日期/时间时，它会确定程序何时开始处理。 如果您希望在选定时间启动电子邮件，则“开始前”会通过提前处理程序为您提供该选项。

## 标准开头 {#standard-head-start}

1. 单击 **营销活动**.

   ![](assets/one-1.png)

1. 查找并选择您的电子邮件程序。

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Head Start不能用于A/B测试。

1. 在“计划”拼贴中，计划电子邮件，然后选择 **开始前** 框中。

   ![](assets/three-1.png)

   选择“开始前”后，该程序将在计划时间前大约12小时开始处理。 处理开始后，程序将被锁定。

   >[!CAUTION]
   >
   >在项目锁定后取消订阅的受众中的任何人仍将收到电子邮件。 我们建议调整您的取消订阅通知，以反映取消订阅可能需要1-2个工作日才能处理。

1. 单击 **批准项目**.

   ![](assets/four-1.png)

   项目批准后，您可能会在“批准”拼贴中看到四种不同的状态。

   * **正在等待运行：** 在程序获得批准后。
   * **处理已启动，正在等待运行：** 正在处理。
   * **处理已完成，正在等待运行：** 处理完成，电子邮件现在正在等待计划的启动时间。
   * **已完成：** 程序已完成。

   >[!TIP]
   >
   >在程序锁定后但在电子邮件发送前想要取消？ 没问题！ 只需单击 **中止程序** 位于“批准”拼贴的右下方。

   >[!NOTE]
   >
   >如果您在电子邮件程序计划运行时间之前不到12小时取消批准，但是您改变了主意，则需要选择一个新的日期/时间，该日期/时间至少比您批准该日期/时间提前12小时。

## 以收件人时区开头 {#head-start-with-recipient-time-zone}

我们现有的“开始前”功能要求该计划至少提前12小时进行计划。 这对收件人时区意味着什么？ 请记住，当“收件人时区”处于活动状态时，我们将在最早时区的午夜(UTC +14:00)开始运行电子邮件程序。 因此，要启用 **both** 开始前和收件人时区，需要计划项目 **比最早时区提前至少12小时（世界协调时+14:00）**.)

这意味着如果您在美国/洛杉矶，并且要同时启用“开始时间”和“收件人时区”，则需要计划计划 **34小时** 提前。 我们怎么得到这个号码的？

![](assets/image2017-12-5-13-3a11-3a46.png)

[了解更多](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) 了解如何使用收件人时区计划电子邮件程序。

>[!MORELIKETHIS]
>
>* [计划电子邮件程序](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [使用收件人时区计划电子邮件程序](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [了解收件人时区](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)


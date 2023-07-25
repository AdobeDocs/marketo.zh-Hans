---
unique-page-id: 10097202
description: 电子邮件程序快速入门 — Marketo文档 — 产品文档
title: 电子邮件程序快速入门
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# 电子邮件程序快速入门 {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[创建电子邮件程序](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

当您为电子邮件程序选择日期/时间时，它会确定程序何时开始处理。 如果您希望电子邮件在选定的时间启动，则提前开始可为您提供该选项，即提前处理该程序。

## 标准头开始 {#standard-head-start}

1. 单击 **营销活动**.

   ![](assets/one-1.png)

1. 查找并选择您的电子邮件计划。

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Head Start不能用于A/B测试。

1. 在“计划”拼贴中，计划您的电子邮件，然后选择 **头开始** 盒子。

   ![](assets/three-1.png)

   选择“Head Start”（开始播放）后，程序将在计划时间之前约12小时开始处理。 一旦处理开始，程序将被锁定。

   >[!CAUTION]
   >
   >受众中在项目锁定后取消订阅的任何人仍会收到电子邮件。 我们建议调整您的取消订阅通知，以反映取消订阅可能需要1-2个工作日才能处理。

1. 单击 **批准项目**.

   ![](assets/four-1.png)

   项目批准后，您可以在“批准”图块中看到四个不同的状态。

   * **正在等待运行：** 项目获得批准后。
   * **处理已开始，正在等待运行：** 正在处理。
   * **处理完成，等待运行：** 处理完成，电子邮件现在等待计划时间启动。
   * **已完成：** 程序已完成。

   >[!TIP]
   >
   >是否要在程序锁定后但在电子邮件发送前取消？ 没问题！ 只需单击 **中止程序** 位于批准图块的右下方。

   >[!NOTE]
   >
   >如果您在计划运行时间之前不到12小时就取消批准电子邮件程序，但随后改变了主意，您将需要选择一个至少比批准时提前12小时的新日期/时间。

## 以收件人时区开头的行程 {#head-start-with-recipient-time-zone}

我们现有的先发制人功能要求项目至少提前12小时计划。 这对收件人时区意味着什么？ 请记住，当收件人时区处于活动状态时，我们会在最早时区的午夜开始运行电子邮件程序(UTC +14:00)。 因此，要启用 **两者** 开头和收件人时区，需要计划程序 **至少比最早时区提前12小时(UTC +14:00**.)

这意味着如果您在美国/洛杉矶并且希望同时启用开始时间和收件人时区，则需要安排该计划 **34小时** 事前准备。 我们怎么找到这个号码的？

![](assets/image2017-12-5-13-3a11-3a46.png)

[了解详情](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) 有关如何使用收件人时区安排电子邮件程序的信息。

>[!MORELIKETHIS]
>
>* [计划您的电子邮件计划](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [按收件人时区计划电子邮件程序](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [了解收件人时区](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

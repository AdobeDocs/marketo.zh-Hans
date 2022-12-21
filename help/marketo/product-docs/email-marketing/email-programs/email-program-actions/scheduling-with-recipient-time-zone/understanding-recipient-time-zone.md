---
unique-page-id: 12983291
description: 了解收件人时区 — Marketo文档 — 产品文档
title: 了解收件人时区
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# 了解收件人时区 {#understanding-recipient-time-zone}

可以将电子邮件和参与计划配置为根据收件人的时区发送，从而无需创建多个计划 — 发送一次，Marketo会自动保存电子邮件直到到正确的当地时间。

>[!NOTE]
>
>收件人时区当前有效 **仅** 与电子邮件内容。 它不适用于默认的参与计划。

## 电子邮件程序 {#email-programs}

在以下两种情况下 [计划电子邮件程序](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. 计划在接下来的25小时内运行程序。
1. 计划该程序在将来运行25小时以上（即下周）。

为了适应每个时区，与收件人时区一起计划的电子邮件程序会在 **first/eariest** 世界时区（世界协调时+14:00）。

## 参与计划 {#engagement-programs}

当您 [计划参与项目流](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) 并且收件人时区处于活动状态，节目群组将在UTC +14:00的午夜开始运行。 我们要求您安排在未来至少25小时内进行第一次投影（24小时+开始营销活动的一段时间），因为人们可能有资格在全球每个时区进行投影。 此时开始处理(UTC +14:00)，确保我们在计划的日期和时间向符合此角色的每个人发送电子邮件。

## 计算时区 {#calculating-time-zone}

Marketo会根据人员的“城市”、“州”、“国家/地区”或“邮政编码”计算时区。 如果我们无法根据这些值计算某人的时区，我们会还原到“推断出的城市”、“推断出的州”、“推断出的国家/地区”和“推断出的邮政编码”字段。

如果我们 **仅** 国家或地区或 **仅** 可用状态：

* 对于时区少于三个的国家，我们选择中时区。
* 对于具有两个时区的州，我们选择两个时区中较早的时区。

如果我们仍无法通过这些字段的任意组合来确定某人的时区，我们将 **not** 分配时区，并根据您的Marketo订阅时区发送电子邮件。 因此，如果您的程序计划在太平洋夏季时间上午9:00，则没有分配时区的人员将在太平洋夏季时间上午9:00收到电子邮件。

>[!NOTE]
>
>当上述任何输入字段发生更改时，Marketo会自动重新计算人员的时区。

>[!MORELIKETHIS]
>
>* [使用收件人时区计划电子邮件程序](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [电子邮件程序开始使用](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [按收件人时区计划参与计划](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)


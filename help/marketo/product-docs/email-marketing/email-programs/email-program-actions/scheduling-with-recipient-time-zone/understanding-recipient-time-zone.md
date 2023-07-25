---
unique-page-id: 12983291
description: 了解收件人时区 — Marketo文档 — 产品文档
title: 了解收件人时区
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# 了解收件人时区 {#understanding-recipient-time-zone}

可以将电子邮件和参与计划配置为根据收件人的时区交付，而无需创建多个计划 — 只发送一次，Marketo会自动保留电子邮件，直到本地时间正确。

>[!NOTE]
>
>收件人时区当前有效 **仅限** 包含电子邮件内容。 它不适用于默认参与计划。

## 电子邮件程序 {#email-programs}

在以下情况下，有两种主要方案 [计划电子邮件程序](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)：

1. 计划程序在未来25小时内运行。
1. 计划程序在未来（即下周）运行超过25小时。

为了适应每个时区，使用收件人时区计划的电子邮件程序在中的午夜开始运行 **第一个/最早的** 世界时区(UTC +14:00)。

## 参与计划 {#engagement-programs}

当您 [安排参与计划流](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) 收件人时区处于活动状态时，程序演绎版将在UTC午夜+14:00开始运行。 我们要求您安排在未来至少25小时（24小时+开始营销活动的时间）进行第一次点播，因为人们可能在全球每个时区都有资格参加点播。 此时按UTC +14:00开始处理，这可保证我们将在计划的日期和时间向符合此演绎版条件的每个人发送电子邮件。

## 计算时区 {#calculating-time-zone}

Marketo根据人员的城市、省/自治区、国家/地区或邮政编码计算时区。 如果我们无法从这些值计算某个人的时区，则我们会返回到“推断的城市”、“推断的州/省”、“推断的国家/地区”和“推断的邮政编码”字段。

如果我们 **仅限** 国家或地区 **仅限** 可用状态：

* 对于时区不超过3个的国家/地区，我们选择中间时区。
* 对于具有两个时区的状态，我们选择两个时区中较早的一个。

如果我们仍然无法从这些字段的任何组合确定某人的时区，我们将 **非** 分配时区，将根据您的Marketo订阅时区发送电子邮件。 因此，如果您的项目安排在太平洋夏季时间上午9:00，则未分配时区的用户将在太平洋夏季时间上午9:00收到电子邮件。

>[!NOTE]
>
>当以上任何输入字段更改时，Marketo会自动重新计算人员的时区。

>[!MORELIKETHIS]
>
>* [按收件人时区计划电子邮件程序](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [电子邮件程序快速入门](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [按照收件人时区安排参与计划](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

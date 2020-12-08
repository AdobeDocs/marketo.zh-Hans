---
unique-page-id: 12983291
description: 了解收件人时区- Marketo Docs —— 产品文档
title: 了解收件人时区
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---


# 了解收件人时区 {#understanding-recipient-time-zone}

可以将电子邮件和参与项目配置为根据收件人的时区发送，从而无需创建多个项目-发送一次，营销人员自动保存电子邮件，直到正确的本地时间。

>[!NOTE]
>
>收件人时区当前仅 **用于** 电子邮件内容。 对于默认的参与项目，它不起作用。

## 电子邮件项目 {#email-programs}

计划电子邮件项目时 [有两种主要情况](schedule-email-programs-with-recipient-time-zone.md):

1. 安排项目在25小时内运行。
1. 安排项目在将来运行25小时以上（即，下周）。

为了适应每个时区，在世界上第一个／最早的时区(UTC +14:00)午 **夜运行收件人时区项目** ，为电子邮件开始安排电子邮件。

## 参与项目 {#engagement-programs}

当您 [计划参与项目流](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) ，并且收件人时区处于活动状态时，项目播放将在UTC +14:00的午夜运行。 我们要求您在将来至少计划25小时(24小时+开始活动的时间)的首次演出，因为在全球的每个时区，人们都有资格参加。 此时以UTC +14:00开始处理，保证我们在预定日期和时间为有资格参加此演播的每个人发送电子邮件。

## 计算时区 {#calculating-time-zone}

Marketo根据个人的城市、州、国家或邮政编码计算时区。 如果我们无法根据这些值计算某人的时区，我们会还原到“推断城市”、“推断州”、“推断国家”和“推断邮政编码”字段。

如果我们拥有**仅**国家／地区或仅 **提供** 州／地区：

* 对于三个或更少时区的国家，我们选择中间时区。
* 对于具有两个时区的州，我们选择两个时区中较早的一个。

如果我们仍无法从这些字段的任意组合中确定某人的时区，则我们将不 **分配** 某个时区，并会根据您的市场订阅时区发送电子邮件。 因此，如果您的项目预定在太平洋夏令时上午9:00，则没有分配时区的人员将在太平洋夏令时上午9:00收到电子邮件。

>[!NOTE]
>
>Marketo在以上任何输入字段发生变化时自动重新计算人员的时区。

>[!NOTE]
>
>**相关文章**
>
>* [计划电子邮件项目(带收件人时区)](schedule-email-programs-with-recipient-time-zone.md)
>* [电子邮件开始主管](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)

   >
   >
* [计划项目与收件人时区](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

>




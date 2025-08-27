---
unique-page-id: 12983291
description: 了解收件人时区 — Marketo文档 — 产品文档
title: 了解收件人时区
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 3%

---

# 了解收件人时区 {#understanding-recipient-time-zone}

可以将电子邮件和参与程序配置为根据收件人的时区发送，从而无需创建多个程序 — 只发送一次，Marketo会自动保留电子邮件，直到到达正确的本地时间。

>[!NOTE]
>
>[!UICONTROL Recipient Time Zone]当前仅对电子邮件内容使用&#x200B;**2}。**&#x200B;它不适用于默认参与计划。

## 电子邮件项目 {#email-programs}

在[计划电子邮件程序](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)时，有两种主要情况：

1. 计划程序在未来25小时内运行。
1. 计划程序在未来（即下周）运行超过25小时。

为了适应每个时区，使用[!UICONTROL Recipient Time Zone]计划的电子邮件程序在世界上&#x200B;**第一个/最早的**&#x200B;时区的午夜开始运行(UTC +14:00)。

## 互动项目 {#engagement-programs}

当您[计划一个参与项目程序流](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)并且[!UICONTROL Recipient Time Zone]处于活动状态时，程序转换将在UTC时间+14:00的午夜开始运行。 我们要求您安排未来至少25小时（24小时+开始营销活动的时间）的首次点播，因为全球各地每个时区都有资格参加点播。 此时以UTC +14:00开始处理，这可保证在计划的日期和时间，为每个符合此转换条件的人发送电子邮件。

## 计算时区 {#calculating-time-zone}

Marketo根据人员的城市、州/省、国家/地区或邮政编码计算时区。 如果我们无法从这些值计算某个人的时区，则我们会返回到“推断的城市”、“推断的州/省”、“推断的国家/地区”和“推断的邮政编码”字段。

在我们只有&#x200B;**个**&#x200B;国家/地区或只有&#x200B;**个**&#x200B;状态可用的情况下：

* 对于时区数等于或少于三个时区的国家/地区，我们选择中间时区。
* 对于具有两个时区的状态，我们选择两个时区中较早的一个。

如果我们仍然无法从这些字段的任意组合确定某人的时区，我们&#x200B;**不会**&#x200B;分配时区，系统将根据您的Marketo订阅时区发送电子邮件。 因此，如果您的项目安排在9:00am PDT，则未分配时区的人员将收到一封电子邮件，地址为9:00am PDT。

>[!NOTE]
>
>当以上任何输入字段发生更改时，Marketo会自动重新计算人员的时区。

>[!MORELIKETHIS]
>
>* [使用[!UICONTROL Recipient Time Zone]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)计划电子邮件程序
>* 电子邮件程序的[开端](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [计划与[!UICONTROL Recipient Time Zone]](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)的参与计划

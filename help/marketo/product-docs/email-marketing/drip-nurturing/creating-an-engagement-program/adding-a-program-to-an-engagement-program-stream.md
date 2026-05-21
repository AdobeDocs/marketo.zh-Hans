---
unique-page-id: 10098134
description: 了解参与流中的嵌套程序以及何时使用它们。 为子组、多点触控和额外流量步骤添加程序。
title: 将计划添加到参与计划流中
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
feature: Engagement Programs
TQID: https://experienceleague.adobe.com/kI2v6drF78DnJhhEbgeVSi4TYbF5rExY2wgR0aAK-bI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: b0bb9048-d951-48d8-8232-45cf248a7e27id: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 471
ht-degree: 4%

---

# 将计划添加到参与计划流中 {#adding-a-program-to-an-engagement-program-stream}

## 为什么在参与计划流中使用嵌套计划？ {#why-use-a-nested-program-in-an-engagement-program-stream}

在参与计划中，将电子邮件添加到流很容易，并且可以正常运行。 但是，如果您的业务需求更复杂，则可能适合将电子邮件置于项目中。 例如，您可能希望：

* 向流中的子组人员发送电子邮件
* 向流中的子组发送&#x200B;*个不同的*&#x200B;电子邮件
* 将登陆页面、表单或其他资产包含在培养中
* 启用多点触控归因
* 添加额外的流量步骤，如提醒电子邮件

## 当您在流中使用程序时，会出现什么情况？ {#what-happens-when-you-use-a-program-in-a-stream}

使用嵌套程序时，向人员发送电子邮件的决定取决于程序成员资格和程序ID。

* 如果您不是项目群成员，您将会收到属于项目群的任何电子邮件一次
* 如果您是项目群的成员，将不会收到电子邮件
* 如果您不再是会员，但之前已通过该计划收到电子邮件，则您将不会收到电子邮件

当您在流中使用程序时，您以前是否收到过该特定电子邮件并不重要。 只要该特定程序&#x200B;*中的电子邮件未在*&#x200B;之前发出，您就可以再次收到该电子邮件。

在参与计划中，它可能会把电子邮件和程序巧妙地混合在一起。 您可能要使用其中一个。

>[!TIP]
>
>在智能列表中使用&#x200B;**[!UICONTROL Member of Engagement Program]**&#x200B;筛选器。

## 不符合智能列表条件的用户会出现什么情况？ {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

如果从嵌套项目智能营销策划的智能列表中过滤出了某人，则其在当前播放过程中不会转到下一段内容。 他们将继续观看流中&#x200B;*following*&#x200B;演绎版的下一段内容。

## 嵌套程序包含什么？ {#what-does-a-nested-program-contain}

设计良好的嵌套项目包含电子邮件、报表和智能营销策划。 把这些放在一起是合情合理的。

您使用的电子邮件可以存在于程序中、其他程序中，甚至在[!UICONTROL Design Studio]中。 它的存在位置将取决于您要如何使用它。

报告电子邮件位置发生更改。 因此，例如，如果电子邮件位于[!UICONTROL Design Studio]中，则在电子邮件性能报表中，所有量度都显示在一行中 — 不同的流型会合并。 但是，在参与流性能报表中，将单独显示不同的发送。

>[!CAUTION]
>
>如果要重新发送某些内容，则创建新项目和智能营销活动是最安全的。

>[!MORELIKETHIS]
>
>* [向流中添加内容](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [了解程序](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)

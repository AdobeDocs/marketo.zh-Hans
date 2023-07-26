---
unique-page-id: 10098134
description: 将项目添加到参与项目项目流 — Marketo文档 — 产品文档
title: 将计划添加到参与计划流
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# 将计划添加到参与计划流 {#adding-a-program-to-an-engagement-program-stream}

## 为什么在参与计划流中使用嵌套计划？ {#why-use-a-nested-program-in-an-engagement-program-stream}

在参与计划中，可以轻松地将电子邮件添加到流中，并且效果不错。 但是，如果您的业务需求更复杂，则可能适合将电子邮件置于项目中。 例如，您可能希望：

* 向流中的子组人员发送电子邮件
* 发送 *不同* 发送给流中子组的电子邮件
* 将登陆页面、表单或其他资产包含在培养中
* 启用多点触控归因
* 添加额外的流量步骤，如提醒电子邮件

## 当您在流中使用程序时，会出现什么情况？ {#what-happens-when-you-use-a-program-in-a-stream}

使用嵌套程序时，向人员发送电子邮件的决定取决于程序成员资格和程序ID。

* 如果您不是项目群成员，您将会收到属于项目群的任何电子邮件一次
* 如果您是计划的成员，将不会收到电子邮件
* 如果您不再是会员，但之前已通过该计划收到电子邮件，则您将不会收到电子邮件

当您在流中使用程序时，您以前是否收到过该特定电子邮件并不重要。 只要电子邮件以前没有发出 *在特定程序中*，您可以再次收到该邮件。

在参与计划中，它可能会把电子邮件和程序巧妙地混合在一起。 您可能要使用其中一个。

>[!TIP]
>
>确保使用 **参与计划成员** 在智能列表中进行筛选。

## 不符合智能列表条件的用户会出现什么情况？ {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

如果从嵌套项目智能营销策划的智能列表中过滤出了某人，则其在当前播放过程中不会转到下一段内容。 他们将继续观看流中的下一段内容 *关注* 演员阵容。

## 嵌套程序包含什么？ {#what-does-a-nested-program-contain}

设计良好的嵌套项目包含电子邮件、报表和智能营销策划。 把这些放在一起是合情合理的。

您使用的电子邮件可以在程序、其他程序甚至设计工作室中存取。 它的存在位置将取决于您要如何使用它。

报告电子邮件位置发生更改。 因此，例如，如果电子邮件在Design Studio中，则在电子邮件性能报表中，所有量度都显示在一行中 — 不同的投放会组合在一起。 但是，在参与流性能报表中，将单独显示不同的发送。

>[!CAUTION]
>
>如果要重新发送某些内容，则创建新项目和智能营销活动是最安全的。

>[!MORELIKETHIS]
>
>* [将内容添加到流](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [了解项目群](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)

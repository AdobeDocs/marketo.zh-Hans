---
unique-page-id: 10098134
description: 向参与项目流添加项目 — Marketo文档 — 产品文档
title: 向参与项目流添加项目
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# 向参与项目流添加项目 {#adding-a-program-to-an-engagement-program-stream}

## 为什么在参与项目流中使用嵌套程序？ {#why-use-a-nested-program-in-an-engagement-program-stream}

在参与项目的流中添加电子邮件很容易，而且可以正常使用。 但是，如果您的业务需求更复杂，则可能适合将电子邮件放入项目中。 例如，您可能希望：

* 向流中的子组人员发送电子邮件
* 发送 *不同* 电子邮件发送到流中的子组
* 在“培养”中包括登陆页面、表单或其他资产
* 启用多接触归因
* 添加额外的流量步骤，如警报电子邮件

## 在流中使用程序会发生什么情况？ {#what-happens-when-you-use-a-program-in-a-stream}

使用嵌套程序时，根据程序成员资格和程序ID决定向人员发送电子邮件。

* 如果您不是项目的成员，您将收到属于该项目的任何电子邮件
* 如果您是项目的成员，您将不会收到该电子邮件
* 如果您不再是会员，而是通过该程序提前收到了电子邮件，则您将不会收到该电子邮件

当您在流中使用程序时，您之前是否收到过该特定电子邮件并不重要。 只要以前未发出电子邮件 *在特定程序中*，则可以再次收到它。

在参与项目中混合使用电子邮件和程序可能会很棘手。 您可能希望使用其中一种或另一种。

>[!TIP]
>
>请务必使用 **参与计划成员** 过滤器。

## 不符合智能列表标准的用户会遇到什么情况？ {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

如果某人从嵌套项目智能营销活动的智能列表中过滤出来，则他们在当前投放期间不会继续访问下一段内容。 他们将转到流中的下一段内容，以便 *以下项* 铸。

## 嵌套程序包含什么？ {#what-does-a-nested-program-contain}

精心设计的嵌套项目包含电子邮件、报表和智能营销活动。 把这些放在一起是有道理的。

您使用的电子邮件可以存放在项目、其他项目中，甚至在Design Studio中。 它的存在取决于您希望如何使用它。

使用电子邮件位置报告更改。 例如，如果电子邮件位于Design Studio的电子邮件性能报表中，则所有量度都显示在一行中 — 不同的投放会被合并。 但是，在参与流绩效报表中，会单独显示不同的发送。

>[!CAUTION]
>
>如果您想重新发送一些内容，则最安全的做法是创建新项目和智能营销活动。

>[!MORELIKETHIS]
>
>* [向流添加内容](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [了解程序](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)


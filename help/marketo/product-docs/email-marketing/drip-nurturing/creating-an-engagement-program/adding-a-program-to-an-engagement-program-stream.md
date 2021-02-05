---
unique-page-id: 10098134
description: 将项目添加到参与项目流- Marketo Docs —— 产品文档
title: 将项目添加到参与项目流
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# 将项目添加到参与项目流{#adding-a-program-to-an-engagement-program-stream}

## 为何在参与项目流中使用嵌套项目?{#why-use-a-nested-program-in-an-engagement-program-stream}

在参与项目将电子邮件添加到流中很容易，并且它运行正常。 但是，如果您的业务需要更复杂，则将电子邮件放在项目中可能是合理的。 例如，您可能希望：

* 向流中的分组人员发送电子邮件
* 将&#x200B;*不同的*&#x200B;电子邮件发送到流中的子组
* 在培养中包括登陆页、表单或其他资产
* 启用多触归因
* 添加额外的流程步骤，如警报电子邮件

## 在流中使用项目时会发生什么情况？{#what-happens-when-you-use-a-program-in-a-stream}

使用嵌套项目时，根据项目会员资格和项目ID决定向人员发送电子邮件。

* 如果您不是项目的成员，您将收到属于项目的任何电子邮件
* 如果您是项目的成员，您不会收到
* 如果您不再是会员，但是之前通过该项目收到了电子邮件，则不会收到该电子邮件

在流中使用项目时，是否以前收到过该特定电子邮件并不重要。 只要该特定项目&#x200B;*中*&#x200B;之前未发出该电子邮件，您就可以再次收到它。

在互动项目中，您可能会遇到棘手的电子邮件和项目混合问题。 你可能想用一个或另一个。

>[!TIP]
>
>请务必在智能列表中使用&#x200B;**参与项目成员**&#x200B;过滤器。

## 对于不符合智能列表标准的人，会出现什么情况？{#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

在某人被从嵌套项目的智能活动的智能列表中筛选出的事件中，他们在当前播放期间不会继续移动到下一段内容。 在&#x200B;*转换后，它们将移至流中的下一段内容。*

## 嵌套项目包含什么？{#what-does-a-nested-program-contain}

设计良好的嵌套项目包含电子邮件、报表和智能活动。 把它们放在一起是合理的。

您使用的电子邮件可以存放在项目、不同项目，甚至Design Studio中。 它住在哪里取决于你想怎样使用它。

报告会随电子邮件位置而改变。 因此，例如，如果电子邮件位于Design Studio和电子邮件性能报告中，所有指标都会显示在一行中——不同的评测会被组合。 但是，在参与流绩效报告中，会单独显示不同的发送。

>[!CAUTION]
>
>如果要重新发送某些内容，最安全的方法是创建新项目和智能活动。

>[!MORELIKETHIS]
>
>* [向流中添加内容](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [了解项目](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)


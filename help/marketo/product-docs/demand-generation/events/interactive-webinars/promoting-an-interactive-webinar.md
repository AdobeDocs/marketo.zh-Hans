---
description: 推广交互式网络研讨会 — Marketo文档 — 产品文档
title: 推广交互式网络研讨会
feature: Interactive Webinars
exl-id: d26f91ce-3a95-4247-9a52-085260bb15e8
source-git-commit: e4a6123684162d9bbf2edddbd9aaf190030dc728
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# 推广交互式网络研讨会 {#promoting-an-interactive-webinar}

推广交互式网络研讨会与通过Launchpoint推广合作伙伴网络研讨会类似。 创建交互式网络研讨会事件程序时，可以通过运行活动或将成员导入程序来添加成员。 要检查已添加到交互式网络研讨会事件程序的成员，请单击&#x200B;**成员**&#x200B;选项卡。

![](assets/promoting-an-interactive-webinar-1.png)

添加或导入成员后，您可以在交互式网络研讨会活动项目群内创建一个电子邮件促销活动，向所有项目群成员发送邀请，并在发送电子邮件后将其状态更改为“已邀请”。

>[!NOTE]
>
>如果要将共同主持人或演示者作为受众成员添加到交互式网络研讨会事件计划，则必须为他们使用不同的电子邮件ID，否则他们将收到“此电子邮件已注册”错误。

电子邮件可以包含项目的特定详细信息，并包括登陆页面URL，该URL会将收件人重定向到可添加更多有关网络研讨会的信息（例如，内容、演示者信息等）的特定页面。 此登陆页面可在交互式网络研讨会事件程序中创建为本地资产。

您可以通过以下方式请求注册此网络研讨会：在登陆页面上启用表单，并将表单点击链接到交互式网络研讨会事件计划中启用的注册。 然后，可以创建活动，将表单提交用作触发器，并将项目状态从“已邀请”更改为“已注册”。

>[!NOTE]
>
>在交互式网络研讨会中，从“已邀请”到“已注册”的过渡不会是自动的，因为可能会有多个触发器创建该过渡。

一旦成员在交互式网络研讨会活动计划中处于“已注册”项目状态，系统就会自动向Adobe Connect中创建的网络研讨会进行注册。 随后，会将名字、姓氏和电子邮件ID等注册数据传输到Adobe Connect。 这意味着，一旦用户以参与者身份加入网络研讨会，演示者或主持人在网络研讨会期间便可以使用该信息。

在注册后的几分钟内，成员的网络研讨会URL将填充到成员选项卡中。 如果您无法找到网络研讨会URL的列，请确保该列已添加到您的视图中。 这是一个个性化的URL，每个注册成员都可以在计划的时间参加网络研讨会，而无需任何身份验证。 内部交换的令牌负责为成员提供身份验证。

您可以使用令牌在电子邮件促销活动中向个人成员包含网络研讨会URL，以告知他们已在事件中注册，并使用加入URL在计划时间进入网络研讨会。 日历令牌可用于同一电子邮件营销活动，以确保可以将网络研讨会计划添加到成员的日历中。

事件程序中“概述”选项卡右侧的可用链接，可用于创建登陆页面和电子邮件营销活动。 与活动相关的其余促销活动与使用Launchpoint集成的合作伙伴网络研讨会相同。

![](assets/promoting-an-interactive-webinar-2.png)

交互式网络研讨会允许您在网络研讨会之前、期间或之后请求注册。 在所有情况下，您只需要与潜在客户共享网络研讨会URL即可。 在网络研讨会开始前单击该链接，会将其发送到网络研讨会前的登陆页面。 在网络研讨会期间单击该链接会引导他们参加正在进行的网络研讨会。 网络研讨会后单击该按钮可将其转到网络研讨会的录像。

## 交互式网络研讨会令牌 {#interactive-webinars-tokens}

使用令牌在电子邮件和登陆页面中推广交互式网络研讨会，而无需手动添加网络研讨会详细信息。 这提高了整体效率，因为对网络研讨会元数据（如网络研讨会标题、开始日期等）所做的任何更改都将自动反映在您的资源中。

![](assets/promoting-an-interactive-webinar-3.png)

**令牌列表**

* program.webinarCapacity
* program.webinarDuration
* program.webinarEndDate
* program.webinarEndTime
* program.webinarGenericURL
* program.webinarLanguage
* program.webinarStartDate
* program.webinarStartTime
* program.webinarTimezone
* program.webinarTitle

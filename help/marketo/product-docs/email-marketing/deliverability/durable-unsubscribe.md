---
unique-page-id: 10094576
description: 持久取消订阅 — Marketo文档 — 产品文档
title: 持久取消订阅
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# 持久取消订阅 {#durable-unsubscribe}

Marketo改进了取消订阅功能的行为，使其具有“持久性”。 我们添加了一个主控的电子邮件状态，它与人员详细信息记录中显示的取消订阅标记不同。

如果unsubscribe标志从false设置为true，则会更新主控的电子邮件状态，并且更改会传播给具有相同电子邮件地址的其他人。 如果删除人员并重新创建人员，或者使用相同的电子邮件地址创建新记录，则取消订阅标记将 **非** 将被覆盖。

>[!NOTE]
>
>持久Unsubscribe可在整个Marketo数据库中的所有分区中使用。

## 将取消订阅标志从True更新为False（例如，重新订阅人员） {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

可通过多种方式重新订阅用户。

在Salesforce， **清除** 潜在客户/联系人记录中的Email Opt Out字段。 这将同步到Marketo。

![](assets/one.png)

在Marketo中， **清除** 人员记录的“信息”选项卡中的已取消订阅框。

![](assets/two.png)

运行 **更改数据值** 一个或多个用户的流量步骤，如下所示。

![](assets/three.png)

通过SOAP API更新现有人员。

## 创建新人员 {#creating-a-new-person}

创建新人员后，Marketo会根据主控电子邮件状态表检查该人员。 如果人员之前已取消订阅，我们将更新要取消订阅的记录。

## 更改电子邮件地址 {#changing-an-email-address}

如果将人员的电子邮件地址更改为未订阅的电子邮件地址，则将取消订阅该人员。 可以在Marketo或Salesforce中进行此更改。

如果您将取消订阅的电子邮件地址更改为已订阅的电子邮件地址，则该用户将变为已订阅。

## 重新订阅 {#re-subscribing}

正如取消订阅将导致所有拥有相同电子邮件地址的人被取消订阅一样，重新订阅实际上将重新订阅拥有相同电子邮件地址的每个人。

## 活动日志 {#activity-log}

数据值更改定义 _updateLeadEmailStatus_ 和 _resetLeadEmailStatus_ 可在以下位置找到： [此社区文章](https://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688).

>[!MORELIKETHIS]
>
>[了解取消订阅](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)

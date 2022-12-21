---
unique-page-id: 10094576
description: 持久取消订阅 — Marketo文档 — 产品文档
title: 持久取消订阅
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# 持久取消订阅 {#durable-unsubscribe}

Marketo增强了取消订阅功能的行为，使其“持久”。 我们添加了主控的电子邮件状态，该状态与人员详细信息记录中显示的取消订阅标记不同。

如果取消订阅标记将从false设置为true，则会更新主控电子邮件状态，并将所做的更改传播到具有相同电子邮件地址的其他人员。 如果删除并重新创建人员，或者使用相同的电子邮件地址创建新记录，则将显示取消订阅标记 **not** 被覆盖。

>[!NOTE]
>
>持久退订可跨整个Marketo数据库中的所有分区使用。

## 将“取消订阅”标志从True更新为False（例如，为人员重新订阅） {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

可以通过多种方式重新订阅人员。

在Salesforce中， **清除** 潜在客户/联系人记录中的电子邮件选择退出字段。 这将同步到Marketo。

![](assets/one.png)

在Marketo, **清除** 人员记录“信息”选项卡中的未订阅框。

![](assets/two.png)

运行 **更改数据值** 流程步骤，如下所示。

![](assets/three.png)

通过SOAP API更新现有人员。

## 创建新人员 {#creating-a-new-person}

创建新人员后，Marketo会根据主控电子邮件状态表检查该人员。 如果此人先前已退订，我们将更新该记录以退订。

## 更改电子邮件地址 {#changing-an-email-address}

如果您将人员的电子邮件地址更改为未订阅的电子邮件地址，则该人员将被取消订阅。 此更改可在Marketo或Salesforce中发生。

如果您将未订阅的电子邮件地址更改为已订阅的电子邮件地址，则该人将被订阅。

## 重新订阅 {#re-subscribing}

正如取消订阅会导致所有具有相同电子邮件地址的人取消订阅一样，重新订阅实际上也会使每个具有相同电子邮件地址的人重新订阅。

## 活动日志 {#activity-log}

数据值更改定义 _updateLeadEmailStatus_ 和 _resetLeadEmailStatus_ 可在 [此社区文章](https://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688).

>[!MORELIKETHIS]
>
>[了解取消订阅](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)

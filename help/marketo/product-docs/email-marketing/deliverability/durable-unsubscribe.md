---
unique-page-id: 10094576
description: 持久退订- Marketo Docs —— 产品文档
title: 持久退订
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# 持久退订 {#durable-unsubscribe}

Marketo增强了取消订阅功能的行为，使其“耐用”。 我们添加了主控的电子邮件状态，该状态与个人详细信息记录上可见的取消订阅标志分开。

如果取消订阅标志设置为false为true，则更新主控电子邮件状态，并将更改传播到具有相同电子邮件地址的其他人。 如果删除并重新创建人员，或者使用相同的电子邮件地址创建新记录，则不会覆 **盖** 取消订阅标志。

>[!NOTE]
>
>持久退订可跨整个Marketo数据库中的所有分区工作。

## 将取消订阅标志从True更新为False（例如，重新订阅人员） {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

可以通过多种方式重新订阅某个人。

在Salesforce中 **，清选择退出除Lead** /Contact记录上的“电子邮件”字段。 这将同步到Marketo。

![](assets/one.png)

在Marketo中 **，清** 除人员记录“信息”选项卡中取消订阅的框。

![](assets/two.png)

对一个或多个 **人员运行** “更改数据值流”步骤，如下所示。

![](assets/three.png)

通过SOAP API更新现有人。

## 创建新人员 {#creating-a-new-person}

创建新人员后，Marketo会根据主控电子邮件状态表检查该人员。 如果此人先前已取消订阅，我们将更新该记录以取消订阅。

## 更改电子邮件地址 {#changing-an-email-address}

如果将人员的电子邮件地址更改为未订阅的电子邮件地址，则该人员将取消订阅。 此更改可在Marketo或Salesforce中进行。

如果您将取消订阅的电子邮件地址更改为已订阅的电子邮件地址，则该人将被订阅。

## 重新订阅 {#re-subscribing}

正如取消订阅会导致所有具有相同电子邮件地址的人取消订阅一样，重新订阅实际上也会使每个人重新订阅具有相同电子邮件地址的人。

## 活动日志 {#activity-log}

可在此社区文 *章中找* 到 *updateLeadEmailStatus* 和resetLeadEmailStatus的 [数据值更改定义](http://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688)。

>[!NOTE]
>
>**相关文章**
>
>[了解取消订阅](understanding-unsubscribe.md)


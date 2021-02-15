---
unique-page-id: 10094576
description: 持久退订 — Marketo Docs — 产品文档
title: 持久退订
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---


# 持久退订{#durable-unsubscribe}

Marketo已增强了取消订阅功能的行为，使其“持久”。 我们添加了主控的电子邮件状态，该状态与个人详细信息记录上可见的取消订阅标志分开。

如果取消订阅标志设置为false到true，则会更新主控电子邮件状态，并将更改传播到具有相同电子邮件地址的其他人。 如果删除并重新创建人员，或者使用相同的电子邮件地址创建了新记录，则取消订阅标志将&#x200B;**不会覆盖**。

>[!NOTE]
>
>持久退订可以跨整个Marketo数据库中的所有分区工作。

## 将“取消订阅标志”从“True”更新为“False”（例如，重新订阅人员）{#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

可以通过多种方式重新订阅某个人。

在Salesforce中，**清除潜在客户/联系人记选择退出录上的“电子邮件”字段。**&#x200B;此操作将同步到Marketo。

![](assets/one.png)

在Marketo中，**清除人员记录“信息”选项卡中的取消订阅框。**

![](assets/two.png)

运行&#x200B;**更改数据值**&#x200B;流步骤，如下所示，对一个或多个人员。

![](assets/three.png)

通过SOAP API更新现有人。

## 创建新人{#creating-a-new-person}

创建新人员后，Marketo会根据主控电子邮件状态表检查该人员。 如果此人先前已取消订阅，我们将更新该记录以取消订阅。

## 更改电子邮件地址{#changing-an-email-address}

如果您将某人的电子邮件地址更改为未订阅的电子邮件地址，则该人将取消订阅。 此更改可在Marketo或Salesforce中发生。

如果您将未订阅的电子邮件地址更改为已订阅的电子邮件地址，则该人将会订阅。

## 重新订阅{#re-subscribing}

正如取消订阅会导致所有具有相同电子邮件地址的人取消订阅一样，重新订阅实际上会使每个具有相同电子邮件地址的人重新订阅。

## 活动日志{#activity-log}

_updateLeadEmailStatus_&#x200B;和&#x200B;_resetLeadEmailStatus_&#x200B;的数据值更改定义可在[此社区文章](https://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688)中找到。

>[!MORELIKETHIS]
>
>[了解取消订阅](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)

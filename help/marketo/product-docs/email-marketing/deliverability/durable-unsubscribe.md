---
unique-page-id: 10094576
description: 持久退订- Marketo Docs —— 产品文档
title: 持久退订
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---


# 持久退订{#durable-unsubscribe}

Marketo增强了取消订阅功能的行为，使其“耐用”。 我们添加了主控的电子邮件状态，该状态与个人详细信息记录上可见的取消订阅标志分开。

如果取消订阅标志设置为false为true，则更新主控电子邮件状态，并将更改传播到具有相同电子邮件地址的其他人。 如果删除并重新创建人员，或者使用相同的电子邮件地址创建新记录，则取消订阅标志将&#x200B;**不会**&#x200B;被覆盖。

>[!NOTE]
>
>持久退订可跨整个Marketo数据库中的所有分区工作。

## 将“取消订阅标志”从“True”更新为“False”（例如，重新订阅人员）{#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

可以通过多种方式重新订阅某个人。

在Salesforce中，**清除潜在客户／联系人记选择退出录中的电子邮件字段。**&#x200B;这将同步到Marketo。

![](assets/one.png)

在Marketo中，**清除人员记录“信息”选项卡中未订阅的框。**

![](assets/two.png)

运行&#x200B;**更改数据值**&#x200B;流步骤，如一个或多个人员中所示。

![](assets/three.png)

通过SOAP API更新现有人。

## 创建新人{#creating-a-new-person}

创建新人员后，Marketo会根据主控电子邮件状态表检查该人员。 如果此人先前已取消订阅，我们将更新该记录以取消订阅。

## 更改电子邮件地址{#changing-an-email-address}

如果将人员的电子邮件地址更改为未订阅的电子邮件地址，则该人员将取消订阅。 此更改可在Marketo或Salesforce中进行。

如果您将取消订阅的电子邮件地址更改为已订阅的电子邮件地址，则该人将被订阅。

## 重新订阅{#re-subscribing}

正如取消订阅会导致所有具有相同电子邮件地址的人取消订阅一样，重新订阅实际上也会使每个人重新订阅具有相同电子邮件地址的人。

## 活动日志{#activity-log}

数据值&#x200B;*updateLeadEmailStatus*&#x200B;和&#x200B;*resetLeadEmailStatus*&#x200B;的数据值更改定义可在[此社区文章](http://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688)中找到。

>[!MORELIKETHIS]
>
>[了解取消订阅](understanding-unsubscribe.md)


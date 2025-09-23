---
unique-page-id: 2950396
description: 优先级、紧迫性、相对分数和最佳匹配 — Marketo文档 — 产品文档
title: 优先级、紧急性、相对评分和最佳推荐
exl-id: 391aae00-e4f5-4fb1-8728-f5224276dfc2
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 1%

---

# 优先级、紧迫性、相对分数和[!DNL Best Bets] {#priority-urgency-relative-score-and-best-bets}

[!DNL Marketo Sales Insight]根据优先顺序选择您的最佳潜在客户和联系人。 潜在客户或联系人的优先级由两部分组成：紧迫性和相对分数。

![](assets/priority-urgency-relative-score-and-best-bets-1.png)

这些是从商机分数派生的，该分数用于衡量个人对您的产品的兴趣。 分数越高，他们就越有可能积极响应您销售团队的电话。

>[!NOTE]
>
>您需要多次评分营销活动才能获得优先级、紧急程度和相对分数的完整价值。  如果评分营销活动太少或没有，这些字段将毫无用处。

## 紧急 {#urgency}

火焰代表了一种紧迫感 — 这个人的商机分数最近发生了多大变化。 高度紧急（更易激动）意味着此潜在客户的分数最近增加了很多；这是一个很好的迹象，表明此潜在客户对您的选件感兴趣。 你应该尽快跟进这个人！

例如，一位潜在客户请求演示并访问了多个网页，他可能非常急切。 对于未访问您的网页或未打开您的电子邮件的潜在客户，其紧急程度较低。 利用紧迫性确定下一个需要联系的人的优先级。

![](assets/priority-urgency-relative-score-and-best-bets-2.png)

## 相对分数 {#relative-score}

星星代表相对得分 — 一个人的商机得分和其他人的商机得分相比较的指标。相对分数较高意味着相对于相对分数较低的人，此人可能对您的优惠更感兴趣，也更了解您的优惠。

如果两个潜在客户具有相同的紧迫性，您可以使用相对分数来判断哪一个客户应首先致电。 相对得分较高者对你的报价的反应可能比得分较低者更积极。

## [!DNL Best Bets] {#best-bets}

您的[!DNL Best Bets]是紧急性和相对分数最高的潜在客户和联系人。 只有您拥有的潜在客户会显示在列表中，并且列表会随着潜在客户分数的更改而更新。

>[!NOTE]
>
>如果最佳匹配与您拥有的最佳潜在客户和联系人不匹配，请与公司中有权访问Marketo的人员联系，了解如何更新[评分规则](/help/marketo/getting-started/quick-wins/simple-scoring.md)。

### 紧急程度和相对分数的计算方式

为了计算星星和火焰的数量，您的商机和联系人首先按得分或得分变化排序（分别针对相对得分和紧急程度）。 然后它们被分成几层 — 顶层接收最多的星星或火焰，而下一层接收较少的星星或火焰，以此类推。

随着得分的变化，紧急、优先级和相对得分值会立即重新计算。 每晚在Marketo服务器上自动计算紧急程度和相对得分级别。

>[!NOTE]
>
>“相对紧急程度（火焰）”和“相对得分（星星）”计数是Marketo中的整数。 每个可能的值均为0-3。

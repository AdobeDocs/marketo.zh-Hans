---
unique-page-id: 10096583
description: 下一代Munchkin跟踪常见问题解答- Marketo Docs —— 产品文档
title: 下一代Munchkin跟踪常见问题解答
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---


# 下一代Munchkin跟踪常见问题解答{#next-generation-munchkin-tracking-faq}

我们很高兴地宣布，我们将很快开始分阶段推出我们的下一代网络跟踪技术。

以下是最重要的信息：

* 我们将在第1季度版本中删除“是匿名的”智能列表过滤器（已完成）
* 我们正在增加可以收录的Web事件（访问网页、网页上的点击链接）的数量
* 您的Munchkin代码不会更改，因此无需更新网站

## 我的营销订阅什么时候上Munchkin V2?{#when-will-my-marketo-subscription-be-on-munchkin-v}

我们还没有确切的日期，但请查阅此处以获取更新。

## 我是否需要在我的网站上对Munchkin跟踪进行任何更改？{#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

不。 蒙奇金跟踪代码保持不变。 无需对网站进行任何更改。

>[!NOTE]
>
>此更改不会影响Web个性化（实时个性化）。 它继续识别匿名和已知的Web访客，并为这些访客实时个性化内容。

## 为什么Marketo从智能列表中删除“匿名”过滤器？{#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

我们改变了匿名人士与智能活动互动的方式。 以前，他们像熟人一样，经历着聪明的活动。 “是匿名的”过滤器用于指定只有已知或只有匿名人员才能通过活动。

通过Munchkin V2，我们将继续跟踪所有匿名活动;但是，您不再能将过滤器应用于匿名人员。 在转换点（当该人在Marketo中变为已知者），当此人为匿名者时发生的所有活动都会附加到人员活动日志中，此时，这些活动会流过他们有资格获得的。

如果您已经在智能列表(例如，在智能活动或报表中)中使用此过滤器，则不会自动从智能列表中删除该过滤器。 有关更多详细信息，请参见下文。

>[!NOTE]
>
>**触发器**:访问网页，网页是定价页\
>**流程**:更改得分+10和有趣时刻
>**Web**:查看的定价页面
>
>对于Munchkin V2，如果匿名人士访问定价页面，她不会立即进入活动。 当匿名者被曝光时，我们会对她进行活动。 她会：
>
>* 获得10分
   >
   >
* 将网页活动设置为正确的日期（她实际访问时）
   >
   >
* 为她记录一个有趣的时刻（她实际访问该页面的日期，而非她出现时）
   >
   >
* 记录“新人”活动，就像今天一样


## 我的智能列表已经具有“匿名”过滤器，会发生什么情况？{#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

在我们的“16年冬季版”发布后，如果您有具有智能活动的旧智能列表，其中包含“匿名”过滤器，则会发生以下两种情况之一：

1. 如果智能列表具有过滤器“Is Anonymous = False”，则不会发生任何情况。 我们就忽略它。
1. 如果智能列表具有过滤器“Is Anonymous = True”，则此活动将失败，您将收到通知。

## 我使用Marketo已有一段时间了。 我如何知道哪位活动使用“匿名”过滤器？{#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

在进行此更改之前，我们会向您的通知收件箱发送多个每周通知，其中包含使用“匿名”过滤器的列表智能列表、智能活动和报告。 这些过滤器可以帮助您确定当前使用此过滤器的位置。

请查看它们并确定“匿名”设置为True的位置，因为这些是受影响的活动。 大多数情况下，客户使用此设置进行某种评分。 请参阅上面的示例，了解这些活动现在如何工作。

## 我想要更详细的文档。 我在哪里可以找到它？{#id-like-more-detailed-documentation-where-can-i-find-it}

查看以下链接：

[匿名潜在客户升级概述](https://nation.marketo.com/docs/DOC-2937)

[匿名潜在客户升级——在营销UI中的更改](https://nation.marketo.com/docs/DOC-2938)

[匿名潜在客户升级——需要客户行动](https://nation.marketo.com/docs/DOC-2939)

[匿名潜在客户升级——分析报告](https://nation.marketo.com/docs/DOC-2940)

[匿名潜在客户升级——发布计划](https://nation.marketo.com/docs/DOC-2961)

[匿名潜在客户升级——不足](https://nation.marketo.com/docs/DOC-2962)

[对已知潜在客户的匿名潜在客户促销- Munchkin V2行为](https://nation.marketo.com/docs/DOC-2963)

## 我有更多问题！ 我如何获得答案？{#i-have-more-questions-how-do-i-get-them-answered}

请访问[社区](https://nation.marketo.com/welcome)。 您也可以联系[Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support)。 他们会乐意回答你的问题。

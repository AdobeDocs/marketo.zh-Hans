---
unique-page-id: 10096583
description: 下一代Munchkin跟踪常见问题解答 — Marketo文档 — 产品文档
title: 下一代Munchkin跟踪常见问题解答
exl-id: 283189ac-c817-479a-b896-91233980608c
source-git-commit: 813bab6169a121e90919f9a02505ccde5167cda4
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# 下一代Munchkin跟踪常见问题解答 {#next-generation-munchkin-tracking-faq}

我们很高兴地宣布，我们很快将开始分阶段推出我们的下一代Web跟踪技术。

以下是需要了解的最重要事项：

* 我们将在第1季度版本（已完成）中删除“Is Anonymous”智能列表筛选器
* 我们正在增加可摄取的Web事件数（访问网页、网页上的已点击链接）
* 您的Munchkin代码不会更改，因此无需在您的网站上进行任何更新

## 我的Marketo订购什么时候上Munchkin V2? {#when-will-my-marketo-subscription-be-on-munchkin-v}

我们还没有确切的日期，但请返回此处获取更新。

## 我是否需要对网站上的Munchkin跟踪进行任何更改？ {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

否. Munchkin跟踪代码保持不变。 无需对您的网站进行任何更改。

>[!NOTE]
>
>此更改不会影响Web个性化（实时个性化）。 它会继续识别匿名和已知的Web访客，并对这些访客实时个性化内容。

## 为什么Marketo从智能列表中删除了“匿名”过滤器？ {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

我们更改了匿名用户与智能营销活动的交互方式。 以前，他们像知名人一样，通过一场聪明的运动。 “是匿名”过滤器用于指定只有已知或只有匿名人员才能在营销活动中流动。

通过Munchkin V2，我们将继续跟踪所有匿名活动；但是，您无法再将过滤器应用于匿名人员。 转化时(当人员在Marketo中变为已知)，当该人员为匿名时发生的所有活动都会附加到人员活动日志中，此时，这些活动会流过他们有资格参与的营销活动。

如果您已在智能列表中使用此过滤器（例如，在智能营销活动或报表中），则不会自动从智能列表中将其删除。 有关更多详细信息，请参阅下文。

>[!NOTE]
>
>**触发器**:“访问”网页、“网页”是“定价”页\
>**流量**:更改分数+10和有趣的时刻
>**Web**:查看的定价页面
>
>使用Munchkin V2时，如果匿名人员访问定价页面，则她不会立即进入营销活动。 当匿名者被曝光时，我们会对她进行这项运动。 她会：
>
>* 得10分
>
>* 将网页活动设置到正确的日期（实际访问的时间）
>
>* 为她记录了一个有趣的时刻（她实际访问页面的日期，而不是她知道的日期）
>
>* 记录“新人”活动（如今）


## 我的智能列表已具有“匿名”过滤器，但该智能列表会出现什么情况？ {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

在’16年冬季版本发布后，如果您有旧的智能营销活动，且智能列表中具有“匿名”过滤器，则会发生以下两种情况之一：

1. 如果智能列表具有过滤器“Is Anonymous = False”，则不会发生任何情况。 我们就忽略它。
1. 如果智能列表具有过滤器“Is Anonymous = True”，则此营销活动将失败，您将收到通知。

## 我用了Marketo一段时间了。 如何知道我的哪些营销活动使用“匿名”过滤器？ {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

在进行此更改之前，我们每周向您的通知收件箱发送多条通知，其中包含使用“匿名”过滤器的智能列表、智能营销活动和报表列表。 这些功能可帮助您确定当前使用此过滤器的位置。

请查看这些变量，并确定将“匿名”设置为True的位置，因为这些是受影响的营销活动。 大多数情况下，客户会使用此设置进行某种评分。 请参阅上面的示例，了解这些营销活动现在如何工作。

## 我想要更详细的文档。 在哪里可以找到它？ {#id-like-more-detailed-documentation-where-can-i-find-it}

请查看以下链接：

[匿名潜在客户升级概述](https://nation.marketo.com/docs/DOC-2937){target=&quot;_blank&quot;}

[匿名潜在客户升级 — 更改了Marketo UI](https://nation.marketo.com/docs/DOC-2938){target=&quot;_blank&quot;}

[匿名潜在客户升级 — 需要客户操作](https://nation.marketo.com/docs/DOC-2939){target=&quot;_blank&quot;}

[匿名潜在客户升级 — Analytics报表](https://nation.marketo.com/docs/DOC-2940){target=&quot;_blank&quot;}

[匿名潜在客户升级 — 发行计划](https://nation.marketo.com/docs/DOC-2961){target=&quot;_blank&quot;}

[匿名潜在客户升级 — 隐藏](https://nation.marketo.com/docs/DOC-2962){target=&quot;_blank&quot;}

[将匿名潜在客户提升为已知潜在客户 — Munchkin V2行为](https://nation.marketo.com/docs/DOC-2963){target=&quot;_blank&quot;}

## 我还有更多问题！ 我该如何得到他们的回答？ {#i-have-more-questions-how-do-i-get-them-answered}

请在 [社区](https://nation.marketo.com/){target=&quot;_blank&quot;}。 您还可以联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support){target=&quot;_blank&quot;}。 他们很乐意回答你的问题。

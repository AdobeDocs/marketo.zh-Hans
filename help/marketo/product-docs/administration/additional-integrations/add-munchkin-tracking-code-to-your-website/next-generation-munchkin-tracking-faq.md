---
unique-page-id: 10096583
description: “新一代 [!DNL Munchkin] 跟踪常见问题解答 — Marketo文档 — 产品文档”
title: “新一代 [!DNL Munchkin] 跟踪常见问题解答”
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---

# 下一代 [!DNL Munchkin] 跟踪常见问题解答 {#next-generation-munchkin-tracking-faq}

我们很高兴地宣布，我们很快将开始分阶段推出新一代网络跟踪技术。

以下是需要了解的最重要事项：

* 我们正在删除第1季度版本的“匿名”智能列表过滤器（已完成）
* 我们正在增加可以摄取的Web事件（访问网页、已点击网页上的链接）的数量
* 您的 [!DNL Munchkin] 代码不会更改，因此无需对您的网站进行更新

## 我的Marketo订阅将于何时启用 [!DNL Munchkin] V2？ {#when-will-my-marketo-subscription-be-on-munchkin-v}

我们还没有确切日期，但请返回此处查看更新。

## 我是否需要对 [!DNL Munchkin] 在我的网站上进行跟踪？ {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

否. 此 [!DNL Munchkin] 跟踪代码保持不变。 无需对您的网站进行更改。

>[!NOTE]
>
>此更改不影响Web个性化（实时个性化）。 它将继续识别匿名和已知的Web访客，并实时为这些访客个性化内容。

## 为什么Marketo从智能列表中移除“是匿名”筛选器？ {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

我们更改了匿名用户与Smart Campaigns的交互方式。 以前，他们像知名人士一样，参加过一场明智的竞选。 “是匿名的”过滤器用于指定只有已知或仅匿名人员流经该营销活动。

替换为 [!DNL Munchkin] V2，我们将继续跟踪所有匿名活动；但是，您无法再对匿名人员应用筛选器。 在转化时(此人在Marketo中成为已知人时)，此人匿名时发生的所有活动都将附加到人员活动日志中，并且在此时这些活动会流经他们有资格参加的营销活动。

如果您已在智能列表中（例如，在智能营销活动或报表中）使用此筛选器，则不会自动将其从智能列表中删除。 有关更多详细信息，请参阅下文。

>[!NOTE]
>
>**触发器**：访问次数网页，该网页为定价页面\
>**流量**：更改得分+10和有趣的时刻
>**Web**：已查看定价页面
>
>替换为 [!DNL Munchkin] V2，如果匿名人员访问定价页面，她不会立即进入促销活动。 当匿名者被认出时，我们就会对她发起这个运动。 她将：
>
>* 得到10分
>
>* 将网页活动设置为正确的日期（她实际访问的时间）
>
>* 为她记录了一个有趣的时刻（记录她实际访问页面的日期，而不是她何时为人所知）
>
>* 像今天这样记录“新人员”活动

## 已具有“是匿名的”过滤器的智能列表会发生什么情况？ {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

在我们的2016年冬季版本发布后，如果您有带有智能列表的旧智能营销活动，其中包含“Is Anonymous”过滤器，则将发生以下两种情况之一：

1. 如果智能列表具有过滤器“Is Anonymous = False”，则不会发生任何情况。 我们忽略它。
1. 如果智能列表具有“Is Anonymous = True”过滤器，则此营销活动将失败，并将向您发送通知。

## 我使用Marketo已经有一段时间了。 我如何知道我的哪些营销活动使用“是匿名的”过滤器？ {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

在进行此更改之前，我们已将多个每周通知发送到您的“通知”收件箱，其中包含使用“匿名”过滤器的智能列表、智能营销活动和报告的列表。 它们可以帮助您识别当前使用此过滤器的位置。

请检查这些标记，并识别在何处将“匿名”设置为True，因为这些是受影响的营销活动。 大多数情况下，客户使用此设置进行某种评分。 请参阅上面的示例，以了解这些营销活动现在将如何工作。

## 我想要更详细的文档。 我可以在哪里找到它？ {#id-like-more-detailed-documentation-where-can-i-find-it}

查看以下链接：

[匿名潜在客户升级概述](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[匿名潜在客户升级 — Marketo UI中的更改](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[匿名潜在客户升级 — 需要客户操作](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[匿名潜在客户升级 — Analytics报告](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[匿名潜在客户升级 — 发布计划](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[匿名潜在客户升级 — 隐蔽](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[匿名潜在客户促销至已知潜在客户 —  [!DNL Munchkin] V2行为](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## 我还有更多问题！ 我如何才能得到他们的答复？ {#i-have-more-questions-how-do-i-get-them-answered}

请联系 [社区](https://nation.marketo.com/){target="_blank"}. You can also contact [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}. 他们很乐意回答你的问题。

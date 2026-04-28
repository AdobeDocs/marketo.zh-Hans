---
unique-page-id: 10096583
description: 有关新一代 [!DNL Munchkin] 跟踪转出和Is Anonymous筛选器更改的常见问题解答。
title: 下一代 [!DNL Munchkin] 跟踪常见问题解答
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
hidefromtoc: true
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# 下一代[!DNL Munchkin]跟踪常见问题解答 {#next-generation-munchkin-tracking-faq}

Marketo is rolling out next-generation web tracking technology in phases.

以下是需要了解的最重要事项：

* 已删除“Is Anonymous”智能列表筛选器
* Marketo可以摄取的Web事件（访问网页、点击网页上的链接）数量正在增加
* 您的[!DNL Munchkin]代码不会更改，因此无需更新您的网站

## 我的Marketo订阅何时将使用[!DNL Munchkin] V2？ {#when-will-my-marketo-subscription-be-on-munchkin-v}

确切日期尚不可用。 Check this page for updates.

## 我是否需要对我网站上的[!DNL Munchkin]跟踪进行任何更改？ {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

不会。 [!DNL Munchkin]跟踪代码保持不变。 无需对您的网站进行更改。

>[!NOTE]
>
>此更改不会影响Web Personalization (Real-Time Personalization)。 它将继续识别匿名和已知的Web访客，并对这些访客实时地个性化内容。

## 为什么Marketo从智能列表中移除“是匿名的”筛选器？ {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Marketo changed how anonymous people interact with Smart Campaigns. 以前，他们像知名人士一样，参加一场聪明的竞选。 “是匿名的”过滤器用于指定仅已知或仅匿名人员流经营销活动。

使用[!DNL Munchkin] V2时，Marketo将继续跟踪所有匿名活动；但是，您无法再对匿名人员应用筛选器。 在转化时（此人在Marketo中成为已知人时），该人员匿名时发生的所有活动都将附加到人员活动日志中，并且在此时这些活动会流经他们符合条件的营销活动。

如果您已在智能列表中（例如，在智能营销活动或报表中）使用此筛选器，则不会自动将其从智能列表中删除。 有关更多详细信息，请参阅下文。

>[!NOTE]
>
>**触发器**：访问网页，网页为定价页面&#x200B;>**Flow**: Change Score +10 and Interesting Moment >**Web**: Viewed Pricing Page
>
>With [!DNL Munchkin] V2, if an anonymous person visits the pricing page, they do not enter the campaign immediately. At the time the anonymous person becomes known, Marketo runs this campaign on them. They will:
>
>* Get a score of 10
>
>* Have the Web Page activity set to the right date (when they actually visited)
>
>* Have an Interesting Moment logged for them (with the date they actually visited the page, not when they became known)
>
>* Have a &quot;New Person&quot; activity logged, as it is today

## What happens to my Smart Lists that already have the &quot;Is Anonymous&quot; filter? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

After the Winter &#39;16 Release, if you have old Smart Campaigns with a Smart List that has the &quot;Is Anonymous&quot; filter in it, one of two things will happen:

1. If the Smart List has the filter &quot;Is Anonymous = False&quot;, then nothing will happen. It is ignored.
1. If the Smart List has the filter &quot;Is Anonymous = True&quot;, this campaign will fail and a notification is sent.

## I have been using Marketo for a while. How do I know which of my campaigns use the &quot;Is Anonymous&quot; filter? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Before this change, Marketo sent several weekly notifications to your Notifications inbox with a list of Smart Lists, Smart Campaigns and Reports that use the &quot;Is Anonymous&quot; filter. These can help you identify where you are currently using this filter.

Review them and identify where you have &quot;Is Anonymous&quot; set to True, as these are the campaigns that are affected. Most times, this setting is used for some kind of scoring. See the example above to understand how these campaigns will work now.

## I would like more detailed documentation. Where can I find it? {#id-like-more-detailed-documentation-where-can-i-find-it}

Check out these links:

[Anonymous Lead Upgrades Overview](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[匿名潜在客户升级 — Marketo UI中的更改](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[匿名潜在客户升级 — 需要客户操作](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[匿名潜在客户升级 — Analytics报告](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[匿名潜在客户升级 — 发布计划](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[匿名潜在客户升级 — 隐秘的](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[匿名潜在客户促销至已知潜在客户 —  [!DNL Munchkin] V2行为](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## 我有更多问题！ 怎样才能得到他们的答复？ {#i-have-more-questions-how-do-i-get-them-answered}

访问[Marketo社区](https://experienceleaguecommunities.adobe.com/?profile.language=zh-Hans){target="_blank"}。 您还可以联系Marketo支持部门。 他们很高兴回答您的问题。

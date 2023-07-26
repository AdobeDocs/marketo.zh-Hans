---
unique-page-id: 7514898
description: 使用“已请求营销活动”设置触发器智能营销活动 — Marketo文档 — 产品文档
title: 使用“Campaign is Requested”设置触发器智能促销活动
exl-id: ed6d7c27-d54b-48e3-af67-19503da4ef56
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 使用“Campaign is Requested”设置触发器智能促销活动 {#setting-up-a-trigger-smart-campaign-for-sales-using-campaign-is-requested}

Marketo最酷的功能之一是允许销售人员参与营销工作。 他们站在前线，与人互动。 销售代表应能够向正确的方向引导营销。

>[!NOTE]
>
>要请求的智能营销活动示例：
>
>1. **长期培养**  — 当他们今年没有预算，而你只是想保持低调
>1. **有效的销售周期**  — 当销售人员不希望向该人员发送任何消息（他们自己的消息除外）时。 （使用营销活动暂停标记可临时取消订阅这些页面）
>
>发挥创造力。 销售人员希望实现什么自动化？ 只要问问他们，然后把它接上去！

1. 创建 **Smart Campaign。**

   ![](assets/image2015-5-20-16-3a3-3a25.png)

1. 查找并拖动 **已请求营销活动** 到画布上。

   ![](assets/campaignfilterdrag.png)

1. 源选择指示将接受哪种请求。 对于Salesforce功能，请确保选择 **销售** **Insight**.

   >[!TIP]
   >
   >源操作符用于安全目的。 您可以将营销活动限制为仅由特定来源（例如其他智能营销活动或开发人员）发出的请求。 选择 **为任意** ，以允许您允许来自所有源的请求。
   >
   >**记住**，通过选择Sales Insight ，它将神奇地显示在销售框中。 不要做得过火。 太多的人会被他们忽视。

   ![](assets/image2015-5-20-17-3a56-3a56.png)

这是将营销范围扩展到其他部门的绝佳方法。 设置各种要自动化的营销活动。

>[!TIP]
>
>不要忘记为您的智能营销活动指明清楚的名字。 它们将会在Sales Insight中完全按照您的命名方式显示。

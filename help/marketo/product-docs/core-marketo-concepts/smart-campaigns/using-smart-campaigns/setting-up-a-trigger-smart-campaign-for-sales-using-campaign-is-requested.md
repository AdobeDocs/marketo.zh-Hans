---
unique-page-id: 7514898
description: 了解如何使用Campaign is Requested为销售设置触发器Smart Campaign。 允许销售人员从CRM请求营销活动，以获取商机。
title: 使用“请求营销活动”设置销售触发型智能营销活动
exl-id: ed6d7c27-d54b-48e3-af67-19503da4ef56
feature: Smart Campaigns
source-git-commit: 60c5603fa29bb1039b9d477633beb2c6f5c63486
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 11%

---

# 使用“请求营销活动”设置销售触发型智能营销活动 {#setting-up-a-trigger-smart-campaign-for-sales-using-campaign-is-requested}

Marketo最酷的功能之一是允许销售人员参与营销工作。 他们站在前线，与人互动。 销售代表应能够向正确的方向引导营销。

>[!NOTE]
>
>要请求的智能营销活动示例：
>
>1. **长期培养** — 当他们今年没有预算，而您希望保持关注时
>1. **有效的销售周期** — 当销售人员不希望向该人员发送除他们自己之外的任何消息时。 （使用营销活动暂停标记可临时取消订阅这些页面）
>
>询问销售团队他们希望实现什么自动化并进行设置。

1. 创建智能营销活动。

   ![](assets/setting-up-a-trigger-smart-campaign-for-sales-1.png)

1. 找到并将 **[!UICONTROL Campaign is Requested]** 触发器拖动到画布上。

   ![](assets/setting-up-a-trigger-smart-campaign-for-sales-2.png)

1. 源选择指示将接受哪种请求。 对于Salesforce功能，请选择&#x200B;**[!UICONTROL Sales Insight]**。

   >[!TIP]
   >
   >源操作符用于安全目的。 您可以将营销活动限制为仅由特定来源（如其他智能营销活动或开发人员）发出的请求。 如果要允许来自所有源的请求，请在第一个框中选择&#x200B;**[!UICONTROL Is Any]**。
   >
   >_请记住_，选择Sales Insight后，它将会神奇地显示在销售盒中。 避免添加太多，因为它们将被忽略。

   ![](assets/setting-up-a-trigger-smart-campaign-for-sales-3.png)

这是将营销范围扩展到其他部门的绝佳方法。 设置各种要自动化的营销活动。

>[!TIP]
>
>清楚地命名您的智能营销活动。 它们将在Sales Insight中完全按照您的命名方式显示。

---
unique-page-id: 1146940
description: 为Smart Campaign定义智能列表 |批次 — Marketo文档 — 产品文档
title: 为Smart Campaign定义智能列表 |批次
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# 为Smart Campaign定义智能列表 |批次 {#define-smart-list-for-smart-campaign-batch}

智能列表是整个Marketo Engage中用于定义“人员”（哪些人员）的机制，包括报表、列表或智能营销活动。 以下是如何为批处理营销活动定义智能列表。

1. 选择一个智能营销活动，然后单击 **[!UICONTROL 智能列表]**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. 键入以搜索过滤器，并将其拖放到画布上。 对多个筛选器重复执行上述操作。

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >仅包含过滤器的智能营销活动在中运行 _批次_ 模式。 它会在数据库中找到根据过滤器符合条件的人员，并一次性在流中运行所有这些人员。

   >[!NOTE]
   >
   >您可以通过添加触发器来使Smart Campaign每次基于实时事件对一个人运行，这会将Smart Campaign置于 _触发器_ 模式。

1. 单击下拉列表，并为所选的过滤器选择过滤器运算符。

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >红色曲线表示错误或缺少信息。 如果未更正，则营销活动将无效且不会运行。

1. 输入筛选值。

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >默认情况下，满足所有智能列表规则的用户是符合条件的。 您可以根据营销策划需求对此进行修改。 签出  [适用于复杂逻辑的智能列表规则](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"} 了解更多信息。

   要一次触发一个人的实时事件，了解如何 [为Smart Campaign定义智能列表 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}.

   >[!MORELIKETHIS]
   >
   >* [为Smart Campaign定义智能列表 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
   >* [向智能营销活动添加流量步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

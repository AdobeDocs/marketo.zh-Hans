---
unique-page-id: 1146940
description: 为智能营销活动定义智能列表 |批处理 — Marketo文档 — 产品文档
title: 为智能营销活动定义智能列表 |批
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# 为智能营销活动定义智能列表 |批 {#define-smart-list-for-smart-campaign-batch}

智能列表是整个Marketo中定义“谁”（包括哪些人员）的机制，无论是报表、列表还是智能营销活动。 以下是如何为批量营销活动定义智能列表。

1. 选择智能营销活动，然后单击 **智能列表**.

   ![](assets/campaignchoose-hand.png)

1. 键入以搜索过滤器，然后将其拖放到画布中。 对多个过滤器重复执行上述步骤。

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >仅在中运行过滤器的智能营销活动 **批次** 模式。 它会在数据库中查找根据过滤器符合条件的人员，并同时通过流程运行所有这些人员。

   >[!NOTE]
   >
   >您可以通过添加触发器，根据实时事件，一次在一个人上运行智能营销活动，这会将智能营销活动置于 **触发器** 模式。

1. 单击下拉列表，然后为您选择的过滤器选择过滤器运算符。

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >红色的曲线表示错误或缺少信息。 如果未更正，则营销活动将无效，且不会运行。

1. 输入筛选值。

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >默认情况下，满足“所有”智能列表规则的人员符合条件。 可以根据您的营销活动需求对此进行修改。 查看  [复杂逻辑的智能列表规则](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md) 以了解更多。

   要逐个触发实时事件，请了解如何 [为智能营销活动定义智能列表 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [为智能营销活动定义智能列表 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [向智能营销活动添加流量步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)


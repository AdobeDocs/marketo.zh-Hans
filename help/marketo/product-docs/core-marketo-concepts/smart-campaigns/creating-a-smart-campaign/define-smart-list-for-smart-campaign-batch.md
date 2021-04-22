---
unique-page-id: 1146940
description: 为智能列表定义智能活动 |批处理 — Marketo文档 — 产品文档
title: 为智能列表定义智能活动 |批处理
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# 为智能列表定义智能活动 |批{#define-smart-list-for-smart-campaign-batch}

智能列表是整个Marketo中定义要包含的“谁”（哪些人）的机制，无论是报表、列表还是智能活动。 下面介绍如何为批处理列表定义智能活动。

1. 选择智能活动，然后单击&#x200B;**智能列表**。

   ![](assets/campaignchoose-hand.png)

1. 键入以搜索筛选器，然后将其拖放到画布。 对多个过滤器重复上述步骤。

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >仅具有过滤器的智能活动在&#x200B;**批**&#x200B;模式下运行。 它在数据库中根据过滤器查找符合条件的人员，并同时在流中运行所有这些人员。

   >[!NOTE]
   >
   >您可以通过添加触发器，使智能活动每次基于实时事件在一个人上运行，这会将智能活动置于&#x200B;**触发器**&#x200B;模式。

1. 单击下拉列表，然后为您选择的过滤器选择过滤器运算符。

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >红色波浪线指示错误或缺少信息。 如果未更正，活动将无效且不运行。

1. 输入筛选值。

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >默认情况下，符合所有智能列表规则的人员是合格的。 可以修改此项以满足您的活动需求。 请查阅[复杂逻辑的智能列表规则](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)以了解更多信息。

   要一次触发实时事件，请了解如何[为智能列表定义智能活动 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)。

   >[!MORELIKETHIS]
   >
   >* [为智能列表定义智能活动 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [向智能活动添加流步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)


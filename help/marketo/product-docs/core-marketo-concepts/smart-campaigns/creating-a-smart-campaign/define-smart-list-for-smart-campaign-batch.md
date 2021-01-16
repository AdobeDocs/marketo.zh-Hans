---
unique-page-id: 1146940
description: 为智能列表定义智能活动 |批处理——营销文档——产品文档
title: 为智能列表定义智能活动 |批处理
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---


# 为智能列表定义智能活动 |批{#define-smart-list-for-smart-campaign-batch}

智能列表是整个市场中定义“谁”（哪些人）的机制，包括报告、列表或智能活动。 下面介绍如何为批处理列表定义智能活动。

1. 选择智能活动，然后单击&#x200B;**智能列表**。

   ![](assets/campaignchoose-hand.png)

1. 键入以搜索筛选器，然后将其拖放到画布中。 对多个过滤器重复上述步骤。

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >仅具有过滤器的智能活动在&#x200B;**Batch**&#x200B;模式下运行。 它会根据过滤器在数据库中查找符合条件的人员，并同时在流中运行所有这些人员。

   >[!NOTE]
   >
   >通过添加触发器，可以使智能活动根据实时事件一次运行于一个人上，这将智能活动置于&#x200B;**触发器**&#x200B;模式。

1. 单击下拉列表，然后为您选择的筛选器选择筛选器运算符。

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >红色波浪线表示错误或缺少信息。 如果未更正，活动将无效且无法运行。

1. 输入筛选值。

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >默认情况下，符合所有智能列表规则的人员均符合条件。 可以修改此项以满足您的活动需求。 请查阅[复杂逻辑的智能列表规则](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)以了解更多信息。

   要一次触发实时事件，请学习如何[为智能列表定义智能活动 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)。

   >[!MORELIKETHIS]
   >
   >* [为智能列表定义智能活动 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [向智能活动添加流步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)


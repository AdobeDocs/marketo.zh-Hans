---
unique-page-id: 1146940
description: 为Smart Campaign定义智能列表 | 批次 — Marketo文档 — 产品文档
title: 为Smart Campaign定义智能列表 | 批次
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: c3aa1a29b084cb1c1add9d22cdbfc23bdcf7512b
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# 为Smart Campaign定义智能列表 | 批次 {#define-smart-list-for-smart-campaign-batch}

智能列表是整个Marketo Engage中用于定义“人员”（哪些人员）的机制，包括报表、列表或智能营销活动。 以下是如何为批处理营销活动定义智能列表。

>[!CAUTION]
>
>对活动营销活动进行智能列表或流程步骤编辑可能会破坏其功能。 如果您选择这么做，请谨慎操作。

1. 选择智能营销活动，然后单击&#x200B;**[!UICONTROL 智能列表]**。

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. 键入以搜索过滤器，并将其拖放到画布上。 对多个筛选器重复执行上述操作。

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >仅包含筛选器的智能营销活动在&#x200B;_批处理_&#x200B;模式下运行。 它会在数据库中找到根据过滤器符合条件的人员，并一次性在流中运行所有这些人员。

   >[!NOTE]
   >
   >您可以通过添加触发器使Smart Campaign处于&#x200B;_触发器_&#x200B;模式，根据实时事件逐人运行Smart Campaign。

1. 单击下拉列表，并为所选的过滤器选择过滤器运算符。

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >红色曲线表示错误或缺少信息。 如果未更正，则营销活动将无效且不会运行。

1. 输入筛选值。

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >默认情况下，满足所有智能列表规则的用户是符合条件的。 您可以根据营销策划需求对此进行修改。 请查看复杂逻辑的[智能列表规则](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}以了解更多信息。

   要在实时事件中一次触发一个人，了解如何[为Smart Campaign定义智能列表 | 触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}。

   >[!MORELIKETHIS]
   >
   >* [为智能营销活动定义智能列表 | 触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
   >* [向智能营销活动添加流程步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

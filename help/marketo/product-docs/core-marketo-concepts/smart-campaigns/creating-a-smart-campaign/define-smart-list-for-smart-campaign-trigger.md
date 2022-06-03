---
unique-page-id: 1146942
description: 为智能营销活动定义智能列表 |触发器 — Marketo文档 — 产品文档
title: 为智能营销活动定义智能列表 |触发器
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
source-git-commit: a15a4b9bccb069b51186aac7b913008d15aa645e
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# 为智能营销活动定义智能列表 |触发器 {#define-smart-list-for-smart-campaign-trigger}

通过添加触发器，根据实时事件，一次在一个人上运行智能营销活动。

1. 在您的智能营销活动中，单击 **智能列表** 选项卡。

   ![](assets/image2014-9-19-16-3a22-3a55.png)

1. 搜索触发器，然后将触发器拖放到画布中。

   ![](assets/image2014-9-19-16-3a23-3a24.png)

   >[!NOTE]
   >
   >具有触发器的智能营销活动在中运行 **触发器** 模式。 它根据触发的事件和任何其他过滤器一次只在一个人上运行。

   >[!IMPORTANT]
   >
   >在触发器促销活动智能列表中使用布尔字段时，必须将其明确设置为“false”，以便该字段在执行促销活动期间正确评估。

1. 单击下拉列表，然后选择运算符。

   ![](assets/image2014-9-19-16-3a23-3a29.png)

   >[!CAUTION]
   >
   >红色的曲线表示错误或缺少信息。 如果未更正，则营销活动将无效，且不会运行。

   >[!TIP]
   >
   >在同时具有触发器和过滤器的智能营销活动中，触发器位于顶部，触发时，只有满足过滤器标准的用户才会进入流程。

1. 定义触发器。

   ![](assets/image2014-9-19-16-3a24-3a36.png)

   >[!NOTE]
   >
   >使用多个触发器时，如果 **任意** 其中一个触发器将被激活。

要同时针对一组人员运行营销活动，请了解如何 [为智能营销活动定义智能列表 |批](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

>[!MORELIKETHIS]
>
>[向智能营销活动添加流量步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

---
unique-page-id: 1146942
description: 为Smart Campaign定义智能列表 | 触发器 — Marketo文档 — 产品文档
title: 为Smart Campaign定义智能列表 | 触发器
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
feature: Smart Campaigns
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# 为Smart Campaign定义智能列表 | 触发器 {#define-smart-list-for-smart-campaign-trigger}

通过添加触发器，根据实时事件逐人运行Smart Campaign。

>[!CAUTION]
>
>对活动营销活动进行智能列表或流程步骤编辑可能会破坏其功能。 如果您选择这么做，请谨慎操作。

1. 在Smart Campaign中，单击&#x200B;**[!UICONTROL Smart List]**&#x200B;选项卡。

   ![](assets/define-smart-list-for-smart-campaign-trigger-1.png)

1. 搜索所需的触发器，并将其拖放到画布上。

   ![](assets/define-smart-list-for-smart-campaign-trigger-2.png)

   >[!NOTE]
   >
   >带有触发器的Smart Campaign在&#x200B;_触发器_&#x200B;模式下运行。 它根据触发的事件和任何其他过滤器，每次只针对一个人运行。

   >[!IMPORTANT]
   >
   >在触发器促销活动智能列表中使用布尔字段时，必须将其明确设置为“false”，以便该字段在执行促销活动期间正确评估。

1. 单击下拉菜单并选择运算符。

   ![](assets/define-smart-list-for-smart-campaign-trigger-3.png)

   >[!CAUTION]
   >
   >红色曲线表示错误或缺少信息。 如果未更正，则营销活动将无效且不会运行。

   >[!TIP]
   >
   >在同时具有触发器和过滤器的Smart Campaign中，触发器位于顶部，触发时，只有符合筛选条件的用户才会流过。

1. 定义触发器。

   ![](assets/define-smart-list-for-smart-campaign-trigger-4.png)

   >[!NOTE]
   >
   >对于多个触发器，如果激活了&#x200B;_ANY_&#x200B;其中一个触发器，则人员会通过流程。

若要同时对一组人员运行营销活动，请了解如何[为智能营销活动定义智能列表 | 批次](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}。

>[!MORELIKETHIS]
>
>[向智能营销活动添加流程步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

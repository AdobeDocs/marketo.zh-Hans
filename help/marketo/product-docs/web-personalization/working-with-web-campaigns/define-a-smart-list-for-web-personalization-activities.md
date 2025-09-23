---
unique-page-id: 10097867
description: 为Web Personalization活动定义智能列表 — Marketo文档 — 产品文档
title: 为 Web 个性化活动定义智能列表
exl-id: 9987f922-f50c-47b3-aef6-230326b094fc
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 2%

---

# 为[!DNL Web Personalization]活动定义智能列表 {#define-a-smart-list-for-web-personalization-activities}

在智能营销活动中定义智能列表时，您可以在过滤器和触发器中使用[!DNL Web Personalization]活动。 在这里，您要捕获单击[!DNL Web Personalization] call to action （营销活动）的所有人员。

使用触发器发送电子邮件或警报，或根据点击并参与[!DNL Web Personalization] call to action的访客更改值或分数。 您还可以过滤和查看那些单击[!DNL Web Personalization] call to action的潜在客户。

1. 在智能营销活动中，单击&#x200B;**[!UICONTROL Smart List]**&#x200B;选项卡。

   ![](assets/image2016-2-9-10-3a49-3a18.png)

   >[!NOTE]
   >
   >智能列表可以做一些令人惊叹的事情。 在[智能列表深入分析](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)中了解详情。

1. 搜索触发器，然后将触发器拖放到画布上。

   ![](assets/image2016-6-8-9-3a24-3a24.png)

   >[!NOTE]
   >
   >具有触发器的智能营销活动在触发器模式下运行。 它根据触发的事件和添加的过滤器，每次只针对一个人运行。

1. 单击下拉菜单并选择运算符。

   ![](assets/image2016-6-7-11-3a10-3a8.png)

   >[!CAUTION]
   >
   >红色曲线表示错误。 如果未更正，则会使营销活动无效，并且无法运行。

1. 定义触发器。

   ![](assets/image2016-6-7-11-3a12-3a23.png)

1. 根据需要添加过滤器。

   ![](assets/image2016-6-7-11-3a14-3a20.png)

   >[!TIP]
   >
   >在同时具有触发器和过滤器的智能营销活动中，触发器位于顶部。 触发时，只有符合筛选条件的用户才会通过流。

   >[!NOTE]
   >
   >对于多个触发器，如果任何一个触发器被激活，则人员将通过流执行操作。

   若要同时对一组人员运行营销活动，请了解如何[为智能营销活动定义智能列表 | 批次](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)。

   >[!MORELIKETHIS]
   >
   >* [为智能营销活动定义智能列表 | 批次](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [向智能营销活动添加流程步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [为预测性内容活动定义智能列表](/help/marketo/product-docs/predictive-content/define-a-smart-list-for-predictive-content-activities.md)

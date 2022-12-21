---
unique-page-id: 10097873
description: 为预测内容活动定义智能列表 — Marketo文档 — 产品文档
title: 为预测内容活动定义智能列表
exl-id: 2c72b215-8c0b-48b4-8492-8e3fe832fae9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# 为预测内容活动定义智能列表 {#define-a-smart-list-for-predictive-content-activities}

在智能营销活动中定义智能列表时，您可以在触发器和过滤器中使用预测内容活动。 您可以通过 [富媒体模板](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), [内容推荐栏](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)，或 [电子邮件](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md).

1. 在您的智能营销活动中，导航到 **智能列表** 选项卡。

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >智能列表可以做出令人惊叹的事情。 在 [智能列表深深深入](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. 搜索触发器，然后将其拖放到画布上。

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >具有触发器的智能营销活动在触发器模式下运行。 它根据触发的事件和添加的过滤器，一次只在一个人上运行。

1. 单击 **名称** 下拉菜单，然后选择一个运算符。

   ![](assets/smart-list-dropdown-hands.png)

1. 定义触发器。

   ![](assets/smart-lislt-select-content-hands.png)

1. 添加 **类型** 约束。

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. 选择智能列表所需的源。

   ![](assets/pc-add-constraint.png)

1. 如果您使用电子邮件源来提供预测内容，请将 **电子邮件中的点击链接** 触发器。 选择您的电子邮件并添加 **是预测** 约束，定义为 **true**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. 根据需要添加任何其他过滤器。

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >在同时具有触发器和过滤器的智能营销活动中，触发器位于顶部。 触发时，只有满足筛选条件的人员才会浏览流程。

   >[!NOTE]
   >
   >如果激活了任意一个触发器，则人员会通过多个触发器进入流程。

   要同时针对一组人员运行营销活动，请了解如何 [为批量智能营销活动定义智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [为智能营销活动定义智能列表 |批](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [向智能营销活动添加流量步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [为Web个性化活动定义智能列表](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [为Web富媒体启用预测内容](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [启用内容推荐栏](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)


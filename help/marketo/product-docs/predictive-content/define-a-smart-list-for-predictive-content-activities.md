---
unique-page-id: 10097873
description: 为预测内容活动定义智能列表 — Marketo文档 — 产品文档
title: 为预测性内容活动定义智能列表
exl-id: 2c72b215-8c0b-48b4-8492-8e3fe832fae9
feature: Predictive Content
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 5%

---

# 为预测性内容活动定义智能列表 {#define-a-smart-list-for-predictive-content-activities}

在智能营销活动中定义智能列表时，您可以在触发器和过滤器中使用预测内容活动。 您可以为通过[富媒体模板](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)、[内容推荐栏](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)或在[电子邮件](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md)中单击预测内容的任何人触发操作。

1. 在智能营销活动中，导航到&#x200B;**[!UICONTROL Smart List]**&#x200B;选项卡。

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >智能列表可以做一些令人惊叹的事情。 在[智能列表深入分析](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)中了解详情。

1. 搜索触发器，然后将其拖放到画布上。

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >具有触发器的智能营销活动在触发器模式下运行。 它根据触发的事件和添加的过滤器，每次只针对一个人运行。

1. 单击&#x200B;**[!UICONTROL Name]**&#x200B;下拉列表并选择运算符。

   ![](assets/smart-list-dropdown-hands.png)

1. 定义触发器。

   ![](assets/smart-lislt-select-content-hands.png)

1. 添加&#x200B;**[!UICONTROL Type]**&#x200B;约束。

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. 选择智能列表所需的源。

   ![](assets/pc-add-constraint.png)

1. 如果您将电子邮件源用于预测内容，请添加&#x200B;**[!UICONTROL Clicks Link in Email]**&#x200B;触发器。 选择您的电子邮件并添加定义为&#x200B;**[!UICONTROL Is Predictive]**&#x200B;的&#x200B;**[!UICONTROL true]**&#x200B;约束。

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. 根据需要添加任何其他过滤器。

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >在同时具有触发器和过滤器的智能营销活动中，触发器位于顶部。 触发时，只有符合筛选条件的用户才会通过流。

   >[!NOTE]
   >
   >对于多个触发器，如果触发了任意一个触发器，则人员会通过流程进行处理。

   若要对一组人员同时运行该营销活动，了解如何[为批量智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)定义智能列表。

   >[!MORELIKETHIS]
   >
   >* [为智能营销活动定义智能列表 | 批次](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [向智能营销活动添加流程步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [为Web Personalization活动定义智能列表](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [启用Web富媒体的预测内容](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [启用内容推荐栏](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)

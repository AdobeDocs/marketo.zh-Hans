---
unique-page-id: 10097873
description: 为预测内容活动定义智能列表- Marketo Docs — 产品文档
title: 为预测内容列表定义智能活动
translation-type: tm+mt
source-git-commit: f1d7b270454ba41db5197a069e0dcc2caebdec63
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# 为预测内容活动定义智能列表{#define-a-smart-list-for-predictive-content-activities}

在智能活动中定义智能列表时，您可以在触发器和过滤器中使用预测内容活动。 您可以通过[富媒体模板](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)、[内容推荐栏](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)或[电子邮件](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md)为单击预测内容的任何人触发操作。

1. 在您的智能活动中，导航到&#x200B;**智能列表**&#x200B;选项卡。

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >聪明的列表可以做令人惊叹的事情。 在[智能列表深潜](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)中了解更多信息。

1. 搜索触发器，然后将其拖放到画布上。

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >具有触发器的智能活动在触发器模式下运行。 它根据触发的事件和添加的过滤器一次只运行一个人。

1. 单击&#x200B;**名称**&#x200B;下拉框并选择运算符。

   ![](assets/smart-list-dropdown-hands.png)

1. 定义触发器。

   ![](assets/smart-lislt-select-content-hands.png)

1. 添加&#x200B;**Type**&#x200B;约束。

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. 选择您的智能列表所需的源。

   ![](assets/pc-add-constraint.png)

1. 如果您正在使用预测内容的电子邮件源，请添加“电子邮件&#x200B;**中的**&#x200B;点击链接”触发器。 选择您的电子邮件并添加&#x200B;**Is Predictive**&#x200B;约束，定义为&#x200B;**true**。

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. 根据需要添加任何其他过滤器。

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >在具有触发器和过滤器的智能活动中，触发器位于顶部。 触发时，只有符合筛选条件的人才会浏览流程。

   >[!NOTE]
   >
   >如果任何一个触发器被激活，则用户会通过多个触发器进入流程。

   要同时在一组人员上运行活动，请了解如何[为批量智能活动定义智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)。

   >[!MORELIKETHIS]
   >
   >* [为智能列表定义智能活动 |批处理](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [向智能活动添加流步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [为Web个性化列表定义智能活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [为Web富媒体启用预测内容](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [启用内容推荐栏](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)


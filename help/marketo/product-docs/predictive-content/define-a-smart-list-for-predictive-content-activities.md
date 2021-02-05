---
unique-page-id: 10097873
description: 为预测性内容活动定义智能列表- Marketo Docs —— 产品文档
title: 为预测性内容列表定义智能活动
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---


# 为预测内容列表定义智能活动{#define-a-smart-list-for-predictive-content-activities}

>[!NOTE]
>
>根据购买日期，您的营销订阅可能包括Marketo Predictive Content或Content`<sup>AI</sup>`。 对于使用预测内容的用户，Marketo在2018年4月30日之前将启用“内容`<sup>AI</sup>`分析”功能。 要使这些功能在该日期之后保持不变，请联系您的Marketo Customer Success Manager以升级到Marketo Content`<sup>AI</sup>`。

在智能活动中定义智能列表时，您可以在触发器和过滤器中使用预测内容活动。 您可以通过[富媒体模板](enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)、[内容推荐栏](enabling-predictive-content/enable-the-content-recommendation-bar.md)或电子邮件为单击预测内容的任何人触发操作。

1. 在智能活动中，导航至&#x200B;**智能列表**&#x200B;选项卡。

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >**深潜**
   >
   >
   >聪明的列表可以做令人惊叹的事情。 在[智能列表深潜](../../product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)中了解更多信息。

1. 搜索触发器，然后将其拖放到画布上。

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >具有触发器的智能活动在触发器模式下运行。 它根据触发的事件和添加的过滤器，一次只运行一个人。

1. 单击&#x200B;**名称**&#x200B;下拉框并选择运算符。

   ![](assets/smart-list-dropdown-hands.png)

1. 定义触发器。

   ![](assets/smart-lislt-select-content-hands.png)

1. 添加&#x200B;**Type**&#x200B;约束。

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. 选择您需要的智能列表源。

   ![](assets/pc-add-constraint.png)

1. 如果您正在为预测性内容使用电子邮件源，请在电子邮件**触发器中添加**点击链接。 选择您的电子邮件并添加&#x200B;**是预测**&#x200B;约束，定义为&#x200B;**true**。

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. 根据需要添加任何其他过滤器。

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >在具有触发器和过滤器的智能活动中，触发器位于顶部。 触发时，只有满足筛选条件的人才能通过流。

   >[!NOTE]
   >
   >如果任何一个触发器被激活，用户就会通过多个触发器进入流程。

   [为批智能列表定义智能活动](../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)

   >[!MORELIKETHIS]
   >
   >
   >    
   >    
   >    * [为智能列表定义智能活动 |批处理](../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >    * [向智能活动添加流步骤](../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >    * [为Web个性化列表定义智能活动](../../product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >    * [为Web富媒体启用预测内容](enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >    * [启用内容推荐栏](enabling-predictive-content/enable-the-content-recommendation-bar.md)


要同时对一组人员运行活动，请学习如何。
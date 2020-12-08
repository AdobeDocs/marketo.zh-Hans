---
unique-page-id: 1146980
description: 在流程步骤- Marketo Docs —— 产品文档中使用添加选择
title: 在流步骤中使用添加选择
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# 在流步骤中使用添加选择 {#use-add-choice-in-a-flow-step}

>[!NOTE]
>
>**先决条件**
>
>* [向智能活动添加流步骤](add-a-flow-step-to-a-smart-campaign.md)

>



**添加选项** ，可让您在选择详细信息时使用流步骤并说“这取决于”。

1. 在智能 **活动** 的“流”选项卡下，添加任何流步骤，然后单击“添加 **选择”**。

   ![](assets/image2014-9-22-11-3a58-3a20.png)

1. 选择选择条件。

   ![](assets/image2014-9-22-11-3a58-3a50.png)

1. 选择选择运算符并输入选择值。 这将设置您的标准或选择。

   ![](assets/image2014-9-22-11-3a58-3a54.png)

1. 为选择输入流步骤值。

   ![](assets/image2014-9-22-11-3a58-3a57.png)

   >[!CAUTION]
   >
   >令牌在 **选择流** 程步骤的条件部分将无法工作。

1. 重复上述步骤以添加多个选项，然后添加／调整默认值。

   ![](assets/image2014-9-22-11-3a58-3a59.png)

   >[!TIP]
   >
   >您可以将任何流步骤设置为— Do Nothing（不执行任何操作），在这种情况下，不会对该选择执行任何操作。

   >[!CAUTION]
   >
   >流步骤只应用第一匹配选择。 了解如何 [在流动操作中重新排序“添加选择”](reorder-add-choice-in-a-flow-step.md)。

   >[!NOTE]
   >
   >**相关文章**
   >
   >    
   >    
   >    * [在流步骤中重新排序“添加选择”](reorder-add-choice-in-a-flow-step.md)


太好了！ 您现在可以创建包含流程步骤选择的单个智能活动，而不是为每个选择创建多个智能活动。
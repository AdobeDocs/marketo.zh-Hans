---
title: define-a-smart-列表-for-a-batch-活动
description: 为批处理列表定义智能活动
exl-id: 35130f40-cce5-4677-8eaf-f9d73c995ba3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# 为批处理列表定义智能活动

<br> 

智能列表是整个Marketo中定义要包含的“谁”（哪些人）的机制，无论是报表、列表还是智能活动。 下面介绍如何为批处理列表定义智能活动。

1. 选择智能活动，然后单击&#x200B;**[!UICONTROL Smart List]**。

   ![图像1](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-1.png)

1. 键入以搜索筛选器，然后将其拖放到画布。 对多个过滤器重复上述步骤。

   ![图2](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-2.png)

   >[!NOTE]
   >
   >仅具有过滤器的智能活动在批处理模式下运行。 它在数据库中根据过滤器查找符合条件的人员，并同时在流中运行所有这些人员。

   >[!IMPORTANT]
   >
   >您可以通过添加触发器，使智能活动在实时事件的基础上一次在一个人上运行，这会将智能活动置于触发器模式。

1. 单击下拉框并选择滤镜运算符(例如&#x200B;**[!UICONTROL is]**、**[!UICONTROL is not]**&#x200B;等)。

   ![图3](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-3.png)

   >[!CAUTION]
   >
   >红线表示错误或缺少信息。 如果未更正，活动将无效且不运行。

1. 输入筛选值。

   ![图4](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-4.png)

>[!NOTE]
>
>默认情况下，符合所有智能列表规则的人员
>合格。 可以修改此项以满足您的活动需求。 请查阅[复杂逻辑的智能列表规则](https://docs.marketo.com/display/DOCS/Using+Advanced+Smart+List+Rule+Logic)以了解更多信息。
>
>要一次触发实时事件，请了解如何[为智能列表定义智能活动 |触发器](https://docs.marketo.com/display/DOCS/Define+Smart+List+for+Smart+Campaign+%7C+Trigger)。

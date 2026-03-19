---
unique-page-id: 2359500
description: 了解分段顺序优先级以及它如何确定人员属于哪个区段。 编辑数据库中的区段顺序以控制区段的评估。
title: 分段顺序优先级
exl-id: c20d07c8-5e53-4f54-a7a3-2e1aa4fb0cdd
feature: Segmentation
source-git-commit: 80b39eb99cdaacf4c9655aa175da3d22548dcca6
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 4%

---

# 分段顺序优先级 {#segmentation-order-priority}

了解&#x200B;**订单**&#x200B;如何设置分段中人员的评估优先级，这一点很重要。

>[!PREREQUISITES]
>
>[创建分段](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>[定义区段规则](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>您只能在草稿模式下编辑分段。

1. 转到&#x200B;**数据库**。

   ![](assets/segmentation-order-priority-1.png)

1. 选择您的&#x200B;**分段**。 在&#x200B;**[!UICONTROL Segmentation Actions]**&#x200B;中，单击&#x200B;**[!UICONTROL Edit Segments]**。

   ![](assets/segmentation-order-priority-2.png)

   您可以在此屏幕中检查或编辑区段的顺序。

   ![](assets/segmentation-order-priority-3.png)

>[!NOTE]
>
>* 分部之间互相排斥。 人员一次只能是一个区段的成员。
>* 当人员符合两个区段的条件时，他们仅属于列表中的第一个区段。
>* 如果人员不符合任何区段的条件，他们将成为默认区段的成员。

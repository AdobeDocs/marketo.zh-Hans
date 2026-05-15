---
unique-page-id: 2359447
description: 了解如何创建分段以将人员分组以便于报告和动态内容。 在数据库中添加区段，设置顺序，然后定义区段规则。
title: 创建分段
exl-id: a7907f1d-bc78-4b63-9875-044e96609755
feature: Segmentation
TQID: https://experienceleague.adobe.com/Xp4uo4aDMkK9Di3Dp0ufHnxgg8ci7YDD2qOO6rZwI7M
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 238
ht-degree: 5%

---

# 创建分段 {#create-a-segmentation}

分段允许您将人员分组到不同的配置文件中，以便生成报告和动态内容。 下面是创建这些规则的方法。

1. 转到您的&#x200B;**[!UICONTROL Database]**。

   ![](assets/create-a-segmentation-1.png)

1. 单击&#x200B;**[!UICONTROL New]**，然后单击&#x200B;**[!UICONTROL New Segmentation]**。

   ![](assets/create-a-segmentation-2.png)

   >[!TIP]
   >
   >您最多可以创建20个分段。

1. 输入&#x200B;**[!UICONTROL Name]**，单击&#x200B;**[!UICONTROL Add Segment]**&#x200B;并命名它。

   ![](assets/create-a-segmentation-3.png)

   >[!NOTE]
   >
   >默认无法移动、编辑或删除。

1. 添加所需数量的区段（最多100个）。

   ![](assets/create-a-segmentation-4.png)

   >[!CAUTION]
   >
   >可在区段中创建的区段总数，取决于所使用的过滤器的数量和类型，还取决于区段的逻辑复杂程度。 虽然您可以使用标准字段创建最多100个区段，但使用其他类型的过滤器可能会增加复杂性，并且您的区段可能无法批准。 例如：自定义字段、列表成员、潜在客户所有者字段和收入阶段。
   >
   >如果您在审批期间收到错误消息，并且需要帮助来降低分段的复杂性，请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)。

1. 将区段拖放至周围以更改其顺序。 完成后，单击&#x200B;**[!UICONTROL Create]**。

   ![](assets/create-a-segmentation-5.png)

   >[!NOTE]
   >
   >人员将有资格使用所定义的[订单](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md)中的第一个匹配区段。

   >[!NOTE]
   >
   >您需要先定义区段规则，然后才能使用分段。

   恭喜！ 您距离使用动态内容又近了一步。

   >[!MORELIKETHIS]
   >
   >[定义区段规则](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

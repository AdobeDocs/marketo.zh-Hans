---
unique-page-id: 2359457
description: 批准分段 — Marketo文档 — 产品文档
title: 批准分段
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
source-git-commit: b29186ba84ec88be42432e56d1ad0e77c5b43900
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 2%

---

# 批准分段 {#approve-a-segmentation}

区段的使用需要先获得批准。

>[!PREREQUISITES]
>
>* [创建分段](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>* [定义区段规则](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>一次最多可批准20个分段。

1. 转到&#x200B;**[!UICONTROL Database]**。

   ![](assets/approve-a-segmentation-1.png)

1. 在分段中，单击&#x200B;**[!UICONTROL Segmentation Actions]**，然后单击&#x200B;**[!UICONTROL Approve]**。

   ![](assets/approve-a-segmentation-2.png)

   >[!NOTE]
   >
   >审批正在进行时，状态更改为&#x200B;_审批_。

   >[!CAUTION]
   >
   >完成批准可能需要几分钟到一两天的时间，具体取决于数据库的大小。

1. 批准后，[!UICONTROL Status]将从[!UICONTROL Approving]更改为[!UICONTROL Approved]。

   ![](assets/approve-a-segmentation-3.png)

   >[!TIP]
   >
   >每个区段中的人数显示在区段名称旁边的括号中。

1. **[!UICONTROL People]**&#x200B;中的&#x200B;**[!UICONTROL Segment]**&#x200B;选项卡现在显示该区段的最终人员列表。

   ![](assets/approve-a-segmentation-4.png)

>[!CAUTION]
>
>可在区段中创建的区段总数，取决于所使用的过滤器的数量和类型，还取决于区段的逻辑复杂程度。 虽然您可以使用标准字段创建最多100个区段，但使用其他类型的过滤器可能会增加复杂性，并且您的区段可能无法批准。 例如：自定义字段、列表成员、潜在客户所有者字段和收入阶段。
>
>如果您在审批期间收到错误消息，并且需要帮助来降低分段的复杂性，请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)。

>[!MORELIKETHIS]
>
>[在智能列表中使用区段筛选器](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)

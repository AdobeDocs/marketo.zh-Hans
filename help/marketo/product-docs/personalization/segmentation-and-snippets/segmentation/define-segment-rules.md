---
unique-page-id: 2359449
description: 定义区段规则 — Marketo文档 — 产品文档
title: 定义区段规则
exl-id: e6631848-aa8c-4709-b182-4c88abbd365b
source-git-commit: 4699b17a670655820946cd277adf28f2233f04d3
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# 定义区段规则 {#define-segment-rules}

通过定义区段规则，您可以将人员划分为不同的互斥组。

>[!PREREQUISITES]
>
>[创建分段](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. 转到 **数据库。**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. 选择 **分段** 在树中，单击特定 **区段**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. 单击 **智能列表** 和添加过滤器。

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >当前不支持的区段 _过去_ 和 _时间范围_  运算符。 这是因为分段仅在记录更改数据值时检查更新。 这些值包括 _not_ 记录自动更改的内容，如公式字段和日期。 此外，不支持具有相对日期范围的日期运算符，因为它们是在批准分段时计算的，而不是在“更改数据值”活动时计算的。

   >[!NOTE]
   >
   >分段智能列表当前不支持“SFDC类型”和“Microsoft类型”过滤器。

1. 为过滤器填充适当的值。

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!CAUTION]
   >
   >我们建议 _对_ 在定义区段规则时使用“帐户”字段，因为这可能会导致活动日志记录问题。

1. 单击 **人员（草稿）** 选项卡，以查看可能符合此区段成员资格的人员。

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. 转到 **分段操作**. 单击 **批准**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >您在区段中创建的区段总数取决于所使用的过滤器数量和类型，以及区段逻辑的复杂程度。 虽然您可以使用标准字段创建多达100个区段，但使用其他类型的过滤器可能会增加复杂性，并且您的分段可能无法批准。 例如：自定义字段、列表成员、潜在客户所有者字段和收入阶段。
   >
   >如果您在审批期间收到错误消息，并且需要帮助降低分段的复杂性，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support).

1. 请查看功能板，以快速查看饼图中的区段以及应用的规则。

   ![](assets/image2014-9-15-11-3a36-3a19.png)

干得好！ 这些区段在Marketo的很多地方会派上用场。

>[!NOTE]
>
>人员可能有资格访问不同的区段，但最终只属于依赖于 [区段的优先顺序](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md).

>[!NOTE]
>
>“人员（草稿）”屏幕显示符合成员资格且并不总是最终人员列表的所有人员。 批准您的区段以查看最终列表。

>[!MORELIKETHIS]
>
>[批准分段](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)

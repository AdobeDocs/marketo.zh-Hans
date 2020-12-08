---
unique-page-id: 2359449
description: 定义细分规则——营销文档——产品文档
title: 定义区段规则
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---


# 定义区段规则 {#define-segment-rules}

通过定义细分规则，您可以将人员分为不同的互斥组。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>**先决条件**
>
>[创建分段](create-a-segmentation.md)

1. 转到数 **据库。**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. 单击树中的**分段**，然后单击特定的 **段**。

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. 单击“智 **能列表** ”并添加过滤器。

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >目前，区段在过去和 **在时间* 范围内不支持过滤器的运算符。 这是因为分段仅在记录更改数据值时检查更新。 对于自动 *更改* （如公式字段和日期）的项，不记录这些值。 此外，不支持具有相对日期范围的日期运算符，因为它们是在分段批准时计算的，而不是在“更改数据值”活动时计算的。

   >[!NOTE]
   >
   >分段智能过滤器当前不支持“SFDC类型”和“Microsoft类型”列表。

1. 为过滤器填写适当的值。

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!NOTE]
   >
   >**深潜**
   >
   >
   >智能列表太棒了。 了解您可以利用智能 [列表和静态列表做的一切](http://docs.marketo.com/display/docs/smart+lists+and+static+lists)。

1. 单击“人 **员（草稿）** ”选项卡以视图可能符合此区段成员资格的人员。

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. 转到“ **分段操作**”。 单击 **批准**。

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >在细分中可以创建的细分总数取决于所使用的过滤器数和类型，也取决于细分逻辑的复杂程度。 虽然您可以使用标准字段创建多达100个过滤器段，但使用其他类型的细分会增加复杂性，并且您的细分可能无法批准。 例如：自定义字段、列表成员、潜在客户所有者字段和收入阶段。
   >
   >
   >如果您在审批过程中收到错误消息并需要帮助降低分段的复杂性，请与Marketo支持 [部门联系](http://nation.marketo.com/t5/Support/ct-p/Support)。

1. 查看仪表板，快速概览饼图中的区段以及应用的规则。

   ![](assets/image2014-9-15-11-3a36-3a19.png)

干得好！ 这些细分在Marketo的很多地方都会派上用场。

>[!NOTE]
>
>人员可能有资格访问不同的细分，但最终只属于取决于细分 [的优先级顺序的细分](segmentation-order-priority.md)。

>[!NOTE]
>
>**提醒**
>
>“人员（草稿）”屏幕显示所有有资格成为会员的人员，并且并不总是人员的最终列表。 批准您的区段，以查看最终列表。

>[!NOTE]
>
>**相关文章**
>
>* [批准分段](approve-a-segmentation.md)

>




---
unique-page-id: 2359449
description: 定义细分规则——营销文档——产品文档
title: 定义区段规则
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---


# 定义段规则{#define-segment-rules}

通过定义细分规则，您可以将人员分为不同的互斥组。

>[!PREREQUISITES]
>
>[创建分段](create-a-segmentation.md)

1. 转到&#x200B;**数据库。**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. 单击树中的**分段**，然后单击特定&#x200B;**段**。

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. 单击&#x200B;**智能列表**&#x200B;并添加过滤器。

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >区段当前不支持&#x200B;*过去*&#x200B;和*在时间范围内*过滤器的运算符。 这是因为分段仅在记录更改数据值时检查更新。 对于自动更改的项（如公式字段和日期），这些值为&#x200B;*不*&#x200B;记录。 此外，不支持具有相对日期范围的日期运算符，因为它们是在分段批准时计算的，而不是在“更改数据值”活动时计算的。

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
   >智能列表太棒了。 了解您可以使用[智能列表和静态列表](http://docs.marketo.com/display/docs/smart+lists+and+static+lists)执行的所有操作。

1. 单击&#x200B;**人员（草稿）**&#x200B;选项卡，以视图可能符合此区段成员资格的人员。

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. 转到&#x200B;**分段操作**。 单击&#x200B;**批准**。

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >在细分中可以创建的细分总数取决于所使用的过滤器数和类型，也取决于细分逻辑的复杂程度。 虽然您可以使用标准字段创建多达100个过滤器段，但使用其他类型的细分会增加复杂性，并且您的细分可能无法批准。 例如：自定义字段、列表成员、潜在客户所有者字段和收入阶段。
   >
   >
   >如果您在审批过程中收到错误消息并需要帮助降低分段的复杂性，请与[营销人员支持](http://nation.marketo.com/t5/Support/ct-p/Support)联系。

1. 查看仪表板，快速概览饼图中的区段以及应用的规则。

   ![](assets/image2014-9-15-11-3a36-3a19.png)

干得好！ 这些细分在Marketo的很多地方都会派上用场。

>[!NOTE]
>
>人员可能有资格访问不同的区段，但最终只属于取决于区段[优先级顺序的](segmentation-order-priority.md)。

>[!NOTE]
>
>**提醒**
>
>“人员（草稿）”屏幕显示所有有资格成为会员的人员，并且并不总是人员的最终列表。 批准您的区段，以查看最终列表。

>[!MORELIKETHIS]
>
>* [批准分段](approve-a-segmentation.md)

>




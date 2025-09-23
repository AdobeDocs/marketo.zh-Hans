---
unique-page-id: 3571886
description: 使用成功路径分析器 — Marketo文档 — 产品文档
title: 使用成功路径分析器
exl-id: f816b7ac-a158-46bd-9d00-09ef4cc8b381
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 3%

---

# 使用成功路径分析器 {#using-the-success-path-analyzer}

使用成功路径分析器来探索特定详细信息，这些详细信息反映人员在[收入周期模型](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md)的各个阶段中的流量（数量）和速度（速度，以天数为单位）。

>[!PREREQUISITES]
>
>[创建成功路径分析器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/create-a-success-path-analyzer.md)

1. 转到&#x200B;**[!UICONTROL Analytics]**&#x200B;并选择您的&#x200B;**成功路径分析器**。

   ![](assets/image2015-6-12-17-3a23-3a53.png)

   右侧的图表反映了左侧选定按钮中的数据。 默认情况下，这是&#x200B;**[!UICONTROL Balance]**。

1. 单击&#x200B;**[!UICONTROL In Flow]**&#x200B;可绘制在选定时间范围内进入舞台的人数的图表。

   ![](assets/image2015-6-12-17-3a30-3a52.png)

   * 单击&#x200B;**[!UICONTROL Out Flow]**&#x200B;可绘制退出阶段的人数图表。
   * 单击&#x200B;**[!UICONTROL Conv %]**&#x200B;绘制此阶段到下一阶段的转化率图表。
   * 单击&#x200B;**[!UICONTROL Avg Time]**&#x200B;查看人员在此阶段中停留的时间，然后再进入下一个阶段。

1. 单击&#x200B;**[!UICONTROL Chart Actions]** > **[!UICONTROL Compare Period]**&#x200B;将数据与相同长度的其他时间范围进行比较。

   ![](assets/image2015-6-12-17-3a39-3a15.png)

1. 选择比较时段的&#x200B;**[!UICONTROL From]**&#x200B;日期。

   ![](assets/image2015-6-12-17-3a43-3a49.png)

   **[!UICONTROL To]**&#x200B;日期会自动设置为与原始时段的长度匹配。

1. 单击 **[!UICONTROL Compare]**。

   ![](assets/image2015-6-12-17-3a44-3a8.png)

1. 图表以绿色更新比较期间的重叠数据。

   ![](assets/image2015-6-12-17-3a46-3a16.png)

1. 要更改图表的时间范围，请单击&#x200B;**[!UICONTROL Graph by]**&#x200B;按钮之一：每日（默认）、每周和每月

   ![](assets/image2015-6-12-17-3a46-3a55.png)

1. 对于具有SLA（服务级别协议）的阶段，单击&#x200B;**[!UICONTROL Chart Actions]** > **[!UICONTROL Show SLA Due]**&#x200B;可显示指定时间段内每个错过SLA目标的人员。

   ![](assets/image2015-6-12-17-3a49-3a23.png)

1. 图表将进行更新，以反映每个节点上到期的SLA数量（橙色）。

   ![](assets/image2015-6-12-17-3a50-3a16.png)

   以橙色显示的用户可能为&#x200B;*或不是*，但仍处于SLA阶段。

1. 单击&#x200B;**[!UICONTROL Chart Actions]** > **[!UICONTROL Show SLA Past Due]**&#x200B;可显示在指定时间段结束时仍处于SLA阶段的所有已过期SLA目标的人员。

   ![](assets/image2015-6-12-17-3a51-3a39.png)

1. 图表将进行更新，以反映每个节点上过期的SLA数量（橙色）。

   ![](assets/image2015-6-12-17-3a52-3a17.png)

1. 要读取特定节点（日期）上数据点的特定详细信息，请将鼠标悬停在气泡上。

   ![](assets/image2015-6-12-17-3a52-3a49.png)

1. 要打印图表，请单击&#x200B;**[!UICONTROL Chart Actions]** > **[!UICONTROL Print Chart]**。

   ![](assets/image2015-6-12-17-3a53-3a34.png)

分析器可以帮助您了解模型中的移动情况。 随着您的技术不断进步，这对于制定营销策略将变得非常重要。

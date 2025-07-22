---
unique-page-id: 12981145
description: 设置性能分析 — Marketo文档 — 产品文档
title: 设置性能分析
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 2%

---

# 设置[!UICONTROL Performance Insights] {#setting-up-performance-insights}

按照以下步骤设置MPI。

## 机会设置 {#opportunity-setup}

1. 单击 **[!UICONTROL Admin]**。

   ![](assets/admin.png)

1. 单击 **[!UICONTROL Revenue Cycle Analytics]**。

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >如果您没有RCA，则需要为步骤2选择&#x200B;**[!UICONTROL Program Analysis]**。

1. 在归因下，单击&#x200B;**[!UICONTROL Edit]**。

   ![](assets/three-1.png)

1. 此时会显示归因设置。

   ![](assets/four-2.png)

   如果Attribution是明确的，请确保已填充Opportunity Contact Role（通过Opportunity Role端点或通过CRM集成）。

   如果Attribution是隐式的，请确保商机/联系人上的company字段与商机的客户名称相同。

   >[!NOTE]
   >
   >确保所有机会均已填充相应的字段：
   >
   >* [!UICONTROL Opportunity Amount]
   >* [!UICONTROL Is Closed]
   >* [!UICONTROL Is Won]
   >* [!UICONTROL Creation Date] （在您的案例中可能未设置此项）
   >* [!UICONTROL Closed Date] （在您的案例中可能未设置此项）
   >* [!UICONTROL Opportunity Type]

## 项目设置 {#program-setup}

更新计划成本至少12个月。 您可以手动或使用程序API执行此操作。 在本例中，我们手动执行此操作。

1. 单击 **[!UICONTROL Marketing Activities]**。

   ![](assets/ma.png)

1. 查找并选择您的项目。

   ![](assets/select-program.png)

1. 单击&#x200B;**[!UICONTROL Setup]**&#x200B;选项卡。

   ![](assets/setup-tab.png)

1. 将&#x200B;**[!UICONTROL Period Cost]**&#x200B;拖到画布上。

   ![](assets/period-cost.png)

1. 将计划月份设置为至少12个月前，然后单击&#x200B;**[!UICONTROL Ok]**。

   ![](assets/set-period.png)

1. 设置期间成本并单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/set-cost.png)

接下来，查看Analytics行为，以指示分析中是否应包含特定渠道。 设置Analytics行为（正常、包含、可操作）。

1. 单击 **[!UICONTROL Admin]**。

   ![](assets/admin.png)

1. 单击 **[!UICONTROL Tags]**。

   ![](assets/tags.png)

1. 单击&#x200B;**+**&#x200B;以展开渠道列表。

   ![](assets/channel.png)

1. 双击所需的渠道。

   ![](assets/channel-click.png)

1. 单击&#x200B;**[!UICONTROL Analytics Behavior]**&#x200B;下拉列表并选择所需的行为。

   ![](assets/edit-channel.png)

1. 设置成功标准。

   ![](assets/success.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/save.png)

## 将项目与人员关联 {#tie-the-program-to-the-person}

1. 确保已为数据库中的每个人设置客户获取计划和客户获取日期，以便首次联系归因正常工作。
1. 确保您的项目为人员设置成功状态。

>[!NOTE]
>
>所做的更改不是立即进行的。 在更改生效之前，需要过一夜的时间。

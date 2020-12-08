---
unique-page-id: 12981145
description: 设置性能分析——营销文档——产品文档
title: 设置性能分析
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# 设置性能分析 {#setting-up-performance-insights}

请按照以下步骤设置MPI。

## 业务机会设置 {#opportunity-setup}

1. 单击 **管理**。

   ![](assets/admin.png)

1. 单击 **收入周期分析**。

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >如果您没有RCA，您需要为步骤2选 **择项目** 分析。

1. 在归因下，单击 **编辑**。

   ![](assets/three-1.png)

1. 此时会显示归因设置。

   ![](assets/four-2.png)

   如果Attribution是明确的，请确保已填充Opportunity Contact Role（通过Opportunity Role端点或通过CRM集成）。

   如果“归因”是隐式的，请确保潜在客户／联系人上的公司字段与业务机会的帐户名称相同。

   >[!NOTE]
   >
   >确保所有机会都填充了相应的字段：
   >
   >    
   >    
   >    * 机会金额
   >    * 已关闭
   >    * 是赢
   >    * 创建日期（在您的情况下可能未设置）
   >    * 结束日期（在您的情况下可能未设置）
   >    * 机会类型


## 项目设置 {#program-setup}

将项目成本更新至少12个月。 您可以手动或使用项目API执行此操作。 在本例中，我们手动执行此操作。

1. 单击 **营销活动**。

   ![](assets/ma.png)

1. 查找并选择您的项目。

   ![](assets/select-program.png)

1. 单击“设 **置** ”选项卡。

   ![](assets/setup-tab.png)

1. 将 **期间成本** 拖动到画布上。

   ![](assets/period-cost.png)

1. 将项目月设置为至少12个月前，然后单击“确 **定”**。

   ![](assets/set-period.png)

1. 设置期间成本，然后单击“ **保存**”。

   ![](assets/set-cost.png)

接下来，检查分析行为以指示是否应将特定渠道包含在分析中。 设置分析行为（正常、包含、操作）。

1. 单击 **管理**。

   ![](assets/admin.png)

1. 单击“ **标记**”。

   ![](assets/tags.png)

1. 单击 **+** 以展开渠道列表。

   ![](assets/channel.png)

1. 多次-单击所需的渠道。

   ![](assets/channel-click.png)

1. 单击“ **分析行为** ”下拉框，然后选择所需的行为。

   ![](assets/edit-channel.png)

1. 设置成功标准。

   ![](assets/success.png)

1. 单击 **保存**。

   ![](assets/save.png)

## 将项目与人关联 {#tie-the-program-to-the-person}

1. 确保为数据库中的每个人设置了“客户获取项目”和“客户获取日期”，以便“首次联系归因”正常工作。
1. 确保您的项目为您的员工设置成功状态。

>[!NOTE]
>
>所做的更改并非即时的。 更改生效前需要隔夜时间。


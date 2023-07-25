---
unique-page-id: 12981145
description: 设置性能分析 — Marketo文档 — 产品文档
title: 设置性能分析
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# 设置性能分析 {#setting-up-performance-insights}

按照以下步骤设置MPI。

## 机会设置 {#opportunity-setup}

1. 单击 **管理员**.

   ![](assets/admin.png)

1. 单击 **收入周期分析**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >如果您没有RCA，则需要选择 **项目分析** 步骤2.

1. 在归因下，单击 **编辑**.

   ![](assets/three-1.png)

1. “归因设置”随即显示。

   ![](assets/four-2.png)

   如果Attribution是明确的，请确保已填充机会联系人角色（通过机会角色端点或通过CRM集成）。

   如果Attribution是隐式的，请确保潜在客户/联系人上的company字段与机会的客户名称相同。

   >[!NOTE]
   >
   >确保所有机会都已填充了相应的字段：
   >
   >* 机会金额
   >* 已关闭
   >* 赢得了
   >* 创建日期（在您的案例中可能未设置此日期）
   >* 关闭日期（在您的案例中可能未设置此日期）
   >* 机会类型

## 项目设置 {#program-setup}

更新计划成本至少12个月。 您可以手动或使用程序API执行此操作。 在本例中，我们手动执行此操作。

1. 单击 **营销活动**.

   ![](assets/ma.png)

1. 查找并选择您的项目。

   ![](assets/select-program.png)

1. 单击 **设置** 选项卡。

   ![](assets/setup-tab.png)

1. 拖动 **期间成本** 到画布上。

   ![](assets/period-cost.png)

1. 将计划月设置为至少12个月前，然后单击 **确定**.

   ![](assets/set-period.png)

1. 设置期间成本并单击 **保存**.

   ![](assets/set-cost.png)

接下来，查看Analytics行为，以指示是否应在Analytics中包含特定渠道。 设置Analytics行为（正常、包含、可操作）。

1. 单击 **管理员**.

   ![](assets/admin.png)

1. 单击 **标记**.

   ![](assets/tags.png)

1. 单击 **+** 以展开“渠道”列表。

   ![](assets/channel.png)

1. 双击所需的渠道。

   ![](assets/channel-click.png)

1. 单击 **Analytics行为** 下拉列表并选择所需的行为。

   ![](assets/edit-channel.png)

1. 设置成功标准。

   ![](assets/success.png)

1. 单击 **保存**.

   ![](assets/save.png)

## 将项目与人员关联 {#tie-the-program-to-the-person}

1. 确保已为数据库中的每个人设置客户获取计划和客户获取日期，以便首次联系归因正常工作。
1. 确保您的项目为人员设置成功状态。

>[!NOTE]
>
>所做的更改不是立即进行的。 在更改生效之前，需要过夜时间。

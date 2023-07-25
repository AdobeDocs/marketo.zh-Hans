---
unique-page-id: 557322
description: 从智能列表运行单流程步骤 — Marketo文档 — 产品文档
title: 从智能列表中运行单个流程步骤
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 1%

---

# 从智能列表中运行单个流程步骤 {#run-a-single-flow-step-from-a-smart-list}

如果要运行一次性的仅流程步骤，则可以在智能列表中使用单个流程步骤，而不是创建整个智能营销活动。

>[!PREREQUISITES]
>
>[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-1.png)

1. 选择一个列表或包含人员的智能列表，然后转到 **人员** 选项卡。

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >静态列表和智能列表都具有此功能。

1. 单击 **全选**. 您还可以使用 **Ctrl/Cmd** 并点击以手动选择一些记录。

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >如果结果跨多个页面，请单击 **全选** 将选择所有页面中的所有人员。

1. 下 **人员** **操作**，选择您选择的流程步骤。 在此示例中，我们将使用 [更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

   ![](assets/personactions-hands.png)

1. 查找并选择 **属性**. 在此示例中，我们将接受所有拥有州“加利福尼亚”的人，并将其更改为“CA”。

   ![](assets/runaction-hands.png)

1. 输入一个新值. 单击 **立即运行**.

   ![](assets/runactionnewvalue-hands.png)

1. 如果要更改大量人员的数据值，您可能需要通过键入数字来确认更改。 单击 **大胆试试**.

   ![](assets/changedatavalue.jpg)

做得很棒！ 您将在右上角看到单流程步骤的状态。

![](assets/completesingleflowaction.jpg)

完成后，刷新列表，您将看到更新的信息。

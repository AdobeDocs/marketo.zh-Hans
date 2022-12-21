---
unique-page-id: 557322
description: 从智能列表 — Marketo文档 — 产品文档中运行单一流程步骤
title: 从智能列表中运行单个流步骤
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 1%

---

# 从智能列表中运行单个流步骤 {#run-a-single-flow-step-from-a-smart-list}

如果要运行仅一次性流量步骤，则可以在智能列表中使用单个流量步骤，而不是创建整个智能营销活动。

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

1. 单击 **全选**. 您还可以使用 **Ctrl/Cmd** 并单击以手动选择一些记录。

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >如果结果跨越多个页面，请单击 **全选** 将选择所有页面中的所有人员。

1. 在 **人员** **操作**，选择所选的流程步骤。 在本例中，我们将使用 [更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

   ![](assets/personactions-hands.png)

1. 查找并选择 **属性**. 在此示例中，我们会将所有拥有州“California”的人员更改为“CA”。

   ![](assets/runaction-hands.png)

1. 输入一个新值. 单击 **立即运行**.

   ![](assets/runactionnewvalue-hands.png)

1. 如果您正在更改大量人员的数据值，则可能需要键入数字以确认更改。 单击 **Go It**.

   ![](assets/changedatavalue.jpg)

太棒了！ 您将在右上角看到单个流程步骤的状态。

![](assets/completesingleflowaction.jpg)

完成后，刷新列表，您将看到更新的信息。

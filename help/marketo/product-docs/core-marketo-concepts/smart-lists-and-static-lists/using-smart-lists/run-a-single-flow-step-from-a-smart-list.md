---
unique-page-id: 557322
description: 从智能列表- Marketo文档 — 产品文档运行单流程步骤
title: 从智能列表运行单流步骤
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# 从智能列表{#run-a-single-flow-step-from-a-smart-list}运行单流步骤

如果要运行仅一次的流步骤，您可以在智能列表中使用单个流步骤，而不是创建整个智能活动。

>[!PREREQUISITES]
>
>[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 转至&#x200B;**营销活动**。

   ![](assets/login-marketing-activities-1.png)

1. 选择包含人员的列表或智能列表，然后转到&#x200B;**人员**&#x200B;选项卡。

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >静态列表和智能列表都具有此功能。

1. 单击&#x200B;**选择全部**。 您还可以使用&#x200B;**Ctrl/Cmd**&#x200B;并单击手动选择一些记录。

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >如果结果跨多个页面，则单击&#x200B;**全选**&#x200B;将选择所有页面中的所有人。

1. 在&#x200B;**Person** **Actions**&#x200B;下，选择您选择的流步骤。 在此示例中，我们将使用[更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)。

   ![](assets/personactions-hands.png)

1. 查找并选择&#x200B;**属性**。 在此示例中，我们将将所有拥有州“California”并将其更改为“CA”的人。

   ![](assets/runaction-hands.png)

1. 输入新值。 单击&#x200B;**立即运行**。

   ![](assets/runactionnewvalue-hands.png)

1. 如果您正在更改大量人员的数据值，您可能需要通过键入数字来确认更改。 单击&#x200B;**“Go For It**”。

   ![](assets/changedatavalue.jpg)

太棒了！ 您将在右上角看到单个流步骤的状态。

![](assets/completesingleflowaction.jpg)

完成后，刷新列表，您将看到更新的信息。

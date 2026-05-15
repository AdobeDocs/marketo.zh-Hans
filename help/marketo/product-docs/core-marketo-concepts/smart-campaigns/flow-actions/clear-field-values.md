---
unique-page-id: 1147324
description: 了解如何在Smart Campaign流程步骤中清除字段值。 从人员或公司字段中移除值。
title: 清除字段值
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/57QZb7T-y2JVdNeP4nhTl9PDjIX1S9GcQmRAMJ-53E0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 103
ht-degree: 5%

---

# 清除字段值 {#clear-field-values}

[更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)很好，但如何&#x200B;_完全删除_&#x200B;该值？ 问得好！

1. 在流程步骤中，选择要清除的字段并键入&#x200B;**[!UICONTROL NULL]**（全部大写）作为&#x200B;**[!UICONTROL New Value]**。

   ![](assets/clear-field-values-1.png)

1. 完成流程步骤后，将清除所选字段的值。

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >将新值留空或输入SPACE不会真正清空字段。 必须键入NULL。 此外，请记住，流程步骤在运行后无法撤消。

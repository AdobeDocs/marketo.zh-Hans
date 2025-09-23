---
unique-page-id: 1147324
description: 清除字段值 — Marketo文档 — 产品文档
title: 清除字段值
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '92'
ht-degree: 6%

---

# 清除字段值 {#clear-field-values}

[更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)很好，但如何&#x200B;_完全删除_&#x200B;该值？ 问得好！

1. 在流程步骤中，选择要清除的字段并键入&#x200B;**[!UICONTROL NULL]**（全部大写）作为&#x200B;**[!UICONTROL New Value]**。

   ![](assets/clear-field-values-1.png)

1. 完成流程步骤后，将清除所选字段的值。

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >将新值留空或仅输入SPACE不会真正清空字段。 必须键入NULL。 此外，请记住，运行后无法撤消流程步骤。

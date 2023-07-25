---
unique-page-id: 1147324
description: 清除字段值 — Marketo文档 — 产品文档
title: 清除字段值
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# 清除字段值 {#clear-field-values}

[更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) 很好，但是你怎么 _移除_ 值是否完全相同？ 好问题！

1. 在流程步骤中，选择要清除的字段并键入 **空** （全部大写）作为 **新值**.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. 砰！ 我打赌你不知道！ 完成流程步骤后，将清除所选字段的值。

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >将新值留空或仅输入空格不会真正清空字段。 必须键入NULL。 此外，请记住，流程步骤在运行后无法撤消。

---
unique-page-id: 1147324
description: 清除字段值- Marketo Docs —— 产品文档
title: 清除字段值
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# 清除字段值{#clear-field-values}

[更改数](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) 据值很好，但如何完 __ 全删除该值？问得好！

1. 在流步骤中，选择要清除的字段，并键入&#x200B;**NULL**（所有大写）作为&#x200B;**新值**。

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. 砰！ 我打赌你不知道！ 流步骤完成后，将清除所选字段的值。

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >将新值留空或仅输入空格不会真正清空字段。 必须键入NULL。 另外，请记住，流步骤在运行后无法撤消。

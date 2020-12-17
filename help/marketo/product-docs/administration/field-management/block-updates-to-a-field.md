---
unique-page-id: 2360291
description: 阻止对字段的更新- Marketo Docs —— 产品文档
title: 阻止对字段的更新
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---


# 阻止对字段{#block-updates-to-a-field}的更新

阻止对字段的更新允许您向字段写入一次，然后在字段的生命周期中保留原始值。 这对“人员来源”等字段很有用。

>[!NOTE]
>
>**需要管理员权限**

1. 转至&#x200B;**Admin**&#x200B;并单击&#x200B;**字段管理**。

   ![](assets/image2014-9-24-13-3a54-3a40.png)

1. 找到该字段，选择它，然后在&#x200B;**字段操作**&#x200B;下，单击&#x200B;**块字段更新**。

   ![](assets/two-1.png)

1. 选择要阻止的&#x200B;**输入源**&#x200B;并单击&#x200B;**应用**。

   ![](assets/image2014-9-24-13-3a55-3a16.png)

   >[!CAUTION]
   >
   >执行列表导入时，只有在Marketo根据与&#x200B;**完全匹配**&#x200B;的字段名称（或如果已建立别名）自动识别字段时，才会显示“导入”预览中被阻止的字段的状态。 如果从“市场营销人员字段”下拉列表中手动选择字段，则“导入”预览中不会显示阻止状态，但仍将实现对该字段的更新阻止。


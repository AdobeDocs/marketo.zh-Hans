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


# 阻止对字段的更新 {#block-updates-to-a-field}

阻止对字段的更新允许您向字段写入一次，然后在字段的生命周期中保留原始值。 这对“人员来源”等字段很有用。

>[!NOTE]
>
>**需要管理员权限**

1. 转到“管 **理员** ”并单 **击“字段管理**”。

   ![](assets/image2014-9-24-13-3a54-3a40.png)

1. 找到该字段，选择它，然后在“字 **段操作”下**，单 **击“阻止字段更新”**。

   ![](assets/two-1.png)

1. 选择要 **阻止的** “输入源”，然后单 **击应用**。

   ![](assets/image2014-9-24-13-3a55-3a16.png)

   >[!CAUTION]
   >
   >执行列表导入时，只有在Market根据完全匹配的字段名称（或已建立别名）自动识别字段时，“导入”预览中被阻止的字段的状态才 **会显** 示出来。 如果从“市场营销人员字段”下拉列表中手动选择字段，则“导入”预览中不会显示阻止状态，但仍将实现对该字段的更新阻止。


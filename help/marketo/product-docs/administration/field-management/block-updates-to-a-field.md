---
unique-page-id: 2360291
description: 字段的块更新 — Marketo文档 — 产品文档
title: 阻止字段更新
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# 阻止字段更新 {#block-updates-to-a-field}

阻止对字段进行更新，即允许您向字段写入一次，然后在字段的生命周期内保留原始值。 这对于“人员来源”之类的字段非常有用。

>[!NOTE]
>
>**需要管理员权限**

1. 转到 **管理员** 的上界。

   ![](assets/block-updates-to-a-field-1.png)

1. 单击 **字段管理**.

   ![](assets/block-updates-to-a-field-2.png)

1. 查找字段，将其选中，然后在 **字段操作**，单击 **块字段更新**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >您可以阻止 [程序成员自定义字段](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) 也是。

1. 选择 **输入源** 要阻止并单击 **应用**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >执行列表导入时，只有在Marketo根据字段匹配的名称自动识别字段时，“导入预览”中被阻止的字段的状态才会显示 _完全_ （或者，如果已建立别名）。 如果从“Marketo字段”下拉列表中手动选择字段，则“导入预览”中不会显示阻止的状态，但仍会实施对该字段的更新阻止。

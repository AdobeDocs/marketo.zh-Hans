---
unique-page-id: 2360291
description: 阻止更新字段 — Marketo文档 — 产品文档
title: 阻止更新字段
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# 阻止更新字段 {#block-updates-to-a-field}

阻止字段更新允许您写入字段一次，然后保留字段生命周期的原始值。 这对于之类的字段可能很有用 [!UICONTROL 人员来源].

>[!NOTE]
>
>**需要管理员权限**

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/block-updates-to-a-field-1.png)

1. 单击 **[!UICONTROL 字段管理]**.

   ![](assets/block-updates-to-a-field-2.png)

1. 找到该字段，选择它，然后在 **[!UICONTROL 字段操作]**，单击 **[!UICONTROL 阻止字段更新]**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >您可以阻止对的更新 [项目群成员自定义字段](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) 也一样。

1. 选择 **[!UICONTROL 输入源]** 要阻止并单击 **[!UICONTROL 应用]**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >执行列表导入时，导入预览中阻止的字段的状态仅在Marketo根据字段匹配的名称自动识别该字段时显示 _完全匹配_ （或者如果建立了别名）。 如果从Marketo字段下拉列表中手动选择字段，则导入预览中将不会显示阻止的状态，但仍会对该字段实施更新阻止。

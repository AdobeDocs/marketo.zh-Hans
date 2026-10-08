---
unique-page-id: 2360291
description: 阻止对字段的更新，以便在记录的生命周期内保留写入的第一个值。
title: 阻止字段更新
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
TQID: 'https://experienceleague.adobe.com/XHwNOU3s7CWDUp21LaxOTo--NA1nYZvCL7G4y5AjUFg'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: f5e85a9b-a883-40d0-8759-f3651efb32e9
    internal-label: Field management
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 10%
---
# 阻止字段更新 {#block-updates-to-a-field}

阻止字段更新允许您写入字段一次，然后保留记录生命周期的原始值。 这对于诸如[!UICONTROL Person Source]之类的字段可能很有用。

>[!NOTE]
>
>**需要管理员权限**

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/block-updates-to-a-field-1.png)

1. 单击 **[!UICONTROL Field Management]**。

   ![](assets/block-updates-to-a-field-2.png)

1. 找到该字段并选择它，然后在&#x200B;**[!UICONTROL Field Actions]**&#x200B;下单击&#x200B;**[!UICONTROL Block Field Updates]**。

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >您也可以阻止对[项目成员自定义字段](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)的更新。

1. 选择要阻止的&#x200B;**[!UICONTROL Input Sources]**&#x200B;并单击&#x200B;**[!UICONTROL Apply]**。

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >执行列表导入时，仅当字段的名称与&#x200B;_完全_&#x200B;匹配时（或如果已建立别名），Marketo自动识别该字段时，导入预览中阻止的字段的状态才会显示。 如果从Marketo字段下拉列表中手动选择字段，则导入预览中将不会显示阻止的状态，但仍会对该字段实施更新阻止。

---
unique-page-id: 2360287
description: 在Marketo中创建自定义字段 — Marketo文档 — 产品文档
title: 在Marketo中创建自定义字段
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 在Marketo中创建自定义字段 {#create-a-custom-field-in-marketo}

如果您在Marketo Engage中需要新的自定义字段来存储/捕获数据，以下是如何创建一个。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/create-a-custom-field-in-marketo-1.png)

1. 单击 **[!UICONTROL 字段管理]**.

   ![](assets/create-a-custom-field-in-marketo-2.png)

   >[!TIP]
   >
   >如果您希望字段与CRM保持同步，请在CRM中创建它们，并且这些字段将在Marketo中自动创建。

1. 单击 **[!UICONTROL 新建自定义字段]**.

   ![](assets/create-a-custom-field-in-marketo-3.png)

1. 选择字段类型。 这将更改它在Marketo的智能列表和表单中的呈现方式。

   >[!TIP]
   >
   >查看 [自定义字段类型术语表](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md).

   ![](assets/create-a-custom-field-in-marketo-4.png)

1. 输入 [!UICONTROL 名称] 您希望它在Marketo中显示的方式。 此 [!UICONTROL API名称] 是自动生成的。 您可以对其进行调整，但设置后无法重命名它。 单击 **[!UICONTROL 创建]** 完成时。

>[!CAUTION]
>
>字段名称不能以下列字符开头： **.&amp; +[]**

![](assets/create-a-custom-field-in-marketo-5.png)

>[!NOTE]
>
>API名称由SOAP API和其他后端进程使用。

现在，您可以在表单、流程步骤和智能列表中使用此自定义字段！

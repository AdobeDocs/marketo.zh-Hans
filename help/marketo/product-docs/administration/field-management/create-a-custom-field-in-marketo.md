---
unique-page-id: 2360287
description: 在Marketo Engage中创建新自定义字段以存储和捕获人员或公司数据的步骤。
title: 在 Marketo 中创建自定义字段
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
feature: Field Management
TQID: https://experienceleague.adobe.com/xdG07VzIcNYcqCsR3wfXHTGE07nsLYAvbM8QZZJf0oo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 191
ht-degree: 14%

---

# 在 Marketo 中创建自定义字段 {#create-a-custom-field-in-marketo}

了解如何在Marketo Engage中创建自定义字段以存储和捕获数据。

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/create-a-custom-field-in-marketo-1.png)

1. 单击 **[!UICONTROL Field Management]**。

   ![](assets/create-a-custom-field-in-marketo-2.png)

   >[!TIP]
   >
   >如果您希望字段与CRM保持同步，请在CRM中创建它们，并且这些字段将在Marketo中自动创建。

1. 单击 **[!UICONTROL New Custom Field]**。

   ![](assets/create-a-custom-field-in-marketo-3.png)

1. 选择&#x200B;_[!UICONTROL Object]_。

   ![](assets/create-a-custom-field-in-marketo-4.png)

   >[!NOTE]
   >
   >虽然您无法自行选择&#x200B;_公司_&#x200B;对象，但可以通过联系[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}来请求它。

1. 选择字段&#x200B;_[!UICONTROL Type]_。 这将更改它在Marketo的智能列表和表单中的呈现方式。

   >[!TIP]
   >
   >查看[自定义字段类型术语表](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}。

   ![](assets/create-a-custom-field-in-marketo-5.png)

1. 输入您希望它在Marketo中显示的&#x200B;_[!UICONTROL Name]_（自动生成&#x200B;_[!UICONTROL API Name]_）。 请仔细选择，因为保存后无法重命名它。 完成后，单击 **[!UICONTROL Create]**。

>[!CAUTION]
>
>字段名称不能以下列字符开头： **。 &amp; +[]**

![](assets/create-a-custom-field-in-marketo-6.png)

>[!NOTE]
>
>该API名称由SOAP API和其他后端进程使用。

现在，您可以在表单、流程步骤和智能列表中使用此自定义字段。

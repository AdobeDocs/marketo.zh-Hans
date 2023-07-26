---
unique-page-id: 2949962
description: 动态切换表单字段的可见性 — Marketo文档 — 产品文档
title: 动态切换表单字段的可见性
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# 动态切换表单字段的可见性 {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [在表单中添加国家/地区选择列表](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

Marketo表单的一个真正酷的功能是，您可以动态隐藏/显示表单字段或 [字段集](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**示例**
>
>在此示例中，让我们隐藏 **状态** 字段unless **国家/地区** 选为“美国”。

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-8.png)

1. 选择您的表单并单击 **编辑表单**.

   ![](assets/editform-1.png)

1. 选择要动态隐藏/显示的字段，然后单击链接 **可见性规则**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. 查找并选择要在其周围构建条件的字段。

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. 选择运算符。

   >[!TIP]
   >
   >这很酷，因为您可以选择模糊匹配，如“starts with”。

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. 选择要查找的值，然后单击下拉列表外部的。

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >您可以在下拉列表打开时单击多个值来选择它们。 例如，您可以选择“美国”和“加拿大”。

   >[!NOTE]
   >
   >我们之前已将国家/地区转换为领料单字段类型，并且 [已将所有国家/地区添加为值](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. 单击 **保存**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

就是这样！ 现在，当人们填写此表单并选择“美国国家/地区”时，“州”字段将动态显示指定的选项。

>[!IMPORTANT]
>
>通过使用自定义脚本设置/更新字段值时，表单字段行为将无缝工作 [API函数](https://developers.marketo.com/javascript-api/forms/){target="_blank"} 在Forms 2.0中。
>
>如果字段值由Forms 2.0 JavaScript API以外的外部脚本修改，则条件字段可能无法按预期工作。

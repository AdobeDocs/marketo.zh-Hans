---
unique-page-id: 2949962
description: 动态切换表单字段的可见性 — Marketo文档 — 产品文档
title: 动态切换表单字段的可见性
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 动态切换表单字段的可见性 {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [将国家/地区选取列表添加到表单](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)


Marketo表单的一个非常酷的功能是，您可以动态隐藏/显示表单字段或 [字段集](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**示例**
>
>在本例中，我们将隐藏 **州** 除外 **国家/地区** 被选为“美国”。

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-8.png)

1. 选择您的表单并单击 **编辑表单**.

   ![](assets/editform-1.png)

1. 选择要动态隐藏/显示的字段，然后单击 **可见性规则**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. 查找并选择要围绕此字段构建条件。

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. 选择运算符。

   >[!TIP]
   >
   >这很酷，因为您可以选择模糊匹配，如“开头为”。

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. 选择要查找的值，然后单击下拉列表外的。

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >在下拉列表打开时，您可以单击以选择多个值。 例如，您可以选择美国和加拿大。

   >[!NOTE]
   >
   >我们以前将“国家/地区”转换为挑库列表字段类型， [将所有国家/地区作为值添加](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. 单击 **保存**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

就这样！ 现在，当用户填写此表并选择“美国为国家”时，“状态”字段将动态显示并提供指定的选项。

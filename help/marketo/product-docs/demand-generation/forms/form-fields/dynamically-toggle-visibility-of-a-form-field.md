---
unique-page-id: 2949962
description: 动态切换表单字段的可见性- Marketo Docs —— 产品文档
title: 动态切换表单字段的可见性
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# 动态切换表单字段{#dynamically-toggle-visibility-of-a-form-field}的可见性

>[!PREREQUISITES]
>
>* [将国家／地区选择列表添加到表单](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)


Marketo表单最酷的一个功能是您可以动态隐藏／显示表单字段或[字段集](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md)。

>[!NOTE]
>
>**示例**
>
>在此示例中，让我们隐藏&#x200B;**State**&#x200B;字段，除非将&#x200B;**Country**&#x200B;选为“United States”。

1. 转到&#x200B;**营销活动**。

   ![](assets/login-marketing-activities-8.png)

1. 选择表单，然后单击&#x200B;**编辑表单**。

   ![](assets/editform-1.png)

1. 选择要动态隐藏／显示的字段，然后单击&#x200B;**可见性规则**&#x200B;的链接。

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. 查找并选择要围绕其构建条件的字段。

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. 选择运算符。

   >[!TIP]
   >
   >这很酷，因为您可以选择模糊匹配，如“开始与”。

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. 选择要查找的值，然后在下拉框外单击。

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >在下拉框打开时，您可以通过单击来选择多个值。 例如，您可以选择“美国和加拿大”。

   >[!NOTE]
   >
   >我们以前将“国家／地区”转换为挑库列表字段类型，并且[将所有国家／地区添加为值](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)。

1. 单击&#x200B;**保存**。

   ![](assets/image2014-9-15-15-3a18-3a15.png)

就这样！ 现在，当用户填写此表单并选择“国家／地区为美国”时，“州”字段将动态显示指定的选项。

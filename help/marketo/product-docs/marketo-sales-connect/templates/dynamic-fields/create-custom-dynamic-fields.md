---
unique-page-id: 14352508
description: 创建自定义动态字段 — Marketo文档 — 产品文档
title: 创建自定义动态字段
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# 创建自定义动态字段 {#create-custom-dynamic-fields}

有两种方法可创建自定义动态字段。

## 保存一个或多个联系人的自定义字段 {#saving-custom-fields-for-one-or-a-few-contacts}

1. 在“人员”页面中单击联系人的姓名。

1. 选择取消订阅旁边的下拉列表，然后选择 **编辑**.

1. 向下滚动到编辑页面的底部。 然后，您可以为字段创建名称和值。

1. 单击 **保存**.

## 保存许多联系人的自定义字段 {#saving-custom-fields-for-many-contacts}

1. 创建一个CSV电子表格，其中包含您的自定义字段。

1. 关注 [正常的CSV上传过程](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)，在字段映射屏幕上停止。

1. 选择“预设”字段，而不是“预设”字段 **添加新的自定义字段** 从下拉菜单中。

1. 输入所需的字段名称，然后单击 **确定**.

1. 完成CSV上传。 您的联系人将通过添加的自定义字段。

>[!NOTE]
>
>创建自定义字段后，该字段可能需要大约30分钟才能显示在模板编辑器的动态字段下拉菜单中。

## 如何在模板中使用自定义字段 {#how-to-use-your-custom-fields-in-a-template}

使用上述方法存储自定义字段后，您便可以在模板中引用它们。

1. [创建模板](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) ，然后单击 **动态字段** 按钮。

1. 选择 **自定义字段** 从显示的下拉菜单中。

1. 您将看到预存储的自定义字段，并能够选择一个来填写模板。

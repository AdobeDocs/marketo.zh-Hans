---
unique-page-id: 14352508
description: 创建自定义动态字段 — Marketo文档 — 产品文档
title: 创建自定义动态字段
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# 创建自定义动态字段 {#create-custom-dynamic-fields}

创建自定义动态字段的方法有两种。

## 保存一个或多个联系人的自定义字段 {#saving-custom-fields-for-one-or-a-few-contacts}

1. 在人员页面中单击联系人的姓名。

1. 选择“Unsubscribe（取消订阅）”旁边的下拉菜单并选择 **编辑**.

1. 向下滚动到编辑页面的底部。 然后，您可以为字段创建名称和值。

1. 单击 **保存**.

## 正在保存多个联系人的自定义字段 {#saving-custom-fields-for-many-contacts}

1. 创建一个CSV电子表格，将您的自定义字段放置在其自己的列中。

1. 请遵循 [常规CSV上传过程](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)，在字段映射屏幕上停止。

1. 请选择而不是预设字段之一 **添加新自定义字段** 从下拉菜单中查找。

1. 输入所需的字段名称，然后单击 **确定**.

1. 完成CSV上传。 您的联系人将通过添加的自定义字段进行访问。

>[!NOTE]
>
>创建自定义字段后，大约需要30分钟该字段才会显示在模板编辑器的动态字段下拉列表中。

## 如何在模板中使用自定义字段 {#how-to-use-your-custom-fields-in-a-template}

使用上述方法存储自定义字段后，您就可以在模板中引用它们。

1. [创建模板](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) 然后单击 **动态字段** 你平常的样子。

1. 选择 **自定义字段** 从出现的下拉菜单中单击。

1. 您将看到预存储的自定义字段，并可以选择其中一个字段来填写模板。

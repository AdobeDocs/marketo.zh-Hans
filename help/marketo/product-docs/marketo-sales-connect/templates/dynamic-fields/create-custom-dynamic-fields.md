---
unique-page-id: 14352508
description: 创建自定义动态字段- Marketo Docs —— 产品文档
title: 创建自定义动态字段
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# 创建自定义动态字段 {#create-custom-dynamic-fields}

有两种方法可创建自定义动态字段。

## 保存一个或多个联系人的自定义字段 {#saving-custom-fields-for-one-or-a-few-contacts}

1. 在“人员”页面中单击联系人的姓名。
1. 选择“取消订阅”旁边的下拉框，然后选择“ **编辑**”。
1. 向下滚动到编辑页面的底部。 然后，您可以为字段创建名称和值。
1. 单击 **保存**。

## 保存许多联系人的自定义字段 {#saving-custom-fields-for-many-contacts}

1. 创建CSV电子表格，其中您的自定义字段位于其自己的列中。
1. 按照正 [常的CSV上传流程](http://docs.marketo.com/x/HIPS)，在字段映射屏幕上停止。
1. 从下拉菜单中选择“添加新 **的自定义字段** ”，而不是某个预设字段。
1. 输入所需的字段名称，然后单 **击确定**。
1. 完成CSV上传。 您的联系人将看到添加的自定义字段。

>[!NOTE]
>
>创建自定义字段后，可能需要大约30分钟时间，该字段才会显示在模板编辑器的动态字段下拉列表中。

## 如何在模板中使用自定义字段 {#how-to-use-your-custom-fields-in-a-template}

使用上述方法存储自定义字段后，您便可以在模板中引用这些字段。

1. [创建模板](http://docs.marketo.com/x/OCDG) ，然后单击“ **动态字段** ”按钮（如常）。
1. 从显 **示的** “自定义字段”(Custom Fields)下拉框中选择。
1. 您将看到预存储的自定义字段，并能够选择一个字段以填写模板。


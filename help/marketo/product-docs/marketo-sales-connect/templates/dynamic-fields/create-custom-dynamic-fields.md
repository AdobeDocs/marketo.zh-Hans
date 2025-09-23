---
unique-page-id: 14352508
description: 创建自定义动态字段 — Marketo文档 — 产品文档
title: 创建自定义动态字段
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 4%

---

# 创建自定义动态字段 {#create-custom-dynamic-fields}

创建自定义动态字段的方法有两种。

## 保存一个或多个联系人的自定义字段 {#saving-custom-fields-for-one-or-a-few-contacts}

1. 单击[!UICONTROL People]页面中联系人的姓名。

1. 选择[!UICONTROL Unsubscribe]旁边的下拉菜单并选择&#x200B;**[!UICONTROL Edit]**。

1. 向下滚动到编辑页面的底部。 然后，您可以为字段创建名称和值。

1. 单击 **[!UICONTROL Save]**。

## 正在保存多个联系人的自定义字段 {#saving-custom-fields-for-many-contacts}

1. 创建一个CSV电子表格，将您的自定义字段放置在其自己的列中。

1. 遵循[常规CSV上传流程](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)，在字段映射屏幕上停止。

1. 请从下拉列表中选择&#x200B;**[!UICONTROL Add a new Custom Field]**，而不是其中一个预设字段。

1. 输入所需的字段名称，然后单击&#x200B;**[!UICONTROL OK]**。

1. 完成CSV上传。 您的联系人将通过添加的自定义字段进行访问。

>[!NOTE]
>
>创建自定义字段后，大约需要30分钟该字段才会显示在模板编辑器的动态字段下拉列表中。

## 如何在模板中使用自定义字段 {#how-to-use-your-custom-fields-in-a-template}

使用上述方法存储自定义字段后，您就可以在模板中引用它们。

1. [创建模板](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md)，然后像往常一样单击&#x200B;**[!UICONTROL Dynamic Fields]**&#x200B;按钮。

1. 从出现的下拉列表中选择&#x200B;**[!UICONTROL Custom Fields]**。

1. 您将看到预存储的自定义字段，并可以选择其中一个字段来填写模板。

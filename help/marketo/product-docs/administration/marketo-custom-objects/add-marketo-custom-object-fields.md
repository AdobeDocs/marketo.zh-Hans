---
unique-page-id: 10093688
description: 添加Marketo自定义对象字段 — Marketo文档 — 产品文档
title: 添加Marketo自定义对象字段
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
source-git-commit: a51ee0b2b513d50febbffd7e3a72874c5ef4679c
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# 添加Marketo自定义对象字段 {#add-marketo-custom-object-fields}

创建自定义对象后，您需要向其添加字段以满足您的业务需求。

字段定义自定义对象使用的特定信息。 链接字段具有用于连接自定义对象的特殊作业，该作业在 [单独文章](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. 转到 **管理员** 的上界。

   ![](assets/add-marketo-custom-object-fields-1.png)

1. 单击 **Marketo自定义对象**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. 选择要将字段添加到右侧的对象。

   ![](assets/add-marketo-custom-object-fields-3.png)

1. 在 **字段** ，单击 **新建字段**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >上面显示的三个字段由Marketo在创建自定义对象时自动创建。 Marketo会自动管理这些字段，您无法编辑或删除这些字段。

1. 输入显示名称和说明。

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >只有在API名称获得批准之前，才可对其进行编辑。

1. 现在，从列表中选择适当的数据类型。

   ![](assets/add-marketo-custom-object-fields-6.png)

1. 如果要将新字段用作唯一标识符，请将重复数据消除滑块拉到上面。 单击 **保存** 完成。

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >重复数据删除字段可用于检索、更新或删除自定义对象。 每个自定义对象定义必须至少包含一个（且不超过三个）重复数据消除字段。

1. 添加您需要的任何其他字段。

   >[!NOTE]
   >
   >如果要构建一对多结构，则需要向自定义对象添加链接字段。 对于多对多结构，您不需要自定义对象中的链接字段，但必须在中间对象中添加两个链接字段。 请参阅 [添加Marketo自定义对象链接字段](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) 创建链接字段，以及 [了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) 以了解有关自定义对象类型的详细信息。

>[!MORELIKETHIS]
>
>* [添加Marketo自定义对象链接字段](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [编辑和删除Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [编辑和删除Marketo自定义对象字段](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)


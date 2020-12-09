---
unique-page-id: 10093688
description: 添加Marketo自定义对象字段- Marketo文档——产品文档
title: 添加Marketto自定义对象字段
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# 添加Marketto自定义对象字段 {#add-marketo-custom-object-fields}

创建自定义对象后，您需要向其添加字段以满足您的业务需求。

字段定义自定义对象使用的特定信息。 链接字段具有连接自定义对象的特殊作业，并在单独的文章中 [加以介绍](add-marketo-custom-object-link-fields.md)。

1. 单击 **管理**，在“数据库 **管理”中**，选择 **“Marketo** Custom Objects”。

   ![](assets/image2016-1-18-9-3a2-3a6.png)

1. 选择要在右侧添加字段的对象。

   ![](assets/image2016-1-18-9-3a5-3a3.png)

1. 在**字段**选项卡中，单击“新建 **字段”**。

   ![](assets/image2015-9-15-16-3a53-3a40.png)

   >[!NOTE]
   >
   >在您创建自定义对象时，Marketo会自动创建上面显示的三个字段。 Market To自动管理这些字段，您无法编辑或删除它们。

1. 输入显示名称和说明。

   ![](assets/image2015-10-5-11-3a35-3a48.png)

   >[!NOTE]
   >
   >API名称只能编辑，直至其获得批准。

1. 现在，从列表中选择适当的数据类型。

   ![](assets/image2015-10-5-11-3a37-3a24.png)

1. 如果要将新字段用作唯一标识符，请将重复数据消除滑块拉过。 单击**保存**以完成。

   ![](assets/image2015-10-5-11-3a40-3a12.png)

   >[!TIP]
   >
   >创建重复重复消除字段时，可以使用它删除数据库中的重复数据字段。

1. 添加您需要的任何其他字段。

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >如果要构建一对多结构，您需要向自定义对象添加一个“链接”字段。 对于多对多结构，您不需要自定义对象中的链接字段，但必须在中间对象中添加两个链接字段。 有关 [自定义对象类型的详细信息，请参](add-marketo-custom-object-link-fields.md) 阅添加Marketto自定义对象链接字段 [，以创建链接字段，](understanding-marketo-custom-objects.md) 以及了解Marketto自定义对象。

>[!MORELIKETHIS]
>
>* [添加Marketto自定义对象链接字段](add-marketo-custom-object-link-fields.md)
>* [编辑和删除Marketo自定义对象](edit-and-delete-a-marketo-custom-object.md)
>* [了解Marketo自定义对象](understanding-marketo-custom-objects.md)
>* [编辑和删除Marketto自定义对象字段](edit-and-delete-marketo-custom-object-fields.md)

>




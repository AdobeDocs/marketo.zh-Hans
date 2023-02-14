---
unique-page-id: 10093192
description: 创建Marketo自定义对象 — Marketo文档 — 产品文档
title: 创建Marketo自定义对象
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
source-git-commit: 99b11e17e9c2255a19c658b166e7b38c45cf1001
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# 创建Marketo自定义对象 {#create-marketo-custom-objects}

在Marketo中使用自定义对象来跟踪特定于您的业务的量度。 这可以是从汽车到课程的任何内容 — 无论您想在Marketo中模拟什么样的活动。

>[!NOTE]
>
>您可以设置自定义对象以在一对多或多对多的基础上工作。 创建初始对象的方式相同，但在开始向对象添加字段时，步骤不同。 请参阅  [了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) 以了解更多信息。

>[!NOTE]
>
>批准自定义对象后，便无法创建、编辑或删除链接或重复数据删除字段。

## 为一对多结构创建自定义对象 {#create-a-custom-object-for-a-one-to-many-structure}

此示例显示了Car自定义对象，用于一对多结构。 之后，您将创建一个课程自定义对象和一个中间对象，以在多对多结构中使用。

1. 转到 **管理员** 的上界。

   ![](assets/create-marketo-custom-objects-1.png)

1. 单击 **Marketo自定义对象**.

   ![](assets/create-marketo-custom-objects-2.png)

1. 单击 **新建自定义对象**.

   ![](assets/create-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >“Marketo自定义对象”选项卡在右侧显示所有自定义对象，以及任何已批准对象的详细信息，包括最新更新时的记录和字段数。

1. 输入显示名称。 API名称和复数名称会自动填充。 输入描述（可选）。

   ![](assets/create-marketo-custom-objects-4.png)

   >[!NOTE]
   >
   >在创建这些字段时，您可以编辑这些字段，但保存它们后，您只能编辑“复数名称”字段和 **在潜在客户详细信息中显示** 滑块。

1. 提取 **在潜在客户详细信息中显示** 滑过以显示 **显示** 要在“数据库”(Database)页上查看自定义对象数据时，请执行以下操作： 单击 **保存**.

   ![](assets/create-marketo-custom-objects-5.png)

1. 自定义对象信息显示您输入的内容。 请注意，它处于“草稿”状态。

   ![](assets/create-marketo-custom-objects-6.png)

   下一步是向 [构建自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >您只能通过列表导入来填充Marketo自定义对象，或者 [API](https://developers.marketo.com/documentation/rest/).

## 为多对多结构创建自定义对象 {#create-a-custom-object-for-a-many-to-many-structure}

此示例显示了一个课程自定义对象，您将使用该对象在人员/公司与课程之间创建多对多关系。 完成后，您将创建一个中间对象，以将其连接到数据库中的人员或公司。

>[!NOTE]
>
>对于多对多关系，您无需在自定义对象中创建链接。 相反，您将向中介对象添加两个链接（请参阅下文）。

1. 转到 **管理员** 的上界。

   ![](assets/create-marketo-custom-objects-7.png)

1. 单击 **Marketo自定义对象**.

   ![](assets/create-marketo-custom-objects-8.png)

1. 单击 **新建自定义对象**.

   ![](assets/create-marketo-custom-objects-9.png)

1. 输入显示名称。 API名称和复数名称会自动填充。 输入描述（可选）。

   ![](assets/create-marketo-custom-objects-10.png)

   >[!NOTE]
   >
   >在创建这些字段时，您可以编辑这些字段，但保存它们后，您只能编辑“复数名称”字段和 **在潜在客户详细信息中显示** 滑块。

1. 提取 **在潜在客户详细信息中显示** 滑过以显示 **显示** 要在“数据库”(Database)页上查看自定义对象数据时，请执行以下操作： 单击 **保存**.

   ![](assets/create-marketo-custom-objects-11.png)

1. 自定义对象信息显示您输入的内容。 请注意，它处于“草稿”状态。

   ![](assets/create-marketo-custom-objects-12.png)

   >[!NOTE]
   >
   >您只能通过列表导入来填充Marketo自定义对象，或者 [API](https://developers.marketo.com/documentation/rest/).

下一步是为您创建中间对象（请参阅下文）。 但在此之前，您需要创建一个字段以链接到该字段。

## 创建中间对象 {#create-an-intermediary-object}

使用中间对象将自定义对象连接到人员或公司。 在本例中，它用于将课程自定义对象中的课程与数据库中的人员或公司连接起来。

>[!NOTE]
>
>您无需为一对多自定义对象结构创建中间对象。

1. 转到 **管理员** 的上界。

   ![](assets/create-marketo-custom-objects-13.png)

1. 单击 **Marketo自定义对象**.

   ![](assets/create-marketo-custom-objects-14.png)

1. 单击 **新建自定义对象**.

   ![](assets/create-marketo-custom-objects-15.png)

1. 输入显示名称。 API名称和复数名称会自动填充。 输入描述（可选）。

   ![](assets/create-marketo-custom-objects-16.png)

   >[!NOTE]
   >
   >在创建这些字段时，您可以编辑这些字段，但保存它们后，您只能编辑“复数名称”字段和“显示在潜在客户详细信息”滑块。

1. 提取 **在潜在客户详细信息中显示** 滑过以显示 **显示** 要在“数据库”(Database)页上查看自定义对象数据时，请执行以下操作： 单击 **保存**.

   ![](assets/create-marketo-custom-objects-17.png)

1. 自定义对象信息显示您输入的内容。 请注意，它处于“草稿”状态。

   下一步是让您 [添加链接字段](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) 将中介对象连接到人员/公司和自定义对象。

>[!MORELIKETHIS]
>
>* [添加Marketo自定义对象字段](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [添加Marketo自定义对象链接字段](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)


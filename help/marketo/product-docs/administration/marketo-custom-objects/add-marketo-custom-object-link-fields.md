---
unique-page-id: 10097613
description: 添加Marketo自定义对象链接字段 — Marketo文档 — 产品文档
title: 添加Marketo自定义对象链接字段
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# 添加Marketo自定义对象链接字段 {#add-marketo-custom-object-link-fields}

创建自定义对象时，必须提供链接字段，以将自定义对象记录连接到正确的父记录。

* 对于一对多自定义结构，请使用自定义对象中的链接字段将其连接到个人或公司。
* 对于多对多结构，您使用两个链接字段，这些字段与单独创建的中间对象（这也是一种自定义对象类型）连接。 一个链接连接到数据库中的人员或公司，另一个链接连接到自定义对象。 在这种情况下，链接字段不在自定义对象本身中。

## 为一对多结构创建链接字段 {#create-a-link-field-for-a-one-to-many-structure}

以下是如何在自定义对象中为一对多结构创建链接字段。

1. 单击 **管理员**&#x200B;和 **数据库管理**，选择 **Marketo自定义对象**.

   ![](assets/image2016-1-18-13-3a25-3a11.png)

1. 在列表中选择自定义对象。

   ![](assets/image2016-1-14-15-3a6-3a2.png)

1. 在 **字段** ，单击 **新建字段**.

   ![](assets/image2015-9-17-14-3a9-3a19.png)

1. 命名链接字段并添加可选描述。 确保选择链接数据类型。

   ![](assets/image2015-10-5-13-3a24-3a57.png)

   >[!CAUTION]
   >
   >批准自定义对象后，您将无法返回并创建、编辑或删除链接或重复数据删除字段。

1. 选择链接对象是潜在客户（人员）还是公司。

   ![](assets/image2015-10-5-13-3a28-3a1.png)

   >[!NOTE]
   >
   >如果选择潜在客户，您将在列表中看到Id、电子邮件地址和任何自定义字段。
   >
   >如果选择公司，您将在列表中看到Id和任何自定义字段。

1. 选择要作为新字段的父项连接到的链接字段。

   ![](assets/image2015-10-5-13-3a30-3a6.png)

   >[!NOTE]
   >
   >链接字段中仅支持字符串字段类型。

1. 单击 **保存。**

   ![](assets/image2015-10-5-13-3a34-3a0.png)

## 为多对多结构创建链接字段 {#create-a-link-field-for-a-many-to-many-structure}

以下是如何在中间对象中创建链接字段以用于多对多结构。

>[!PREREQUISITES]
>
>您必须已创建中间对象以及要将其链接到的任何自定义对象。

1. 单击 **管理员**&#x200B;和 **数据库管理**，选择 **Marketo自定义对象**.

   ![](assets/image2016-1-18-9-3a8-3a14.png)

1. 选择要将字段添加到的中间对象。

   ![](assets/image2016-1-18-9-3a10-3a29.png)

1. 在 **字段** ，单击 **新建字段**.

   ![](assets/image2016-1-18-9-3a31-3a43.png)

1. 您需要创建两个链接字段。 一次创建一个。 首先，为数据库列表成员的字段命名（例如，leadID）。 添加可选描述。 确保选择链接数据类型。

   ![](assets/image2016-1-18-9-3a38-3a59.png)

   >[!CAUTION]
   >
   >批准自定义对象后，您将无法返回并创建、编辑或删除链接或重复数据删除字段。

1. 从数据库中选择链接对象，在此例中为“潜在客户”。

   ![](assets/image2016-1-18-9-3a50-3a48.png)

1. 选择您要连接到的链接字段（在本例中为Id）。

   ![](assets/image2016-1-18-9-3a53-3a54.png)

   >[!NOTE]
   >
   >链接字段中仅支持字符串字段类型。

1. 单击 **保存。**

   ![](assets/image2016-1-18-9-3a55-3a18.png)

1. 对自定义对象（在本例中为courseID）的第二个链接重复此过程。 链接对象名称将是课程，链接字段将是courseID。 由于您已经创建并批准了课程自定义对象，因此在下拉菜单中提供了这些选项。

   ![](assets/image2016-1-18-9-3a57-3a46.png)

1. 创建要在中间对象中使用的任何其他字段，如enrollmentID或grade。

## 使用自定义对象 {#using-custom-objects}

下一步是在智能营销活动的过滤器中使用这些自定义对象。 通过多对多关系，您可以选择多个人员/公司和多个自定义对象。 在以下示例中，将列出数据库中符合这些标准的任何人。 coursename字段来自课程自定义对象，而注册等级来自中间对象。

![](assets/image2016-1-14-15-3a57-3a59.png)

>[!MORELIKETHIS]
>
>* [添加Marketo自定义对象字段](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [编辑和删除Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [编辑和删除Marketo自定义对象字段](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)


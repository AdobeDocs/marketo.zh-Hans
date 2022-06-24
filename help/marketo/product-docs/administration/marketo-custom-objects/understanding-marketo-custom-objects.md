---
unique-page-id: 10093188
description: 了解Marketo自定义对象 — Marketo文档 — 产品文档
title: 了解Marketo自定义对象
exl-id: f18b1689-c7bc-4da0-8326-7b29733d527d
source-git-commit: 6f17d79344653d1b2c364753d774998e343c9808
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# 了解Marketo自定义对象 {#understanding-marketo-custom-objects}

使用自定义对象来跟踪特定于您的业务的量度。

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关详细信息，请联系您的销售代表。

在智能营销活动中将自定义对象用作过滤器和触发器。 例如：

* **过滤器**:仅向特定车辆品牌的所有者发送电子邮件
* **触发器**:在将自定义对象添加到人员或公司时发送电子邮件。

您可以在一对多或多对多关系中设置自定义对象。 例如：

* **一对多**:一个人拥有几辆汽车
* **多对多**:多个学生从一个课程目录中注册了多个课程

一对多结构使用单个链接字段将自定义对象连接到个人或公司。

多对多自定义对象使用两个链接字段，这是中间对象的一部分。 一个链接字段与人员或公司相连，另一个字段与自定义对象（如课程目录）相连。 此中间对象可以包含其他自定义字段，如课程级别或出席日期，这进一步定义了连接的性质。

>[!TIP]
>
>在用户界面中使用逗号分隔值(CSV)导入自定义对象，以测试和验证数据示例。 然后，使用API上传所有文件。

>[!CAUTION]
>
>您无法恢复自定义对象，因此在删除这些对象之前，请确保不再需要这些对象。

## 访问Marketo自定义对象 {#accessing-marketo-custom-objects}

1. 要创建或编辑Marketo自定义对象，请单击 **管理员** 然后 **Marketo自定义对象** 链接。

   ![](assets/understanding-marketo-custom-objects-1.png)

1. “Marketo自定义对象”显示的右侧列出了所有自定义对象，但主网格中仅列出了已批准的自定义对象。

   ![](assets/understanding-marketo-custom-objects-2.png)

1. 网格显示对象名称、记录数、字段数和最近更新的日期。

   >[!TIP]
   >
   >Marketo会自动更新这些字段，但您可以通过单击“记录”列中的图标来刷新显示内容。

1. 单击右侧的对象名称以打开详细信息页面。

   ![](assets/understanding-marketo-custom-objects-3.png)

## 查看与人员关联的自定义对象 {#view-custom-objects-associated-to-a-person}

创建自定义对象结构后，当您上载特定的自定义对象数据时，自定义对象将自动与数据库中的人员关联，使用自定义对象中的链接字段。 您可以从人员详细信息页面的“自定义对象”选项卡中查看信息。

1. 转到 **数据库**.

   ![](assets/understanding-marketo-custom-objects-4.png)

1. 打开数据库，然后单击 **人员** 选项卡。 双击与自定义对象关联的人员的记录。

   ![](assets/understanding-marketo-custom-objects-5.png)

1. 在人员详细信息页面上，单击 **自定义对象** 选项卡。 从下拉列表中选择对象。

   ![](assets/understanding-marketo-custom-objects-6.png)

1. 现在，您可以查看与该人员关联的该类型所有自定义对象的列表。

   ![](assets/understanding-marketo-custom-objects-7.png)

## 在公司中使用自定义对象 {#using-custom-objects-with-companies}

如果您从CRM中同步公司，或者如果您使用API明确创建公司，则链接到公司的自定义对象最有效。 我们还建议您使用公司ID作为链接字段。

如果您在Marketo中有多个人员是CRM或仅Marketo记录中的记录，则链接到公司的自定义对象将不会与多个单个记录关联。 这是因为，仅当公司从CRM向下同步，或者如果您使用API明确创建公司，才支持在公司下面包含多个人员的公司。

自定义对象只能直接链接到单个记录。 这意味着，当您的自定义对象类型通过公司字段关联时，如果您使用Marketo的REST API管理公司，则应确保您的人员记录通过CRM中的联系人转化或externalCompanyId字段与公司关联。 对于未明确链接到公司记录的人员记录，使用公司链接的自定义对象将随机链接到单个记录，即使公司字段的值在许多人之间共享也是如此。

请参阅 [导入自定义对象数据](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md) 以了解更多信息。

>[!MORELIKETHIS]
>
>* [创建Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [批准自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [编辑和删除Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [添加Marketo自定义对象字段](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [编辑和删除Marketo自定义对象字段](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [导入自定义对象数据](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)


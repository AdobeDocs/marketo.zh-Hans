---
unique-page-id: 10093188
description: 了解Marketo自定义对象- Marketo文档——产品文档
title: 了解Marketo自定义对象
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---


# 了解Marketo自定义对象 {#understanding-marketo-custom-objects}

使用自定义对象跟踪特定于您企业的指标。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>**可用性**
>
>并非所有客户都购买了此功能。 有关详细信息，请与销售代表联系。

在智能活动中将自定义对象用作过滤器和触发器。 例如：

* **过滤器**:仅向特定汽车品牌的所有者发送电子邮件
* **触发器**:在将自定义对象添加到人员或公司时发送电子邮件。

您可以在一对多或多对多关系中设置自定义对象。 例如：

* **一对多**:一个人拥有几辆车
* **多对多**:多个学生从课程目录登记了多个课程

一对多结构使用单个链接字段将自定义对象连接到个人或公司。

多对多自定义对象使用两个链接字段，它是中间对象的一部分。 一个链接字段连接到个人或公司，另一个链接字段连接到自定义对象，如课程目录。 此中间对象可包含其他自定义字段，如课程级别或出席日期，这进一步定义了连接的性质。

>[!TIP]
>
>在用户界面中使用逗号分隔值(CSV)导入自定义对象，以测试和验证数据范例。 然后，使用API上传您的所有文件。

>[!CAUTION]
>
>无法恢复自定义对象，因此，在删除这些对象之前，请确保不再需要它们。

## 访问Marketo自定义对象 {#accessing-marketo-custom-objects}

1. 要创建或编辑Marketo自定义对象，请单击**Admin **，然后单击“Marketo自 **定义对象”**&#x200B;链接。

   ![](assets/image2016-5-18-16-3a59-3a30.png)

1. “营销至自定义对象”在右侧显示所有自定义对象的列表，但仅在主网格中显示已批准的自定义对象。

   ![](assets/image2016-6-10-15-3a14-3a18.png)

1. 网格显示对象名称、记录数、字段数和最近更新的日期。

   >[!TIP]
   >
   >Market可自动更新这些字段，但您可以单击“记录”列中的图标来刷新显示屏。

1. 单击右侧的对象名称以打开详细信息页面。

   ![](assets/image2016-6-10-15-3a15-3a29.png)

## 视图与人员关联的自定义对象 {#view-custom-objects-associated-to-a-person}

在创建自定义对象结构后，当您上传特定的自定义对象数据时，自定义对象将使用自定义对象中的链接字段自动与数据库中的人员相关联。 您可以从人员详细信息页面的“自定义对象”选项卡中视图信息。

1. 转到数 **据库**。

   ![](assets/db.png)

1. 打开数据库，然后单击“ **人员** ”选项卡。 多次-单击您与自定义对象关联的人的记录。

   ![](assets/five.png)

1. 在人员详细信息页面上，单击“自定 **义对象** ”选项卡。 从下拉列表中选择对象。

   ![](assets/six.png)

1. 现在，您可以视图与该人关联的该类型所有自定义对象的列表。

   ![](assets/seven.png)

## 将自定义对象与公司 {#using-custom-objects-with-companies}

如果您从CRM同步公司，或者使用API显式创建公司，则链接到该公司的自定义对象最有效。 我们还建议您使用公司ID作为链接字段。

如果您在Marketo中有多个人员是CRM或仅限Marketo的记录，则链接到公司的自定义对象将不会与多个单独记录关联。 这是因为只有当公司从CRM向下同步时，或者如果您使用API显式创建公司时，才支持在公司下包含多个人员。

自定义对象只能直接链接到单个记录。 这意味着，当自定义对象类型通过公司字段链接时，如果您使用Marketo的REST API管理公司，则应确保您的个人记录与公司关联，或者在CRM中使用联系人转换，或者使用externalCompanyId字段。 对于未明确链接到公司记录的个人记录，使用公司链接的自定义对象将随机链接到单个记录，即使公司字段的值在许多人之间共享也是如此。

有关详 [细信息，请参阅](import-custom-object-data.md) “导入自定义对象数据”。

>[!NOTE]
>
>**相关文章**
>
>* [创建Marketo自定义对象](create-marketo-custom-objects.md)
>* [批准自定义对象](approve-a-custom-object.md)
>* [编辑和删除Marketo自定义对象](edit-and-delete-a-marketo-custom-object.md)
>* [添加Marketto自定义对象字段](add-marketo-custom-object-fields.md)
>* [编辑和删除Marketto自定义对象字段](edit-and-delete-marketo-custom-object-fields.md)
>* [导入自定义对象数据](import-custom-object-data.md)

>




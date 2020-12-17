---
unique-page-id: 10093192
description: 创建Marketo自定义对象- Marketo文档——产品文档
title: 创建Marketo自定义对象
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---


# 创建Marketo自定义对象{#create-marketo-custom-objects}

使用Market中的自定义对象跟踪特定于您企业的指标。 这可能是从汽车到课程的任何东西——无论您想在Market中建模以运行活动。

>[!NOTE]
>
>您可以设置自定义对象，使其在一对多或多对多的基础上工作。 创建初始对象的方式相同，但在向对象添加字段时，步骤不同。 有关详细信息，请参阅[了解Marketo Custom Objects](understanding-marketo-custom-objects.md)。

>[!NOTE]
>
>在批准自定义对象后，您不能创建、编辑或删除链接或重复数据消除字段。

## 为一对多结构{#create-a-custom-object-for-a-one-to-many-structure}创建自定义对象

此示例显示Car自定义对象，用于一对多结构。 稍后，您将创建课程自定义对象和要在多对多结构中使用的中间对象。

1. 单击&#x200B;**Admin**，在&#x200B;**数据库管理**&#x200B;中选择&#x200B;**Marketo Custom Objects**。

   ** ![](assets/image2016-1-18-13-3a12-3a19.png)

   **

1. 单击&#x200B;**新建自定义对象**。

   ![](assets/image2016-5-18-16-3a28-3a4.png)

   >[!NOTE]
   >
   >“营销商自定义对象”选项卡在右侧显示所有自定义对象以及任何已批准对象的详细信息，包括最新更新时的记录和字段数。

1. 输入显示名称。 API名称和复数名称将自动填充。 输入说明（可选）。

   ![](assets/image2015-9-15-16-3a29-3a17.png)

   >[!NOTE]
   >
   >在创建这些字段时，您可以编辑它们，但在保存它们后，您只能编辑Plural Name字段和&#x200B;**在Lead Detail中显示**&#x200B;滑块。

1. 如果要在“潜在客户视图库”页上自定义对象数据，请拖动“在潜在客户详细信息中显示”**滑块以显示&#x200B;**“显示”**。 单击&#x200B;**保存**。

   ![](assets/image2015-9-15-16-3a32-3a2.png)

1. 自定义对象信息显示您输入的内容。 注意它处于“草稿”状态。

   ![](assets/image2015-9-15-16-3a38-3a22.png)

   下一步是向[构建自定义对象](add-marketo-custom-object-fields.md)添加字段。

   >[!NOTE]
   >
   >您只能通过列表导入或[API](http://developers.marketo.com/documentation/rest/)填充Marketo自定义对象。

## 为多对多结构{#create-a-custom-object-for-a-many-to-many-structure}创建自定义对象

此示例显示一个课程自定义对象，您将使用它在人/公司和课程之间创建多对多关系。 完成后，您将创建一个中间对象，将其连接到数据库中的人员或公司。

>[!NOTE]
>
>对于多对多关系，您无需在自定义对象中创建链接。 相反，您将添加两个指向中间对象的链接（请参阅下面的内容）。

1. 单击&#x200B;**Admin**，在&#x200B;**数据库管理**&#x200B;中选择&#x200B;**Marketo Custom Objects**。

   ![](assets/image2016-1-18-13-3a16-3a25.png)

1. 单击&#x200B;**新建自定义对象**。

   ![](assets/image2016-5-18-16-3a32-3a42.png)

1. 输入显示名称。 API名称和复数名称将自动填充。 输入说明（可选）。

   ![](assets/image2016-1-14-13-3a38-3a46.png)

   >[!NOTE]
   >
   >在创建这些字段时，您可以编辑它们，但在保存它们后，您只能编辑Plural Name字段和&#x200B;**在Lead Detail中显示**&#x200B;滑块。

1. 拖动“潜在客户详细信息”**滑块以显示“如果要在“潜在客户视图库”页上自定义对象数据，则显示“显示”。 单击&#x200B;**保存**。

   ![](assets/image2016-1-14-13-3a42-3a56.png)

1. 自定义对象信息显示您输入的内容。 注意它处于“草稿”状态。

   ![](assets/image2016-1-18-8-3a38-3a58.png)

   >[!NOTE]
   >
   >您只能通过列表导入或[API](http://developers.marketo.com/documentation/rest/)填充Marketo自定义对象。

下一步是创建中间对象（请参阅下面的内容）。 但在此之前，您需要创建一个与其链接的字段。

## 创建中间对象{#create-an-intermediary-object}

使用中间对象将自定义对象连接到人或公司。 在此示例中，它用于将课程自定义对象中的课程连接到数据库中的人员或公司。

>[!NOTE]
>
>您无需为一对多自定义对象结构创建中间对象。

1. 单击&#x200B;**Admin**，在&#x200B;**数据库管理**&#x200B;中，选择&#x200B;**Marketto Custom Objects**。

   ![](assets/image2016-1-18-13-3a17-3a40.png)

1. 单击&#x200B;**新建自定义对象**。

   ![](assets/image2016-5-18-16-3a33-3a16.png)

1. 输入显示名称。 API名称和复数名称将自动填充。 输入说明（可选）。

   ![](assets/image2016-1-14-14-3a10-3a44.png)

   >[!NOTE]
   >
   >在创建这些字段时，您可以编辑它们，但在保存它们后，您只能编辑“多名”字段和“在潜在客户详细信息中显示”滑块。

1. 拖动&#x200B;**在潜在客户详细信息中显示**&#x200B;滑块，显示如果要在“潜在客户视图库”页上自定义对象数据，则显示显示。 单击&#x200B;**保存**。

   ![](assets/image2016-1-14-14-3a12-3a49.png)

1. 自定义对象信息显示您输入的内容。 注意它处于“草稿”状态。

   下一步是[添加链接字段](add-marketo-custom-object-link-fields.md)，将中间对象连接到人/公司和自定义对象。

>[!MORELIKETHIS]
>
>* [添加Marketto自定义对象字段](add-marketo-custom-object-fields.md)
>* [添加Marketto自定义对象链接字段](add-marketo-custom-object-link-fields.md)
>* [了解Marketo自定义对象](understanding-marketo-custom-objects.md)

>




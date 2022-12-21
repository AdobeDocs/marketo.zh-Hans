---
unique-page-id: 12983101
description: 将自定义字段映射到Marketo - Marketo文档 — 产品文档
title: 将自定义字段映射到Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# 将自定义字段映射到Marketo {#map-custom-fields-to-marketo}

您可能希望收集的信息可能多于Facebook默认存储的标准信息，例如某人使用您的在线投放服务的频率。 您可以通过 [创建自定义问题](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) 在您的Facebook潜在客户广告中。

但是， **Marketo不会自动开始收集此数据**. 为了使Marketo开始捕获自定义字段值，您 **必须** 将这些自定义字段映射到Marketo中的字段。

以下是如何在管理员的LaunchPoint区域中设置此设置。

>[!NOTE]
>
>**需要管理员权限**

1. 转到“管理员”区域，然后单击 **LaunchPoint**. 在“已安装的服务”下，查找并编辑 **Facebook潜在客户广告**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. 单击 **下一个**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. 将授权帐户保留为原样 **not** 进行任何更改。 单击 **下一个**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. 与以前一样，保持选定页面原样 — do **not** 进行任何更改。 单击 **下一个**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. 在此处，您可以将自定义Facebook字段映射到Marketo字段。 单击 **添加。**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. 在新行中，输入Facebook自定义字段的名称。

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >只有已保存到Facebook表单模板的字段才会在此处显示为选项。

1. 单击 **Marketo字段** 列。 键入以搜索要映射到的字段。 选择字段后，单击 **保存**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >如果您在Marketo中还没有要将Facebook字段映射到的字段，请了解如何 [创建自定义字段](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>您 **必须** 对任何新的Facebook字段执行此过程，以便Marketo收集数据。

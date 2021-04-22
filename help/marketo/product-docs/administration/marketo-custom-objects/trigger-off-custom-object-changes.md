---
unique-page-id: 11378713
description: 触发自定义对象更改 — Marketo Docs — 产品文档
title: 触发自定义对象更改
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# 触发自定义对象更改{#trigger-off-custom-object-changes}

>[!NOTE]
>
>此功能仅可用：
>
>* 针对使用Orion基础架构的客户
>* 仅用于Marketo自定义对象，而不是通过本机Salesforce或Microsoft Dynamics集成同步的自定义对象
>* 作为触发器，而不是过滤器

>
>
请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)以启用自定义对象更改触发器。

在智能活动的智能列表中，当将自定义对象添加到人物或公司时，您可以触发流动操作。 您还可以创建一个智能列表，它使用自定义对象中的&#x200B;*change*&#x200B;作为触发器。 例如，使用它在课程名称更新时发送电子邮件。

>[!NOTE]
>
>在更改自定义对象记录时不会创建活动日志条目。

1. 在Marketo中，转到&#x200B;**营销活动。**

   ![](assets/image2016-7-25-15-3a49-3a52.png)

1. 创建或打开现有智能活动，然后选择智能列表。

   ![](assets/image2016-7-25-16-3a9-3a19.png)

1. 搜索所需的触发器并将其拖动到画布上。

   ![](assets/image2016-7-25-16-3a16-3a43.png)

1. 选择触发器属性。

   ![](assets/image2016-7-25-16-3a21-3a42.png)

1. （可选）设置约束。

   ![](assets/image2016-9-6-14-3a25-3a22.png)

1. 你在这。 更改将自动保存。

   ![](assets/image2016-9-6-14-3a25-3a54.png)

   >[!NOTE]
   >
   >* [创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)


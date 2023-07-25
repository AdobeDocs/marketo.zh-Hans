---
unique-page-id: 2359663
description: 设置隐藏表单字段值 — Marketo文档 — 产品文档
title: 设置隐藏表单字段值
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# 设置隐藏表单字段值 {#set-a-hidden-form-field-value}

隐藏字段通常会动态填充。 它们不会显示给填写表单的人。 以下是如何设置该值。

>[!PREREQUISITES]
>
>[将表单字段设置为隐藏](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## 选择字段 {#select-the-field}

1. 在表单中，选择隐藏字段并单击 **编辑** 对象 **自动填写**.

   ![](assets/autofill.png)

## 使用默认值 {#use-default-value}

通过选择使用默认值，您可以对特定值进行硬编码，以便在提交此表单时始终使用。 输入“默认值”并单击“保存”。

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL参数 {#url-parameter}

如果您要在填写表单时从人员所在的页面中捕获URL参数（查询字符串），则可以使用 **URL参数** 以填充隐藏字段。

>[!NOTE]
>
>这些参数有点技术含量高，不是吗？ 但一旦你得到它们，它们就会变得强大。 此 [关于查询字符串的维基百科页面](https://en.wikipedia.org/wiki/Query_string) 会有所帮助。

1. 选择 **URL参数** 对象 **获取值类型**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. 输入 **参数名称** 并单击 **保存**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>您可以输入默认值，以防找不到URL参数。

## Cookie值 {#cookie-value}

如果您将数据存储在Cookie中，则可以使用 **Cookie值** 以在表单提交时提取数据。

1. 选择 **Cookie值** 对象 **值获取来源**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. 输入所需的Cookie参数名称，然后单击 **保存**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >您可以输入默认值，以防找不到参数/Cookie。

## 反向链接参数 {#referrer-parameter}

如果您要在填写表单之前从访客来自的页面捕获数据，则可以使用 **反向链接参数**.

1. 设置 **值获取来源** 到 **反向链接参数**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. 输入 **参数名称** ，然后点击 **保存**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >您可以输入 **默认值** 如果找不到反向链接参数。

1. 单击 **完成**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. 单击 **批准并关闭**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)

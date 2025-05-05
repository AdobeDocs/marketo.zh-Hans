---
unique-page-id: 2359663
description: 设置隐藏表单字段值 — Marketo文档 — 产品文档
title: 设置隐藏表单字段值
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# 设置隐藏表单字段值 {#set-a-hidden-form-field-value}

隐藏字段通常会动态填充。 它们不会显示给填写表单的人。 下面是如何设置该值的。

>[!PREREQUISITES]
>
>[将表单字段设置为隐藏](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## 选择字段 {#select-the-field}

1. 在您的表单中，选择隐藏字段并单击&#x200B;**自动填写**&#x200B;的&#x200B;**编辑**。

   ![](assets/autofill.png)

## 使用默认值 {#use-default-value}

通过选择使用默认值，您可以对特定值进行硬编码，以便在提交此表单时始终使用。 输入“默认值”，然后单击“保存”。

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL Parameter {#url-parameter}

如果要在填写表单时从人员所在的页面中捕获URL参数（查询字符串），则可以使用&#x200B;**URL参数**&#x200B;填充隐藏字段。

>[!NOTE]
>
>这些参数有点技术性，不是吗？ 一旦你得到它们，它们就会变得强大。 查询字符串[&#128279;](https://en.wikipedia.org/wiki/Query_string)上的此Wikipedia页面有些帮助。

1. 为&#x200B;**获取值类型**&#x200B;选择&#x200B;**URL参数**。

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. 输入&#x200B;**参数名称**&#x200B;并单击&#x200B;**保存**。

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>您可以输入默认值，以备找不到URL参数时使用。

## Cookie值 {#cookie-value}

如果您将数据存储在Cookie中，则可以使用&#x200B;**Cookie值**&#x200B;在提交表单时提取数据。

1. 为&#x200B;**从**&#x200B;获取值选择&#x200B;**Cookie值**。

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. 输入所需的Cookie参数名称，然后单击&#x200B;**保存**。

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >您可以输入默认值，以防未找到参数/Cookie。

## 反向链接参数 {#referrer-parameter}

如果您要在填写表单之前从访客来自的页面中捕获数据，则可以使用&#x200B;**反向链接参数**。

1. 将&#x200B;**获取值从**&#x200B;设置为&#x200B;**反向链接参数**。

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. 输入要从反向链接URL中抓取的&#x200B;**参数名称**，然后单击&#x200B;**保存**。

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >您可以输入&#x200B;**默认值**，以防未找到反向链接参数。

1. 单击&#x200B;**完成**。

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. 单击&#x200B;**批准并关闭**。

   ![](assets/image2014-9-15-13-3a10-3a43.png)

---
unique-page-id: 2359663
description: 设置隐藏的表单字段值- Marketo Docs —— 产品文档
title: 设置隐藏表单字段值
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---


# 设置隐藏表单字段值 {#set-a-hidden-form-field-value}

隐藏字段通常动态填充。 不会向填写表单的人显示。 下面介绍如何设置值。

>[!PREREQUISITES]
>
>[将表单字段设置为隐藏](set-a-form-field-as-hidden.md)

## 选择字段 {#select-the-field}

1. 在表单中，选择隐藏字段，然后单击“ **编辑** ”以 **自动填写**。

   ![](assets/autofill.png)

## 使用默认值 {#use-default-value}

通过选择使用默认值，您可以硬编码在提交此表单时始终使用的特定值。 输入默认值，然后单击保存。

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL参数 {#url-parameter}

如果要在填写表单时从人员所在的页面捕获URL参数(查询字符串)，可以使用 **URL****参** 数来填充隐藏字段。

>[!NOTE]
>
>参数有点技术，不是吗？ 但一旦你得到了它们，它们就会变得强大。 查询 [字符串上的这个维基百科页面](http://en.wikipedia.org/wiki/Query_string) ，有些帮助。

1. 为“ **获取值** ”类 **型选择URL参数**。

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. 输入参 **数名称** ，然后单击 **保存**。

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>如果找不到URL参数，可以输入默认值。

## Cookie值 {#cookie-value}

如果您将数据存储在cookie中，则可以在提 **交表单****时使用Cookie** Value来获取数据。

1. 选择 **Cookie** **Value****Get** Value ******** From Jat.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. 输入所需的Cookie参数名称，然后单击 **保存**。

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >如果找不到参数/cookie，可以输入默认值。

## 推荐人参数 {#referrer-parameter}

如果要在填写表单之前从访客来自的页面捕获数据，可以使用 **推荐人** 参数 ****。

1. 设 **置Get** **Value** From **Adobe Adobe Prameter** Amperater从 **推荐人******&#x200B;到参数。

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. 输入 **要从推荐人** URL捕获的参数名称，然后单击 **保存**。

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >如果找不到 **推荐人****参数，** 则可以输入默认值。

1. 单击 **完成**。

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. 单击 **批准并关闭**。

   ![](assets/image2014-9-15-13-3a10-3a43.png)

真贴心！ 你表现不错。 有更多关于表单的 [信息](http://docs.marketo.com/display/docs/forms)。

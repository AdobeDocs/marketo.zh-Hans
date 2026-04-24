---
unique-page-id: 7515401
description: 了解如何在Marketo中创建引导式登陆页面模板。 使用语法定义引导编辑器的可编辑区域和变量。
title: 创建引导式登录页面模板
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
source-git-commit: 4a95c37fe8c09cdbe3cc84e701f0fc50286fc276
workflow-type: tm+mt
source-wordcount: '1127'
ht-degree: 21%

---

# 创建引导式登录页面模板 {#create-a-guided-landing-page-template}

引导式登陆页面模板具有特殊的语法。 使用此语法可指定可自定义的内容以及内容在从模板构建的每个登陆页面上的结束位置。 只有指定为可编辑的区域或变量才可以在“引导式”登陆页面编辑器中自定义。

>[!TIP]
>
>使用良好的命名惯例，您的营销团队就会爱上您。

有两种方法可声明页面上的某些内容应可编辑：

* 将对象声明为“element”。 登陆页面创建者将能够将图像、文本或Marketo资源添加到这些指定区域中。
* 将字符串声明为“变量”。 登陆页面创建者将能够通过true/false杠杆使用字符串、颜色或布尔状态替换该变量。

## 可编辑元素 {#editable-elements}

通过以下方法声明元素：向模板中添加普通DOM元素，然后使用Marketo特定的类名称修饰该元素。

## 文本 {#text}

如果将某个区域定义为富文本，用户即可[使用 Marketo 的富文本编辑器](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)来编辑其内容。

必需属性：
**类**：&quot;mktoText&quot;
**id**：ID 字符串。 仅可包含字母、数字、短横线“-”和下划线“_”。 不允许包含空格。 必须唯一。
**mktoName**：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

可选：
具有类mktoText的元素的内容（如果提供）将用作可编辑区域的默认值。

示例：

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## 图像 {#image}

您可以使用两个选项来定义可编辑的图像元素。 您可以使用`<div>`或`<img>`标记，前者用于指定图像将插入到的容器。

## 选项 1 — 使用 `<div>` {#option-use-a-div}

必需属性：

类： &quot;mktoImg&quot;
id： ID字符串。 仅可包含字母、数字、短横线“-”和下划线“_”。 不允许包含空格。 必须唯一。
mktoName ：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

可选：
mktoImgClass: String. 此处的值将添加到该 div 内 `<img>` 元素的类属性中。

示例：

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## 选项 2 — 使用 `<img>` {#option-use-a-img}

必需属性：
类： &quot;mktoImg&quot;
id： ID字符串。 仅可包含字母、数字、短横线“-”和下划线“_”。 不允许包含空格。 必须唯一。
mktoName ：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

可选：
src: String URL. This will be used as the default value for the image.

示例：

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>When using the `<img>` version, the rendered HTML will contain a generated div wrapper around the `<img>` tag. It will be set to class .&quot;mktoImg.mktoGen,&quot; and will be display:inline-block.

## 表单 {#form}

Example:Required attributes:
**class**: &quot;mktoForm&quot;
**id**：ID 字符串。 仅可包含字母、数字、短横线“-”和下划线“_”。 不允许包含空格。 必须唯一。
**mktoName**：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## 代码段 {#snippet}

必需属性：
**class**: &quot;mktoSnippet&quot;
**id**：ID 字符串。 仅可包含字母、数字、短横线“-”和下划线“_”。 不允许包含空格。 必须唯一。
**mktoName**：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

示例：

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## Share Button {#share-button}

必需属性：
**class**: &quot;mktoShareButton&quot;
**id**：ID 字符串。 仅可包含字母、数字、短横线“-”和下划线“_”。 不允许包含空格。 必须唯一。
**mktoName**：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

示例：

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## 视频 {#video}

>[!NOTE]
>
>When using the video element in a landing page, Marketo only supports videos from YouTube. If you use another service, we recommend utilizing a rich text box and pasting in the video&#39;s embed code.

必需属性：
**class**: &quot;mktoVideo&quot;
**id**：ID 字符串。 仅可包含字母、数字、短横线“-”和下划线“_”。 不允许包含空格。 必须唯一。
**mktoName**：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

示例：

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## Editable Variables {#editable-variables}

All variable types are used by referencing the value of their id attribute wrapped inside of a ${ } character sequence. They can be used anywhere in the document, except for inside of other variable declarations.

示例：

`${var1}`

**Declaration:**

Variables are declared as meta tags inside the `<head>` element of the template. There are three types of variables available for use: String, Color, and Boolean.

## 字符串 {#string}

Required Attributes:
**class** : &quot;mktoString&quot;,
**id**：ID 字符串。 仅可包含字母、数字、短横线“-”和下划线“_”。 不允许包含空格。 必须唯一。
**mktoName**：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

可选：
**default**: String value for the attribute. Blank if none provided.
**allowHtml**: &quot;true&quot; or &quot;false&quot;. Controls if the value will be printed without being HTML escaped. Defaults to &quot;false&quot; if unset.

Basic Example:

`<meta class="mktoString" id="var1" mktoName="My Variable">`

具有所有属性的示例：

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## 颜色 {#color}

必需属性：
**类** ： &quot;mktoColor&quot;，
**id**：ID 字符串。 仅可包含字母、数字、短横线“-”和下划线“_”。 不允许包含空格。 必须唯一。
**mktoName**：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

可选：
**默认值**：7位十六进制字符颜色代码。 例如：“#336699”

基本示例：

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

具有所有属性的示例：

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## 布尔值 {#boolean}

必需属性：
**类** ： &quot;mktoBoolean&quot;，
**id**：ID 字符串。 仅可包含字母、数字、短横线“-”和下划线“_”。 不允许包含空格。 必须唯一。
**mktoName**：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

可选：
**默认值**：布尔字符串。 “true”或“false”控制值是从ON还是OFF位置开始。 &quot;false&quot;（如果未提供）。
**false_value**：字符串。 变量处于OFF位置时要插入的值。 &quot;false&quot;（如果未提供）。
**true_value**：字符串。 当变量处于ON位置时要插入的值。 如果未提供，则为“true”。
**false_value_name**：字符串。 当值处于OFF位置时将在登陆页面编辑器中显示的显示名称。 如果未提供，则为“关”。
**true_value_name**：字符串。 当值处于“开”位置时将在登陆页面编辑器中显示的显示名称。 如果未提供，则为“开”。

基本示例：

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

具有所有属性的示例：

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

此示例显示了一个常见用例，其中布尔变量通过将css display属性的值设置为“block”或“none”来控制css元素的可见性，从而通过CSS按ID显示/隐藏元素。 登陆页面编辑器将使用显示名称Show/Hide而不是OFF/ON。

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>程序令牌(my.token)还可以在引导式或自由格式登陆页面中的任意位置使用。

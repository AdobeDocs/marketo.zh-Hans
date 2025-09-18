---
unique-page-id: 7515401
description: 创建引导式登陆页面模板 — Marketo文档 — 产品文档
title: 创建引导式登录页面模板
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
source-git-commit: 29c1b59c9d2598626f546554a8bdc1b26b9e1590
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 2%

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

如果将区域定义为富文本，用户将可以使用Marketo的富文本编辑器[编辑其内容](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)。

必需属性：
**类**： &quot;mktoText&quot;
**id**： ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
**mktoName** ：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

可选：
具有类mktoText的元素的内容（如果提供）将用作可编辑区域的默认值。

示例：

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## 图像 {#image}

您可以使用两个选项来定义可编辑的图像元素。 您可以使用`<div>`或`<img>`标记，前者用于指定图像将插入到的容器。

## 选项1 — 使用`<div>` {#option-use-a-div}

必需属性：

类： &quot;mktoImg&quot;
id： ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
mktoName ：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

可选：
mktoImgClass：字符串。 此处的值将添加到div内`<img>`元素的类属性中。

示例：

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## 选项2 — 使用`<img>` {#option-use-a-img}

必需属性：
类： &quot;mktoImg&quot;
id： ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
mktoName ：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

可选：
src：字符串URL。 这将用作图像的默认值。

示例：

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>使用`<img>`版本时，渲染的HTML将在`<img>`标记周围包含生成的div包装器。 它将设置为类。”mktoImg.mktoGen”和“，将显示为:inline-block。

## 表单 {#form}

示例:Required属性：
**类**： &quot;mktoForm&quot;
**id**： ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
**mktoName** ：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## 代码段 {#snippet}

必需属性：
**类**： &quot;mktoSnippet&quot;
**id**： ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
**mktoName** ：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

示例：

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## “共享”按钮 {#share-button}

必需属性：
**类**： &quot;mktoShareButton&quot;
**id**： ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
**mktoName** ：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

示例：

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## 视频 {#video}

>[!NOTE]
>
>在登陆页面中使用视频元素时，Marketo仅支持来自YouTube的视频。 如果您使用其他服务，我们建议使用富文本框并在视频的嵌入代码中粘贴。

必需属性：
**类**： &quot;mktoVideo&quot;
**id**： ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
**mktoName** ：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

示例：

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## 可编辑的变量 {#editable-variables}

所有变量类型均可通过引用包装在${ }字符序列中的ID属性的值来使用。 它们可以在文档中的任意位置使用，但其他变量声明内部除外。

示例：

`${var1}`

**声明：**

变量在模板的`<head>`元素中声明为元标记。 可以使用三种类型的变量：字符串、颜色和布尔值。

## 字符串 {#string}

必需属性：
**类** ： &quot;mktoString&quot;，
**id**： ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
**mktoName** ：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

可选：
**默认值**：属性的字符串值。 如果未提供，则为空。
**allowHtml**：“true”或“false”。 控制是否打印值而不对HTML进行转义。 如果未设置，则默认为“false”。

基本示例：

`<meta class="mktoString" id="var1" mktoName="My Variable">`

具有所有属性的示例：

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## 颜色 {#color}

必需属性：
**类** ： &quot;mktoColor&quot;，
**id**： ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
**mktoName** ：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

可选：
**默认值**：7位十六进制字符颜色代码。 例如：“#336699”

基本示例：

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

具有所有属性的示例：

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## 布尔值 {#boolean}

必需属性：
**类** ： &quot;mktoBoolean&quot;，
**id**： ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
**mktoName** ：字符串。 这是将显示在登陆页面编辑器中的显示名称。 最佳实践是使用描述性名称。

可选：
**默认值**：布尔字符串。 “true”或“false”控制值是从ON还是OFF位置开始。 &quot;false&quot;（如果未提供）。
**false_value**：字符串。 变量处于OFF位置时要插入的值。 &quot;false&quot;（如果未提供）。
**true_value**：字符串。 当变量处于ON位置时要插入的值。 如果未提供，则为“true”。
**false_value_name**：字符串。 当值处于OFF位置时将在登陆页面编辑器中显示的显示名称。 如果未提供，则为“关”。
**true_value_name**：字符串。 当值处于“开”位置时将在登陆页面编辑器中显示的显示名称。 如果未提供，则为“开”。

基本示例：

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

具有所有属性的示例：

此示例显示了一个常见用例，其中布尔变量通过将css display属性的值设置为“block”或“none”来控制css元素的可见性，从而通过CSS按ID显示/隐藏元素。 登陆页面编辑器将使用显示名称Show/Hide而不是OFF/ON。

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>程序令牌(my.token)还可以在引导式或自由格式登陆页面中的任意位置使用。

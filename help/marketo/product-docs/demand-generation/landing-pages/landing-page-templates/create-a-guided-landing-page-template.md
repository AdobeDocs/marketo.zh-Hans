---
unique-page-id: 7515401
description: 创建引导式登陆页模板- Marketo Docs —— 产品文档
title: 创建引导式登陆页模板
translation-type: tm+mt
source-git-commit: 975e048271dae6a877ae9ff5d39360b159afcc8a
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 0%

---


# 创建引导登陆页模板{#create-a-guided-landing-page-template}

>[!NOTE]
>
>**深潜：** 厌倦阅读？[使用分步](https://youtu.be/3O7e4GdZKsM) 说明观看此精彩视频。

向导式登陆页模板具有特殊的语法。 使用此语法可指定哪些内容可自定义以及内容将最终显示在从模板构建的每个登陆页上的位置。 只有指定为可编辑的区域或变量才能在“向导式”登陆页编辑器中进行自定义。

>[!TIP]
>
>使用良好的命名惯例，您的营销团队将爱上您。

有两种方法可声明页面上的内容应可编辑：

* 将对象声明为“元素”。 登陆页创建者将能够向这些指定区域添加图像、文本或Marketo资产。
* 将字符串声明为“变量”。 登陆页创建器将能够用字符串、颜色或布尔状态替换该变量，该状态来自真／假杠杆。

## 可编辑元素{#editable-elements}

通过向模板添加普通DOM元素，然后使用特定于Marketo的类名装饰元素来声明元素。

## 文本{#text}

如果将区域定义为富文本，则用户将能够使用Marketo的富文本编辑器](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)编辑其内容[。

必需属性：\
**类**:&quot;mktoText&quot;\
**id**:ID字符串。仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。\
**mktoName** :字符串。这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

可选：\
具有mktoText类（如果提供）的元素的内容将用作可编辑区域的默认值。

示例：

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### 图像{#image}

有两个选项可用于定义可编辑的图像元素。 您可以使用`<div>`(它指定将图像插入的容器)或`<img>`标记。

## 选项1 —— 使用 <div> {#option-use-a-div}

必需属性：

类：&quot;mktoImg&quot;\
id:ID字符串。 仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。\
mktoName:字符串。 这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

可选：\
mktoImgClass:字符串。 此处的值将添加到div中`<img>`元素的类属性。

示例：

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## 选项2 —— 使用`<img>` {#option-use-a-img}

必需属性：\
类：&quot;mktoImg&quot;\
id:ID字符串。 仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。\
mktoName:字符串。 这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

可选：\
src:字符串URL。 这将用作图像的默认值。

示例：

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>使用`<img>`版本时，呈现的HTML将包含围绕`<img>`标记生成的div包装器。 将设置为类。”mktoImg.mktoGen”，将显示：inline-block。

## 表单{#form}

示例：必需属性：\
**类**:&quot;mktoForm&quot;\
**id**:ID字符串。仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。\
**mktoName** :字符串。这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## 代码片断{#snippet}

必需属性：\
**类**:&quot;mktoSnippet&quot;\
**id**:ID字符串。仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。\
**mktoName** :字符串。这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

示例：

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## 共享按钮{#share-button}

必需属性：\
**类**:&quot;mktoShareButton&quot;\
**id**:ID字符串。仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。\
**mktoName** :字符串。这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

示例：

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## 视频{#video}

>[!NOTE]
>
>在登陆页中使用视频元素时，Marketo仅支持来自YouTube的视频。 如果您使用其他服务，我们建议使用富文本框并粘贴到视频的嵌入代码中。

必需属性：
**class**:&quot;mktoVideo&quot;
**id**:ID字符串。 仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。
**mktoName** :字符串。这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

示例：

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## 投票{#poll}

必需属性：\
**类**:&quot;mktoPoll&quot;\
**id**:ID字符串。仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。\
**mktoName** :字符串。这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

示例：

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## 推荐{#referral}

必需属性：\
**类**:&quot;mktoReferral&quot;\
**id**:ID字符串。仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。\
**mktoName** :字符串。这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

示例：

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## 抽奖{#sweepstakes}

必需属性：\
**类**:“mktoSweepstakes”\
**id**:ID字符串。仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。\
**mktoName** :字符串。这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

示例：

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## 可编辑变量{#editable-variables}

所有变量类型均通过引用其ID属性值（包含在${ }字符序列中）来使用。 它们可以在文档中的任意位置使用，其他变量声明中除外。

示例：

`<pre data-theme="Confluence">${var1}</pre>`

**声明：**

变量在模板的`<head>`元素中声明为meta标签。 有三种类型的变量可供使用：字符串、颜色和布尔值。

## 字符串{#string}

必需属性：\
**类** :&quot;mktoString&quot;,\
**id**:ID字符串。仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。\
**mktoName** :字符串。这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

可选：\
**默认**:属性的字符串值。如果未提供，则为空。\
**allowHtml**:“true”或“false”。控制是否打印值而不进行HTML转义。 如果取消设置，则默认为“false”。

基本示例：

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

所有属性的示例：

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## 颜色{#color}

必需属性：\
**类** :&quot;mktoColor&quot;,\
**id**:ID字符串。仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。\
**mktoName** :字符串。这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

可选：\
**默认**:7位HEX字符颜色代码。例如：&quot;#336699&quot;

基本示例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

所有属性的示例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## 布尔值{#boolean}

必需属性：\
**类** :&quot;mktoBoolean&quot;,\
**id**:ID字符串。仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。\
**mktoName** :字符串。这是将在登陆页编辑器中显示的显示名称。 最佳实践是使用描述性名称。

可选：\
**默认**:布尔字符串。“true”或“false”控制值是否开始在ON或OFF位置。 如果未提供，则为“false”。\
**false_value**:字符串。变量在OFF位置时要插入的值。 如果未提供，则为“false”。\
**true_value**:字符串。变量在ON位置时要插入的值。 如果未提供，则为“true”。\
**false_value_name**:字符串。值处于“关闭”位置时要在登陆页编辑器中显示的显示名称。 “OFF”（如果未提供）。\
**true_value_name**:字符串。值处于“开启”位置时要在登陆页编辑器中显示的显示名称。 如果未提供，则为“ON”。

基本示例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

所有属性的示例：

此示例显示一个常见用例，布尔变量通过将css显示属性的值设置为“block”或“none”以按CSS的id显示／隐藏元素来控制css元素的可见性。 登陆页编辑器将使用显示名称“显示／隐藏”，而不是“关闭／打开”。

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>项目令牌(my.token)还可以在引导登陆页或自由形式的任意位置使用。

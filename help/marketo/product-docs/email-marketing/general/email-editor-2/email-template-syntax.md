---
unique-page-id: 11371040
description: 电子邮件模板语法- Marketo Docs —— 产品文档
title: 电子邮件模板语法
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '2397'
ht-degree: 0%

---


# 电子邮件模板语法 {#email-template-syntax}

在Marketo的新电子邮件2.0体验中，电子邮件模板由元素、变量、模块或容器的任意组合组成。 每个语法的定义都是向HTML中添加特定于Market的语法。 旧(v1.0)电子邮件模板在电子邮件编辑器2.0中受支持；但是，它们不会包括所有新编辑的功能。

Marketo电子邮件语法仅在模板和单个电子邮件中有效；如果嵌 **入到代** 码片段或富文本令牌中，则它不起作用。

>[!NOTE]
>
>Marketo支持未设置为在CSS/HTML方面提供帮助。 如果您不熟悉CSS/HTML，请咨询您的开发人员。

>[!CAUTION]
>
>包含Marketo语法（即mktoModule、mktoContainer、mktoText）的类值区分大小写。 自定义属性名称（即mktoimgwidth、mktoname）不是。

## Elements {#elements}

元素是您在电子邮件模板中定义为可编辑的内容区域。 元素的编辑体验是其类型特有的，优惠是处理内容的简单方式。 电子邮件模板中可能包含的元素包括：

* 富文本
* 图像
* 代码片段
* 视频

## 富文本 {#rich-text}

如果将区域定义为富文本，则用户将能够使用Marketo的富文 [本编辑器编辑其内容](../../../../product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)。 在电子邮件模板中定义富文本元素有两种方法：mktEditable和mktoText。 请记住，富文本元素始终可以从电子邮件编辑器中转换为片段。

### 选项1 - mktEditable {#option-mkteditable}

由于电子邮件编辑器2.0向后兼容，因此某些旧电子邮件模板可能会通过在任何HTML元素上添加class=&quot;mktEditable&quot;来指定富文本元素。 这仍受支持，元素的ID将用作电子邮件编辑器中的显示名称。

必需属性

* **类**:“mktEditable”。
* **id**:ID字符串。 仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。

可选属性

* **mktoName** :字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。

默认值

HTML元素（如果提供）中的class=&quot;mktEditable&quot;内容将用作富文本元素的默认值。

示例：

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### 选项2 - mktoText {#option-mktotext}

建议使用class=&quot;mktoText&quot;语法指定富文本元素。 这可确保元素始终具有正确的显示名称。

必需属性

* **类**:&quot;mktoText&quot;
* **id**:ID字符串。 仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。
* **mktoName** :字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。

默认值

HTML元素（如果提供）中的class=&quot;mktoText&quot;内容将用作富文本元素的默认值。

示例：

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## 图像 {#images}

有两个选项可用于定义可编辑的图像元素。 您可以使用 `<div>`指定将插入的容器 `<img>` 的标记或标 `<img>` 记。 如果您希望最终用户只需选择一个将返回图像URL的图像（与DOM相对），请参阅下面部分中的“图像变量”。 以下两个选项将插入一个HTML `<img>` 元素。

### 选项1 —— 使用\&lt;div\> {#option-use-a-div}

必需属性

* **类：** “mktoImg”。
* **id:** ID字符串。 仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。
* **mktoName:** 字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。

可选属性

* **mktoImgClass:** 字符串。 此处的值将添加到div中元素 `<img>` 的类属性。
* **mktoImgSrc:** 用作此div中放置的图像的默认值。 如果省略此项，则使用占位符。
* **mktoImgLink:** 指示应 `<img>` 该由带有此目 `<a>` 标URL的标记所环绕。 用户可以在电子邮件编辑器中更改此设置。
* **mktoImgLinkTarget:** 指示mktoImgLink `<a>` 属性中的标记应使用此目标。 如果同时未使用mktoImgLink，则无效。
* **mktoImgWidth:** 用作封闭的宽度 `<img>`。
* **mktoImgHeight:** 用作封闭的高度 `<img>`。
* **mktoLockImgSize:** 用于解锁元 `<img>` 素的height和width属性，以便最终用户可以修改（如果省略，则默认值为true）。
* **mktoLockImgStyle:** 用于锁定元 `<img>` 素的样式属性（默认为false）。

默认值（可选）

**`<img>`**:要用作要放 `<img>` 置图像的元素。 如果要向图像添加内联样式，则此功能非常有用。 请记住要包 `<a> </a>` 含周围的标记，因此，如果用户添加链接，您的样式将不会被去除！

示例：

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="http://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### 选项2 —— 使用\&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>此选项不允许最终用户添加指向其图像的链接。 如果这对模板很重要，请使用选项1。

必需属性

* **类：** “mktoImg”。
* **id:** ID字符串。 仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。
* **mktoName:** 字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。  默认值（可选）
* **src:** 用作图像的默认值。 如果省略此项，则使用占位符。
* **mktoLockImgSize:** 用于解锁元 `<img>` 素的height和width属性，以便最终用户可以修改（如果省略，则默认值为true）。
* **mktoLockImgStyle:** 用于锁定元 `<img>` 素的样式属性（默认为false）。

示例：
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## 代码片段 {#snippets}

如果您将某个区域定义为“代码片断”，最终用户将能够选择要 [](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)在此区域中插入的已批准的片段。 尽管富文本元素可以从电子邮件编辑器中转换为片段，但当您将某个区域专门定义为片段时，它将无法转换为富文本。 您可以使用类=&quot;mktoSnippet&quot; `<div>` 指定代码片断区域

必需属性

* **id:** ID字符串。 仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。
* **mktoName:** 字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。

默认值（可选）

**mktoDefaultSnippetId**:默认情况下应显示的Marketo代码片断的数字ID（仅当具有该ID的代码片断存在且在该工作区中获得批准时才有效）。

示例：

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## 视频 {#video}

如果您将区域定义为视频，最终用户将能够在电子邮件中插入YouTube或Vimeo URL，该URL将作为缩略图（带有“播放”按钮）显示。 您可以使用类=&quot;mktoVideo&quot; `<div>` 指定视频区域

必需属性

* **id:** ID字符串。 仅包含字母、数字、短划线“-”和下划线“_”。 不允许使用空格。 必须是唯一的。
* **mktoName:** 字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。

可选属性

* **mktoImgClass:** 字符串。 此处的值将添加到div中视频缩略图的 `<img>` 类属性。

示例：

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## 变量 {#variables}

变量与令牌类似。 您首先使用标记在电 `<head>` 子邮件模板的部分中定 `<meta>` 义这些标记，然后在整个模板中按所需次数使用它们。 由于模板中定义了这些值，因此最终用户将能够根据自己的规则修改其值。 请注意，您可以将变量定义为范围中的局部或全局变量。 如果您在“模块”中使用变量（见下文），并且最终用户重复了该模块，则本地变量将具有独立值，而全局变量将应用于这两个模块。

## 字符串 {#string}

如果将变量指定为“字符串”，则最终用户将能够在电子邮件编辑器的文本框中输入文本。 使用class=&quot;mktoString&quot; `<meta>` 指定字符串变量

必需属性

* **id:** 您在电子邮件模板中引用变量的方式。
* **mktoName:** 字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。

可选属性

* **allowHTML:** 布尔值。 控制变量的值是否为HTML转义。 如果省略，则默认为False。
* **默认**:字符串的默认值。 如果省略，则为空。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，变量是局部(true)还是全局(false)。 如果省略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

示例用法：

`<pre data-theme="Confluence">${textHeader}</pre>`

## 列表 {#list}

如果将变量指定为列表，则最终用户将能够从您在电子邮件编辑器中定义的一组值中进行选择。 您使用类=&quot;mktoList `<meta>` &quot;指定列表变量

必需属性

* **id**:您在电子邮件模板中引用变量的方式。
* **mktoName:** 字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。
* **值：** 以逗号分隔的值列表。 必须至少有一个字符串。

可选属性

* **默认：** 选择下拉列表的默认值。 如果省略，则使用“values”属性中的第一个值。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，变量是局部(true)还是全局(false)。 如果省略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

示例用法：

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## 数字 {#number}

如果将变量指定为数字，则最终用户将能够在电子邮件编辑器中输入数字。 使用class=&quot;mktoNumber&quot; `<meta>` 指定一个Number变量

必需属性

* **id**:您在电子邮件模板中引用变量的方式。
* **mktoName**:字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。
* **默认：** 变量的默认数值。

可选属性

* **分钟：** 可接受的最小值。
* **max:** 最大可接受值。
* **单位：** 要附加到数字值的单位(例如：px、pt、em等) 显示在电子邮件编辑器中以及生成的代码中。
* **步骤：** 数字变量应增加／减少多少个单位（0.1、1、10等）。 如果省略，则默认为1。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，变量是局部(true)还是全局(false)。 如果省略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

示例用法：

`<pre data-theme="Confluence">${textFontSize}</pre>`

## 颜色 {#color}

如果将变量指定为“颜色”，则最终用户将能够输入十六进制颜色值或从电子邮件编辑器中的拾色器选择颜色。 使用类=&quot;mktoColor&quot; `<meta>` 指定颜色变量

必需属性

* **id**:您在电子邮件模板中引用变量的方式。
* **mktoName**:字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。

可选属性

* **默认：** 颜色的默认值。 6位十六进制颜色代码。 例如：#ffffff。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，变量是局部(true)还是全局(false)。 如果省略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

示例用法：

`<pre data-theme="Confluence">${textColor}</pre>`

## 布尔值 {#boolean}

如果将变量指定为布尔值，则最终用户将能够在电子邮件编辑器中打开／关闭该选项。 您使用类=&quot;mktoBoolean `<meta>` &quot;指定布尔变量

必需属性

* **id**:您在电子邮件模板中引用变量的方式。
* **mktoName**:字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。

可选属性

* **默认：** 确定切换开关的默认状态的布尔值。 如果省略，则为false。
* **false_value:** 在切换处于“关闭”位置时要插入的值。 如果省略，则为false。
* **true_value:** 在切换处于开启位置时要插入的值。 如果省略，则返回true。
* **false_value_name:** 处于关闭位置时，切换中显示的UI。 如果省略，则为false。
* **true_value_name:** UI在处于开启位置时在切换中显示。 如果省略，则返回true。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，变量是局部(true)还是全局(false)。 如果省略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

示例用法：

`<pre data-theme="Confluence">${showFooter}</pre>`

## HTML块 {#html-block}

如果将变量指定为HTML块，则最终用户将能够从电子邮件编辑器中逐字输入HTML。 使用class=&quot;mktoHTML&quot; `<meta>` 指定HTML块变量

必需属性

* **id**:您在电子邮件模板中引用变量的方式。
* **mktoName**:字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。

可选属性

* **默认：** HTML编码值用作块的默认内容。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，变量是局部(true)还是全局(false)。 如果省略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

示例用法：

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## 图像变量 {#image-variable}

如果将变量指定为图像，则最终用户将能够从电子邮件编辑器中的图像选取器中选择图像。 所选图像URL将是变量的值。 使用class=&quot;mktoImg&quot; `<meta>` 指定图像变量

必需属性

* **id**:您在电子邮件模板中引用变量的方式。
* **mktoName**:字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。

可选属性

* **默认：** 元素的默认图像URL。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，变量是局部(true)还是全局(false)。 如果省略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="http://www.company.com/image.jpg"></pre>`

示例用法：

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## 模块 {#modules}

模块是在模板级别定义的模板化部分，将显示给最终用户将其插入其电子邮件。 由于您已预建了这些模块，因此您可以确保它们能够以完全响应式方式与其余电子邮件内容正常交互。 只能将模块放入容器。

**对于容器类 `<table>`型 `<tbody>`、、 `<thead>`或 `<tfoot>`:**

使用 `<tr>` class=&quot;mktoModule&quot;指定

**对于容器类 `<td>`型：**

使用 `<table>` class=&quot;mktoModule&quot;指定

必需属性

* **id**:您如何在电子邮件模板中引用模块。
* **mktoName**:字符串。 这是将在电子邮件编辑器2.0中显示的显示名称。最佳实践是使用描述性名称。

可选属性

* **mktoActive:** 确定此模块是否显示在电子邮件编辑器中的模块列表中。 默认值为true。 如果为false，则最终用户无法将模块添加到电子邮件。
* **mktoAddByDefault:** 确定此模块是否将位于创建时使用此模板的新电子邮件的画布中。 默认值为true（如果mktoActive为false，则忽略此值）。

>[!NOTE]
>
>**提醒**
>
>包含Marketo语法（即mktoModule、mktoContainer、mktoText）的类值区分大小写。 自定义属性名称（即mktoimgwidth、mktoname）不是。

## 容器 {#containers}

容器保存模块并定义可放置模块的位置。 当最终用户重新订购模块并将其插入其电子邮件时，容器会控制他们可能去的位置。

**使用 `<table>`、 `<tbody>`、 `<thead>`或 `<tfoot>` 与class= `<td>` &quot;mktoContainer&quot;指定**

必需属性

**id**:您如何在电子邮件模板中引用模块。

>[!CAUTION]
>
>容器只能包含模块——如果存在其他任何模块，则容器被视为无效！ 每个模板只允许一个容器。

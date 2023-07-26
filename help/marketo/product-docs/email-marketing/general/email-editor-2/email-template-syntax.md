---
unique-page-id: 11371040
description: 电子邮件模板语法 — Marketo文档 — 产品文档
title: 电子邮件模板语法
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '2423'
ht-degree: 0%

---

# 电子邮件模板语法 {#email-template-syntax}

在Marketo的新Email 2.0 Experience中，电子邮件模板由元素、变量、模块或容器的任意组合组成。 每个规则都是通过向HTML添加特定于Marketo的语法来定义的。 电子邮件编辑器2.0支持旧的(v1.0)电子邮件模板；但是，这些模板不会包含新编辑器的所有功能。

Marketo电子邮件语法仅在模板和单个电子邮件中起作用；它有效 **非** 如果嵌入到代码片段或富文本令牌中，则有效。

>[!NOTE]
>
>Marketo支持未设置为协助进行CSS/HTML。 如果您不熟悉CSS/HTML，请咨询您的开发人员。

>[!CAUTION]
>
>包含Marketo语法的类值（即mktoModule、mktoContainer、mktoText）区分大小写。 自定义属性名称（即mktoimgwidth、mktoname）无效。

## 元素 {#elements}

元素是您在电子邮件模板中定义为可编辑的内容区域。 元素的编辑体验因类型而异，它提供了一种处理内容的简单方法。 可以包含在电子邮件模板中的可能元素包括：

* 富文本
* 图像
* 代码片段
* 视频

## 富文本 {#rich-text}

如果将区域定义为富文本，则用户将能够编辑其内容 [使用Marketo富文本编辑器](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). 可通过两种方式在电子邮件模板中定义富文本元素：mktEditable和mktoText。 请记住，富文本元素始终可以在电子邮件编辑器中转换为代码片段。

### 选项1 - mktEditable {#option-mkteditable}

由于电子邮件编辑器2.0向后兼容，因此某些旧电子邮件模板可以通过在任何HTML元素上添加class=&quot;mktEditable&quot;来指定富文本元素。 这仍受支持，并且元素的ID将成为电子邮件编辑器中的显示名称。

必需属性

* **类**：“mktEditable”。
* **id**： ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。

可选属性

* **mktoName** ：字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。

默认值

HTML元素（如果提供）中具有class=&quot;mktEditable&quot;的内容将用作富文本元素的默认值。

示例：

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### 选项2 - mktoText {#option-mktotext}

建议使用class=&quot;mktoText&quot;语法指定富文本元素。 这可确保元素始终具有正确的显示名称。

必需属性

* **类**：“mktoText”
* **id**： ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
* **mktoName** ：字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。

默认值

HTML元素（如果提供）中具有class=&quot;mktoText&quot;的内容将用作富文本元素的默认值。

示例：

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## 图像 {#images}

有两个选项可用于定义可编辑的图像元素。 您可以使用 `<div>`，指定容器，该容器 `<img>` 将被插入到，或者 `<img>` 标记之前。 如果您打算让最终用户只选取将返回图像URL（而不是DOM）的图像，请参阅以下部分中的“图像变量”。 以下两个选项将插入HTML `<img>` 元素。

### 选项1 — 使用 `<div>` {#option-use-a-div}

必需属性

* **class：** “mktoImg”。
* **id：** ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
* **mktoName ：** 字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。

可选属性

* **mktoImgClass：** 字符串。 此处的值将添加到的 `<img>` div中的元素。
* **mktoImgSrc：** 用作放置在此div中的图像的默认值。 如果忽略此项，则使用占位符。
* **mktoImgLink：** 指示 `<img>` 应该由 `<a>` 标记对应的目标URL。 用户可以在电子邮件编辑器中更改此设置。
* **mktoImgLinkTarget：** 指示 `<a>` mktoImgLink属性中的标记应使用此目标。 如果未同时使用mktoImgLink，则不起作用。
* **mktoImgWidth：** 用作所包含内容的宽度 `<img>`.
* **mktoImgHeight：** 用作所包含的高度 `<img>`.
* **mktoLockImgSize：** 用于解锁 `<img>` 元素的height和width属性，以便最终用户进行修改（如果忽略，则默认为true）。
* **mktoLockImgStyle：** 用于锁定 `<img>` 元素的样式属性（默认值为false）。

默认值（可选）

**`<img>`**：用作 `<img>` 将放置图像的元素。 如果要向图像添加内联样式，则此选项非常有用。 请记住要包含周围 `<a> </a>` 标记，因此如果用户添加链接，则不会去除您的样式！

示例：

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### 选项2 — 使用\&lt;img> {#option-use-an-img}

>[!NOTE]
>
>此选项不允许最终用户向其图像添加链接。 如果对模板很重要，请使用选项1。

必需属性

* **class：** “mktoImg”。
* **id：** ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
* **mktoName：** 字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。  默认值（可选）
* **src：** 用作图像的默认值。 如果忽略此项，则使用占位符。
* **mktoLockImgSize：** 用于解锁 `<img>` 元素的height和width属性，以便最终用户进行修改（如果忽略，则默认为true）。
* **mktoLockImgStyle：** 用于锁定 `<img>` 元素的样式属性（默认值为false）。

示例：
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## 代码片段 {#snippets}

如果您将区域定义为代码片段，最终用户将能够选择已批准的区域 [代码片段](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)他们想插进这个地区。 尽管富文本元素可以在电子邮件编辑器中转换为代码片段，但如果您将某个区域专门定义为代码片段，则无法将该区域转换为富文本。 您可以使用指定代码片段区域 `<div>` with class=&quot;mktoSnippet&quot;

必需属性

* **id：** ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
* **mktoName：** 字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。

默认值（可选）

**mktoDefaultSnippetId**：默认显示的Marketo代码片段的数字ID（只有存在具有该ID的代码片段并且在该工作区中获得批准时，该ID才有效）。

示例：

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## 视频 {#video}

如果将区域定义为视频，则最终用户能够插入将作为缩略图图像（带有“播放”按钮）显示在电子邮件中的YouTube或Vimeo URL。 您可以使用指定 `<div>` with class=&quot;mktoVideo&quot;

必需属性

* **id：** ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许使用空格。 必须是唯一的。
* **mktoName：** 字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。

可选属性

* **mktoImgClass：** 字符串。 此处的值将添加到视频缩略图的类属性中 `<img>` 在div中。

示例：

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## 变量 {#variables}

变量就像令牌一样。 您首先在 `<head>` 使用的电子邮件模板部分 `<meta>` 标记后，可在整个模板中根据需要多次使用它们。 由于在模板中定义了这些值，因此最终用户能够根据其规则修改其值。 请注意，您可以在范围内将变量定义为局部或全局变量。 如果在“模块”中使用变量（见下文），并且最终用户复制了该模块，则局部变量将具有独立的值，而全局变量将应用于这两个模块。

## 字符串 {#string}

如果将变量指定为字符串，最终用户将能够在电子邮件编辑器的文本框中输入文本。 使用以下方式指定字符串变量 `<meta>` with class=&quot;mktoString&quot;

必需属性

* **id：** 如何在电子邮件模板中引用变量。
* **mktoName：** 字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。

可选属性

* **allowHTML：** 布尔型。 控制变量的值是否进行HTML转义。 如果忽略，则默认为False。
* **默认**：字符串的默认值。 如果省略，则留空。
* **mktoModuleScope**：布尔值。 控制变量在模块中使用时是局部(true)还是全局(false)。 如果忽略，则默认为False。

声明示例：

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

用法示例：

`<pre data-theme="Confluence">${textHeader}</pre>`

## 列表 {#list}

如果将变量指定为List ，最终用户将能够从您在电子邮件编辑器中定义的一组值中进行选择。 使用以下方式指定列表变量 `<meta>` with class=&quot;mktoList&quot;

必需属性

* **id**：如何在电子邮件模板中引用变量。
* **mktoName：** 字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。
* **值：** 逗号分隔的值列表。 必须至少有一个字符串。

可选属性

* **默认：** 选择下拉列表的默认值。 如果忽略，则使用“values”属性中的第一个值。
* **mktoModuleScope**：布尔值。 控制变量在模块中使用时是局部(true)还是全局(false)。 如果忽略，则默认为False。

声明示例：

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

用法示例：

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## 数字 {#number}

如果指定一个变量作为数字，最终用户将能够在电子邮件编辑器中输入数字。 使用以下方式指定数字变量 `<meta>` with class=&quot;mktoNumber&quot;

必需属性

* **id**：如何在电子邮件模板中引用变量。
* **mktoName**：字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。
* **默认：** 变量的默认数值。

可选属性

* **最小值：** 可接受的最小值。
* **最大：** 接受的最大值。
* **件数：** 附加到数字值的单位（例如：px、pt、em等） 在电子邮件编辑器中显示时以及在生成的代码中显示。
* **步骤：** 数量变量应增加/减少的单位数量（0.1、1、10等）。 如果忽略，则默认为1。
* **mktoModuleScope**：布尔值。 控制变量在模块中使用时是局部(true)还是全局(false)。 如果忽略，则默认为False。

声明示例：

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

用法示例：

`<pre data-theme="Confluence">${textFontSize}</pre>`

## 颜色 {#color}

如果将变量指定为“颜色”，最终用户将能够输入十六进制颜色值，或从电子邮件编辑器中的拾色器中选择颜色。 使用以下方式指定颜色变量 `<meta>` with class=&quot;mktoColor&quot;

必需属性

* **id**：如何在电子邮件模板中引用变量。
* **mktoName**：字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。

可选属性

* **默认：** 颜色的默认值。 6位十六进制颜色代码。 例如： #ffffff。
* **mktoModuleScope**：布尔值。 控制变量在模块中使用时是局部(true)还是全局(false)。 如果忽略，则默认为False。

声明示例：

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

用法示例：

`<pre data-theme="Confluence">${textColor}</pre>`

## 布尔值 {#boolean}

如果指定变量作为布尔值，最终用户将能够在电子邮件编辑器中打开/关闭该选项。 使用以下方式指定布尔变量 `<meta>` with class=&quot;mktoBoolean&quot;

必需属性

* **id**：如何在电子邮件模板中引用变量。
* **mktoName**：字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。

可选属性

* **默认：** 确定切换开关的默认状态的布尔值。 如果省略，则返回False。
* **false_value：** 切换开关处于“关闭”位置时要插入的值。 如果省略，则返回False。
* **true_value：** 切换开关处于“开”位置时要插入的值。 如果忽略，则返回True。
* **false_value_name：** 当处于关闭位置时，会在切换中显示用户界面。 如果省略，则返回False。
* **true_value_name：** 当处于开启位置时，切换开关中显示UI。 如果忽略，则返回True。
* **mktoModuleScope**：布尔值。 控制变量在模块中使用时是局部(true)还是全局(false)。 如果忽略，则默认为False。

声明示例：

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

用法示例：

`<pre data-theme="Confluence">${showFooter}</pre>`

## HTML块 {#html-block}

如果指定变量作为HTML块，最终用户将能够在电子邮件编辑器中输入逐字HTML。 使用以下方式指定HTML块变量 `<meta>` with class=&quot;mktoHTML&quot;

必需属性

* **id**：如何在电子邮件模板中引用变量。
* **mktoName**：字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。

可选属性

* **默认：** HTML编码值，用作块的默认内容。
* **mktoModuleScope**：布尔值。 控制变量在模块中使用时是局部(true)还是全局(false)。 如果忽略，则默认为False。

声明示例：

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

用法示例：

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## 图像变量 {#image-variable}

如果指定变量作为图像，最终用户将能够从电子邮件编辑器中的图像选择器中选择图像。 选定的图像URL将是变量的值。 使用以下方式指定图像变量 `<meta>` with class=&quot;mktoImg&quot;

必需属性

* **id**：如何在电子邮件模板中引用变量。
* **mktoName**：字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。

可选属性

* **默认：** 元素的默认图像URL。
* **mktoModuleScope**：布尔值。 控制变量在模块中使用时是局部(true)还是全局(false)。 如果忽略，则默认为False。

声明示例：

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

用法示例：

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## 模块 {#modules}

模块是在模板级别定义的模板化部分，最终用户将看到这些模板化部分插入其电子邮件。 由于您已预建这些模块，因此您可以确保它们将以完全响应的方式与您的其余电子邮件内容正常交互。 您只能在容器中放入模块。

>[!IMPORTANT]
>
>从包含已定义模块组件的电子邮件模板生成电子邮件时，对模板模块所做的任何更改都将 **非** 被推送到那封电子邮件里。

**对于类型为的容器 `<table>`， `<tbody>`， `<thead>`，或 `<tfoot>`：**

使用指定 `<tr>` with class=&quot;mktoModule&quot;

**对于类型为的容器 `<td>`：**

使用指定 `<table>` with class=&quot;mktoModule&quot;

必需属性

* **id**：如何在电子邮件模板中引用模块。
* **mktoName**：字符串。 这是将显示在电子邮件编辑器2.0中的显示名称。最佳实践是使用描述性名称。

可选属性

* **mktoActive：** 确定此模块是否显示在电子邮件编辑器的模块列表中。 默认为true。 如果为false，则最终用户无法将模块添加到电子邮件。
* **mktoAddByDefault：** 确定此模块是否将在创建时使用此模板的新电子邮件的画布中。 默认值为true（如果mktoActive为false，则忽略此值）。

>[!NOTE]
>
>包含Marketo语法的类值（即mktoModule、mktoContainer、mktoText）区分大小写。 自定义属性名称（即mktoimgwidth、mktoname）无效。

## 容器 {#containers}

容器包含模块并定义模块的放置位置。 当最终用户重新订购模块并将模块插入其电子邮件时，容器会控制他们可能前往的位置。

**使用以下任一方式指定 `<table>`， `<tbody>`， `<thead>`， `<tfoot>` 或 `<td>` with class=&quot;mktoContainer&quot;**

必需属性

**id**：如何在电子邮件模板中引用模块。

>[!CAUTION]
>
>容器只能包含模块 — 如果存在其他内容，则将容器视为无效！ 每个模板只允许一个容器。

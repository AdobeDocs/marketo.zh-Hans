---
unique-page-id: 11371040
description: 电子邮件模板语法 — Marketo文档 — 产品文档
title: 电子邮件模板语法
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
source-git-commit: a59b6b2505c6e5a83c6137a1925aa4e60e56eac8
workflow-type: tm+mt
source-wordcount: '2423'
ht-degree: 0%

---

# 电子邮件模板语法 {#email-template-syntax}

在Marketo的新Email 2.0体验中，电子邮件模板由元素、变量、模块或容器的任意组合组成。 每个变量的定义方式是向HTML添加特定于Marketo的语法。 Email Editor 2.0支持旧(v1.0)电子邮件模板；但是，它们不会包含所有新编辑器功能。

Marketo电子邮件语法仅适用于模板和单个电子邮件；是 **not** 如果嵌入在代码片段或富文本令牌中，则可以正常工作。

>[!NOTE]
>
>Marketo支持未设置为协助处理CSS/HTML。 如果您不熟悉CSS/HTML，请咨询您的开发人员。

>[!CAUTION]
>
>包含Marketo语法的类值（例如mktoModule、mktoContainer、mktoText）区分大小写。 自定义属性名称（即mktoimgwidth、mktoname）不会。

## 元素 {#elements}

元素是您在电子邮件模板中定义为可编辑的内容区域。 元素的编辑体验因其类型而异，提供了一种处理内容的简单方法。 电子邮件模板中可能包含的元素包括：

* 富文本
* 图像
* 代码片段
* 视频

## 富文本 {#rich-text}

如果将区域定义为富文本，则用户将能够编辑其内容 [使用Marketo的富文本编辑器](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). 在电子邮件模板内，可通过两种方式定义富文本元素：mktEditable和mktoText。 请记住，富文本元素始终可以在电子邮件编辑器中转换为代码片段。

### 选项1 - mktEditable {#option-mkteditable}

由于电子邮件编辑器2.0向后兼容，因此某些旧电子邮件模板可能会通过在任何HTML元素中添加class=&quot;mktEditable&quot;来指定富文本元素。 此功能仍受支持，元素的ID将用作电子邮件编辑器中的显示名称。

必需属性

* **类**:&quot;mktEditable&quot;。
* **id**:ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许有空格。 必须唯一。

可选属性

* **mktoName** :字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。

默认值

HTML元素（如果提供）中具有class=&quot;mktEditable&quot;的内容将用作富文本元素的默认值。

示例：

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### 选项2 - mktoText {#option-mktotext}

建议使用class=&quot;mktoText&quot;语法指定富文本元素。 这可确保元素始终具有正确的显示名称。

必需属性

* **类**:&quot;mktoText&quot;
* **id**:ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许有空格。 必须唯一。
* **mktoName** :字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。

默认值

HTML元素（如果提供）中具有class=&quot;mktoText&quot;的内容将用作富文本元素的默认值。

示例：

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## 图像 {#images}

有两个选项可用于定义可编辑的图像元素。 您可以使用 `<div>`，它指定一个容器， `<img>` 将插入到中，或 `<img>` 标记。 如果您打算让最终用户只需选取一个将返回图像URL（而不是DOM）的图像，请参阅下面部分的“图像变量”。 以下两个选项将插入一个HTML `<img>` 元素。

### 选项1 — 使用 `<div>` {#option-use-a-div}

必需属性

* **类：** “mktoImg”。
* **id:** ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许有空格。 必须唯一。
* **mktoName :** 字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。

可选属性

* **mktoImgClass:** 字符串。 此处的值将添加到的类属性中 `<img>` div内的元素。
* **mktoImgSrc:** 用作此div中放置的图像的默认值。 如果忽略此设置，则使用占位符。
* **mktoImgLink:** 指示 `<img>` 应被 `<a>` 标记。 用户可以在电子邮件编辑器中更改此设置。
* **mktoImgLinkTarget:** 指示 `<a>` mktoImgLink属性中的标记应使用此目标。 如果不同时使用mktoImgLink，则不起作用。
* **mktoImgWidth:** 用作封闭的 `<img>`.
* **mktoImgHeight:** 用作封闭的 `<img>`.
* **mktoLockImgSize:** 用于解锁 `<img>` 元素的height和width属性，以便最终用户可以修改（如果忽略，则默认为true）。
* **mktoLockImgStyle:** 用于锁定 `<img>` 元素的样式属性（默认值为false）。

默认值（可选）

**`<img>`**:用作 `<img>` 元素。 当您想要向图像添加内联样式时，此变量非常有用。 请记住包含周围 `<a> </a>` 标记，因此如果用户添加链接，将不会剥夺您的样式！

示例：

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### 选项2 — 使用\&lt;img> {#option-use-an-img}

>[!NOTE]
>
>此选项不允许最终用户添加指向其图像的链接。 如果这对模板很重要，请使用选项1。

必需属性

* **类：** “mktoImg”。
* **id:** ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许有空格。 必须唯一。
* **mktoName:** 字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。  默认值（可选）
* **src:** 用作图像的默认值。 如果忽略此设置，则使用占位符。
* **mktoLockImgSize:** 用于解锁 `<img>` 元素的height和width属性，以便最终用户可以修改（如果忽略，则默认为true）。
* **mktoLockImgStyle:** 用于锁定 `<img>` 元素的样式属性（默认值为false）。

示例：
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## 代码片段 {#snippets}

如果您将区域定义为代码片段，则最终用户将能够选择批准的区域 [代码片段](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)他们想在这个地区插入。 虽然富文本元素可以在电子邮件编辑器中转换为片段，但是当您将区域专门定义为代码片段时，它无法转换为富文本。 您可以使用 `<div>` with class=&quot;mktoNippet&quot;

必需属性

* **id:** ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许有空格。 必须唯一。
* **mktoName:** 字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。

默认值（可选）

**mktoDefaultDippletId**:默认情况下应显示的Marketo代码片段的数字ID（仅当存在具有该ID的代码片段并在该工作区中获得批准时，才可使用）。

示例：

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## 视频 {#video}

如果将区域定义为“视频”，则最终用户将能够在电子邮件中插入YouTube或Vimeo URL，该URL将作为缩略图（使用“播放”按钮）显示。 您可以使用 `<div>` with class=&quot;mktoVideo&quot;

必需属性

* **id:** ID字符串。 仅包含字母、数字、短划线“ — ”和下划线“_”。 不允许有空格。 必须唯一。
* **mktoName:** 字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。

可选属性

* **mktoImgClass:** 字符串。 此处的值将添加到视频缩略图的类属性中 `<img>` div内。

示例：

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## 变量 {#variables}

变量与令牌类似。 首先，在 `<head>` 部分 `<meta>` 标记，则可以在整个模板中根据需要多次使用这些标记。 由于它们是在模板中定义的，因此最终用户将能够根据其规则修改其值。 请注意，您可以在范围中将变量定义为本地或全局变量。 如果您在“模块”中使用变量（请参阅下文），并且最终用户复制了该模块，则本地变量将具有独立值，而全局变量将应用于这两个模块。

## 字符串 {#string}

如果将变量指定为字符串，则最终用户将能够在电子邮件编辑器的文本框中输入文本。 您可以使用 `<meta>` with class=&quot;mktoString&quot;

必需属性

* **id:** 如何在电子邮件模板中引用变量。
* **mktoName:** 字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。

可选属性

* **allowHTML:** 布尔值。 控制变量的值是否进行HTML转义。 如果忽略，则默认为False。
* **默认**:字符串的默认值。 如果忽略，则为空。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，该变量是局部变量(true)还是全局变量(false)。 如果忽略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

用法示例：

`<pre data-theme="Confluence">${textHeader}</pre>`

## 列表 {#list}

如果将变量指定为列表，则最终用户将能够从您在电子邮件编辑器中定义的一组值中进行选择。 您可以使用 `<meta>` with class=&quot;mktoList&quot;

必需属性

* **id**:如何在电子邮件模板中引用变量。
* **mktoName:** 字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。
* **值：** 以逗号分隔的值列表。 必须至少包含一个字符串。

可选属性

* **默认：** 选择下拉菜单的默认值。 如果忽略，则使用“values”属性的第一个值。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，该变量是局部变量(true)还是全局变量(false)。 如果忽略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

用法示例：

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## 数字 {#number}

如果将变量指定为数字，则最终用户将能够在电子邮件编辑器中输入数字。 您可以使用 `<meta>` with class=&quot;mktoNumber&quot;

必需属性

* **id**:如何在电子邮件模板中引用变量。
* **mktoName**:字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。
* **默认：** 变量的默认数值。

可选属性

* **最小：** 可接受的最小值。
* **最大：** 最大接受值。
* **件数：** 要附加到数字值的单位(例如：px、pt、em等) 显示在电子邮件编辑器中时，以及在生成的代码中。
* **步骤：** 数字变量应增加/减少的单位数（0.1、1、10等）。 如果忽略，则默认为1。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，该变量是局部变量(true)还是全局变量(false)。 如果忽略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

用法示例：

`<pre data-theme="Confluence">${textFontSize}</pre>`

## 颜色 {#color}

如果将变量指定为“颜色”，则最终用户将能够输入十六进制颜色值，或从电子邮件编辑器的拾色器中选择颜色。 您可以使用 `<meta>` with class=&quot;mktoColor&quot;

必需属性

* **id**:如何在电子邮件模板中引用变量。
* **mktoName**:字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。

可选属性

* **默认：** 颜色的默认值。 6位十六进制颜色代码。 例如：#ffffff。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，该变量是局部变量(true)还是全局变量(false)。 如果忽略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

用法示例：

`<pre data-theme="Confluence">${textColor}</pre>`

## 布尔值 {#boolean}

如果将变量指定为布尔值，则最终用户将能够在电子邮件编辑器中打开/关闭选项。 使用 `<meta>` with class=&quot;mktoBoolean&quot;

必需属性

* **id**:如何在电子邮件模板中引用变量。
* **mktoName**:字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。

可选属性

* **默认：** 确定切换开关默认状态的布尔值。 如果忽略，则为False。
* **false_value:** 切换位置为“关闭”位置时要插入的值。 如果忽略，则为False。
* **true_value:** 切换位置为“开”位置时要插入的值。 如果忽略，则为True。
* **false_value_name:** 当处于“关闭”位置时，切换开关中会显示UI。 如果忽略，则为False。
* **true_value_name:** 当处于“开启”位置时，切换开关中会显示UI。 如果忽略，则为True。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，该变量是局部变量(true)还是全局变量(false)。 如果忽略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

用法示例：

`<pre data-theme="Confluence">${showFooter}</pre>`

## HTML块 {#html-block}

如果将变量指定为HTML块，则最终用户将能够在电子邮件编辑器中输入逐字HTML。 您可以使用 `<meta>` 与class=&quot;mktoHTML&quot;

必需属性

* **id**:如何在电子邮件模板中引用变量。
* **mktoName**:字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。

可选属性

* **默认：** HTML编码值用作块的默认内容。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，该变量是局部变量(true)还是全局变量(false)。 如果忽略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

用法示例：

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## 图像变量 {#image-variable}

如果将变量指定为“图像”，则最终用户将能够从电子邮件编辑器的图像选取器中选择图像。 所选图像URL将是变量的值。 您可以使用 `<meta>` with class=&quot;mktoImg&quot;

必需属性

* **id**:如何在电子邮件模板中引用变量。
* **mktoName**:字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。

可选属性

* **默认：** 元素的默认图像URL。
* **mktoModuleScope**:布尔值。 控制在模块中使用变量时，该变量是局部变量(true)还是全局变量(false)。 如果忽略，则默认为False。

示例声明：

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

用法示例：

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## 模块 {#modules}

模块是在模板级别定义的模板化部分，将显示给最终用户以插入其电子邮件。 由于您已预先构建了这些模块，因此您可以确保它们能够与电子邮件内容的其余部分（以完全响应的方式）正常交互。 您只能将模块放入容器中。

>[!IMPORTANT]
>
>从包含已定义模块组件的电子邮件模板生成电子邮件时，对模板模块所做的任何更改都将 **not** 被推送到上述电子邮件。

**对于类型的容器 `<table>`, `<tbody>`, `<thead>`或 `<tfoot>`:**

使用指定 `<tr>` with class=&quot;mktoModule&quot;

**对于类型的容器 `<td>`:**

使用指定 `<table>` with class=&quot;mktoModule&quot;

必需属性

* **id**:如何在电子邮件模板中引用模块。
* **mktoName**:字符串。 这是将在Email Editor 2.0中显示的显示名称。最佳做法是使用描述性名称。

可选属性

* **mktoActive:** 确定此模块是否显示在电子邮件编辑器的模块列表中。 默认值为true。 如果为false，则最终用户无法将模块添加到电子邮件。
* **mktoAddByDefault:** 确定此模块是否将位于创建时使用此模板的新电子邮件的画布中。 默认值为true（如果mktoActive为false，则忽略此值）。

>[!NOTE]
>
>包含Marketo语法的类值（例如mktoModule、mktoContainer、mktoText）区分大小写。 自定义属性名称（即mktoimgwidth、mktoname）不会。

## 容器 {#containers}

容器保存模块并定义它们的放置位置。 当最终用户重新排序并在其电子邮件中插入模块时，容器会控制他们的去向。

**使用 `<table>`, `<tbody>`, `<thead>`, `<tfoot>` 或 `<td>` ，其中为class=&quot;mktoContainer&quot;**

必需属性

**id**:如何在电子邮件模板中引用模块。

>[!CAUTION]
>
>容器只能包含模块 — 如果存在其他任何内容，则容器会被视为无效！ 每个模板只允许一个容器。

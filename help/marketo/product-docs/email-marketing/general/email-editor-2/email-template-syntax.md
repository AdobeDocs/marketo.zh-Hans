---
unique-page-id: 11371040
description: 电子邮件模板语法 — Marketo 文档 — 产品文档
title: 电子邮件模板语法
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '2449'
ht-degree: 100%

---

# 电子邮件模板语法 {#email-template-syntax}

在 Marketo 全新的 Email 2.0 体验中，电子邮件模板可由元素、变量、模块或容器的任意组合构成。每一项都通过在 HTML 中添加 Marketo 专用语法来定义。旧版（v1.0）电子邮件模板在电子邮件编辑器 2.0 中仍受支持，但不会包含新编辑器的全部功能。

Marketo 的电子邮件语法仅在模板和单个电子邮件中生效；如果嵌入到片段或富文本令牌中，则&#x200B;**不会**&#x200B;生效。

>[!NOTE]
>
>Marketo 支持团队不提供 CSS/HTML 相关协助。如果您不熟悉 CSS/HTML，请咨询您的开发人员。

>[!CAUTION]
>
>包含 Marketo 语法的 class 值（例如 mktoModule、mktoContainer、mktoText）区分大小写。自定义属性名称（例如 mktoimgwidth、mktoname）不区分大小写。

## 元素 {#elements}

元素是您在电子邮件模板中定义为可编辑的内容区域。不同类型的元素具有各自独特的编辑体验，提供了简化内容编辑的方式。电子邮件模板中可包含的元素类型包括：

* 富文本
* 图像
* 代码段
* 视频

## 富文本 {#rich-text}

如果将某个区域定义为富文本，用户即可[使用 Marketo 的富文本编辑器](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)来编辑其内容。在电子邮件模板中定义富文本元素有两种方式：mktEditable 和 mktoText。请注意，富文本元素始终可以在电子邮件编辑器中转换为片段。

### 选项 1 — mktEditable {#option-mkteditable}

由于电子邮件编辑器 2.0 具备向后兼容性，一些旧版电子邮件模板可能通过在任意 HTML 元素上添加 class=&quot;mktEditable&quot; 来指定富文本元素。这种方式仍受支持，且该元素的 ID 将作为其在电子邮件编辑器中的显示名称。

所需属性

* **类**：“mktEditable”。
* **id**：ID 字符串。仅可包含字母、数字、短横线“-”和下划线“_”。不允许包含空格。必须唯一。

可选属性

* **mktoName**：字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。

默认值

带有 class=&quot;mktEditable&quot; 的 HTML 元素中所包含的内容（如果提供）将作为该富文本元素的默认值。

示例：

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### 选项 2 — mktoText {#option-mktotext}

建议使用 class=&quot;mktoText&quot; 语法来指定富文本元素。这样可以确保该元素始终具有合适的显示名称。

所需属性

* **类**：&quot;mktoText&quot;
* **id**：ID 字符串。仅可包含字母、数字、短横线“-”和下划线“_”。不允许包含空格。必须唯一。
* **mktoName**：字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。

默认值

带有 class=&quot;mktoText&quot; 的 HTML 元素中所包含的内容（如果提供）将作为该富文本元素的默认值。

示例：

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## 图像 {#images}

您有两种方式来定义可编辑的图像元素。您可以使用 `<div>`（用于指定插入 `<img>` 的容器），或直接使用 `<img>` 标记。如果您希望最终用户仅选择一张图片并返回其 URL（而非操作 DOM），请参阅下文中的“图像变量”。以下两种方式都会插入一个 HTML `<img>`元素。

### 选项 1 — 使用 `<div>` {#option-use-a-div}

所需属性

* **类：**“mktoImg”。
* **id**：ID 字符串。仅可包含字母、数字、短横线“-”和下划线“_”。不允许包含空格。必须唯一。
* **mktoName：**&#x200B;字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。

可选属性

* **mktoImgClass：**&#x200B;字符串。此处的值将添加到该 div 内 `<img>` 元素的类属性中。
* **mktoImgSrc：**&#x200B;用作放置在该 div 中图像的默认值。如果省略，则会使用占位图像。
* **mktoImgLink：**&#x200B;指定应使用包含此目标 URL 的 `<a>` 标记包裹该 `<img>` 元素。用户可在电子邮件编辑器中更改此设置。
* **mktoImgLinkTarget：**&#x200B;指定由 mktoImgLink 属性生成的 `<a>` 标记应使用此目标值。如果未同时使用 mktoImgLink，则此属性不起作用。
* **mktoImgWidth：**&#x200B;用于设置所包含 `<img>` 元素的宽度。
* **mktoImgHeight：**&#x200B;用于设置所包含 `<img>` 元素的高度。
* **mktoLockImgSize：**&#x200B;用于解锁 `<img>` 元素的高度和宽度属性，以便最终用户进行修改（如果省略，默认值为真）。
* **mktoLockImgStyle：**&#x200B;用于锁定 `<img>` 元素的样式属性（默认值为假）。

默认值（可选）

**`<img>`**：用于指定图像将放置在其中的 `<img>` 元素。如果您希望为图像添加内联样式，这将非常有用。请务必包含外层的 `<a> </a>` 标记，这样当用户添加链接时，您的样式才不会被移除！

示例：

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div>`

### 选项 2 — 使用 \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>此选项不允许最终用户为图像添加链接。如果这一点对您的模板很重要，请使用选项 1。

所需属性

* **类：**“mktoImg”。
* **id**：ID 字符串。仅可包含字母、数字、短横线“-”和下划线“_”。不允许包含空格。必须唯一。
* **mktoName：**&#x200B;字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。默认值（可选）
* **src：**&#x200B;用作图像的默认值。如果省略，则会使用占位图像。
* **mktoLockImgSize：**&#x200B;用于解锁 `<img>` 元素的高度和宽度属性，以便最终用户进行修改（如果省略，默认值为真）。
* **mktoLockImgStyle：**&#x200B;用于锁定 `<img>` 元素的样式属性（默认值为假）。

示例：
`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## 代码段 {#snippets}

如果将某个区域定义为片段，最终用户即可选择要在该区域中插入的已批准[片段](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)。尽管富文本元素可以在电子邮件编辑器中转换为片段，但如果某个区域被明确指定为片段，则无法再转换为富文本。您可以使用带有 class=&quot;mktoSnippet&quot; 的 `<div>` 来指定片段区域。

所需属性

* **id**：ID 字符串。仅可包含字母、数字、短横线“-”和下划线“_”。不允许包含空格。必须唯一。
* **mktoName：**&#x200B;字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。

默认值（可选）

**mktoDefaultSnippetId**：默认显示的 Marketo 片段的数值 ID（仅当该 ID 对应的片段存在且已在该工作区获批时才会生效）。

示例：

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## 视频 {#video}

如果将某个区域定义为视频，最终用户即可插入 YouTube 或 Vimeo 的 URL，并在电子邮件中以带有“播放”按钮的缩略图形式显示。您可以使用带有 class=&quot;mktoVideo&quot; 的 `<div>` 来指定视频区域。

所需属性

* **id**：ID 字符串。仅可包含字母、数字、短横线“-”和下划线“_”。不允许包含空格。必须唯一。
* **mktoName：**&#x200B;字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。

可选属性

* **mktoImgClass：**&#x200B;字符串。此处的值将添加到该 div 内视频缩略图 `<img>` 的类属性中。

示例：

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## 变量 {#variables}

变量的作用类似于令牌。您需要先在电子邮件模板的 `<head>` 部分使用 `<meta>` 标记定义变量，然后即可在整个模板中多次使用这些变量。由于变量是在模板中定义的，最终用户可以根据自身规则修改其值。请注意，您可以将变量定义为局部或全局作用域。如果在“模块”中使用变量，且最终用户复制了该模块，则局部变量将拥有各自独立的值，而全局变量将同时应用于两个模块。

## 字符串 {#string}

如果将变量指定为字符串，最终用户即可在电子邮件编辑器中的文本框内输入文本。您可以使用带有 class=&quot;mktoString&quot; 的 `<meta>` 来指定字符串变量。

所需属性

* **id：**&#x200B;用于在电子邮件模板中引用该变量的标识。
* **mktoName：**&#x200B;字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。

可选属性

* **allowHTML：**&#x200B;布尔值。用于控制变量值是否进行 HTML 转义。如果省略，默认值为假。
* **默认值**：字符串的默认值。如果省略，则默认为空。
* **mktoModuleScope**：布尔值。用于控制该变量在模块中使用时是局部变量（真）还是全局变量（假）。如果省略，默认值为假。

声明示例：

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

使用示例：

`${textHeader}`

## 列表 {#list}

如果将变量指定为列表，最终用户即可在电子邮件编辑器中从您定义的一组值中进行选择。您可以使用带有 class=&quot;mktoList&quot; 的 `<meta>` 来指定列表变量。

所需属性

* **id**：用于在电子邮件模板中引用该变量的标识。
* **mktoName：**&#x200B;字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。
* **值：**&#x200B;以逗号分隔的值列表。至少必须包含一个字符串。

可选属性

* **默认值：**&#x200B;下拉选择框的默认值。如果省略，则使用 &quot;values&quot; 属性中的第一个值。
* **mktoModuleScope**：布尔值。用于控制该变量在模块中使用时是局部变量（真）还是全局变量（假）。如果省略，默认值为假。

声明示例：

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

使用示例：

`${textFontFamily}`

## 数值 {#number}

如果将变量指定为数字，最终用户即可在电子邮件编辑器中输入数值。您可以使用带有 class=&quot;mktoNumber&quot; 的 `<meta>` 来指定数字变量。

所需属性

* **id**：用于在电子邮件模板中引用该变量的标识。
* **mktoName**：字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。
* **默认值：**&#x200B;变量的默认数值。

可选属性

* **最小值：**&#x200B;可接受的最小值。
* **最大值：**&#x200B;可接受的最大值。
* **单位：**&#x200B;附加到数值后的单位（例如 px、pt、em 等），会同时显示在编辑器和生成的代码中。
* **步长：**&#x200B;数值变量每次增加或减少的步长（如 0.1、1、10 等）。如果省略，默认值为 1。
* **mktoModuleScope**：布尔值。用于控制该变量在模块中使用时是局部变量（真）还是全局变量（假）。如果省略，默认值为假。

声明示例：

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1">`

使用示例：

`${textFontSize}`

## 颜色 {#color}

如果将变量指定为“颜色”，最终用户即可在电子邮件编辑器中输入十六进制颜色值，或通过颜色选择器选择颜色。您可以使用带有 class=&quot;mktoColor&quot; 的 `<meta>` 来指定颜色变量。

所需属性

* **id**：用于在电子邮件模板中引用该变量的标识。
* **mktoName**：字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。

可选属性

* **默认值：**&#x200B;颜色的默认值。6 位十六进制颜色代码。例如：#ffffff。
* **mktoModuleScope**：布尔值。用于控制该变量在模块中使用时是局部变量（真）还是全局变量（假）。如果省略，默认值为假。

声明示例：

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

使用示例：

`${textColor}`

## 布尔值 {#boolean}

如果将变量指定为布尔值，最终用户即可在电子邮件编辑器中切换该选项的开启或关闭状态。您可以使用带有 class=&quot;mktoBoolean&quot; 的 `<meta>` 来指定布尔变量。

所需属性

* **id**：用于在电子邮件模板中引用该变量的标识。
* **mktoName**：字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。

可选属性

* **默认值：**&#x200B;用于确定切换开关默认状态的布尔值。如果省略，默认值为假。
* **false_value：**&#x200B;当切换开关处于关闭状态时插入的值。如果省略，默认值为假。
* **true_value：**&#x200B;当切换开关处于开启状态时插入的值。如果省略，默认值为真。
* **false_value_name：**&#x200B;切换开关处于关闭状态时在 UI 中显示的名称。如果省略，默认值为假。
* **true_value_name：**&#x200B;切换开关处于开启状态时在 UI 中显示的名称。如果省略，默认值为真。
* **mktoModuleScope**：布尔值。用于控制该变量在模块中使用时是局部变量（真）还是全局变量（假）。如果省略，默认值为假。

声明示例：

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

使用示例：

`${showFooter}`

## HTML 块 {#html-block}

如果将变量指定为 HTML 块，最终用户即可在电子邮件编辑器中直接输入原始 HTML 内容。您可以使用带有 class=&quot;mktoHTML&quot; 的 `<meta>` 来指定 HTML 块变量。

所需属性

* **id**：用于在电子邮件模板中引用该变量的标识。
* **mktoName**：字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。

可选属性

* **默认值：**&#x200B;经过 HTML 编码的值，用作该块的默认内容。
* **mktoModuleScope**：布尔值。用于控制该变量在模块中使用时是局部变量（真）还是全局变量（假）。如果省略，默认值为假。

声明示例：

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

使用示例：

`${trackingPixel}`

## 图像变量 {#image-variable}

如果将变量指定为“图像”，最终用户即可在电子邮件编辑器中通过图像选择器选择图片。所选图像的 URL 将作为该变量的值。您可以使用带有 class=&quot;mktoImg&quot; 的 `<meta>` 来指定图像变量。

所需属性

* **id**：用于在电子邮件模板中引用该变量的标识。
* **mktoName**：字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。

可选属性

* **默认值：**&#x200B;该元素的默认图像 URL。
* **mktoModuleScope**：布尔值。用于控制该变量在模块中使用时是局部变量（真）还是全局变量（假）。如果省略，默认值为假。

声明示例：

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

使用示例：

`${heroBackgroundImage}`

## 模块 {#modules}

模块是在模板级别定义的模板化区块，最终用户可以将其插入到电子邮件中使用。由于这些模块是预先构建的，您可以确保它们能够与电子邮件的其他内容良好协作（并具备完整的响应式表现）。模块只能放置在容器中。

>[!IMPORTANT]
>
>当基于包含已定义模块组件的电子邮件模板生成电子邮件后，对模板中模块所做的任何更改都&#x200B;**不会**&#x200B;同步到该电子邮件。

**对于类型为 `<table>`、`<tbody>`、`<thead>` 或 `<tfoot>` 的容器：**

使用带有 class=&quot;mktoModule&quot; 的 `<tr>` 进行指定

**对于类型为 `<td>` 的容器：**

使用带有 class=&quot;mktoModule&quot; 的 `<table>` 进行指定

所需属性

* **id**：用于在电子邮件模板中引用该模块的标识。
* **mktoName**：字符串。这是在电子邮件编辑器 2.0 中显示的名称，最佳做法是使用具有描述性的名称。

可选属性

* **mktoActive：**&#x200B;用于确定该模块是否显示在电子邮件编辑器的模块列表中。默认值为真。如果设置为假，最终用户将无法将该模块添加到电子邮件中。
* **mktoAddByDefault：**&#x200B;用于确定在基于该模板创建新电子邮件时，该模块是否会默认出现在画布中。默认值为真（如果 mktoActive 为假，则会忽略此值）。

>[!NOTE]
>
>包含 Marketo 语法的 class 值（例如 mktoModule、mktoContainer、mktoText）区分大小写。自定义属性名称（例如 mktoimgwidth、mktoname）不区分大小写。

## 容器 {#containers}

容器用于承载模块，并定义模块可放置的位置。当最终用户在电子邮件中重新排序或插入模块时，容器将控制模块可放置的范围。

**使用带有 class=&quot;mktoContainer&quot; 的 `<table>`、`<tbody>`、`<thead>`、`<tfoot>` 或 `<td>` 进行指定**

所需属性

**id**：用于在电子邮件模板中引用该模块的标识。

>[!CAUTION]
>
>容器中只能包含模块——如果包含其他任何内容，该容器将被视为无效！每个模板只允许包含一个容器。

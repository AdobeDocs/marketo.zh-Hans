---
solution: Marketo Engage
product: marketo
title: 可自定义的片段
description: 了解如何通过使某些字段可编辑来自定义片段。 在电子邮件Designer中创建灵活的可重用片段。
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
TQID: https://experienceleague.adobe.com/SCmyn9QUECmvQgVltKknlvLuvL15Tz3LYorBFYB1hqI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 8ba2ac1fa056e96aac50abbde16042e522779ab3
workflow-type: tm+mt
source-wordcount: 1405
ht-degree: 0%

---

# 可自定义的片段 {#customizable-fragments}

在电子邮件或电子邮件模板中使用片段时，默认情况下会由于继承而锁定这些片段，这意味着对片段所做的任何更改都会自动传播到使用该片段的所有资源。 利用可自定义的片段，在将片段添加到电子邮件或电子邮件模板时，可以将片段中的特定字段定义为可编辑。 例如，如果片段中包含横幅、某些文本和按钮，您可以将某些字段（如图像或按钮目标URL）指定为可编辑。

通过可自定义的片段，您可以管理和个性化内容，而无需创建全新的内容块或中断片段继承。 在片段级别所做的更改仍会传播，同时允许在电子邮件或电子邮件模板级别进行自定义。

可视片段和表达式片段均可以标记为可自定义。

## 在可视片段中添加可编辑字段 {#visual}

要使可视片段的某些部分可编辑，请执行以下步骤：

>[!NOTE]
>
>可编辑的字段可添加到&#x200B;**图像**、**文本**&#x200B;和&#x200B;**按钮**&#x200B;组件中。 对于&#x200B;**HTML**&#x200B;组件，使用个性化编辑器添加可编辑的字段，类似于表达式片段。 [了解如何在HTML组件和表达式片段中添加可编辑字段](#expression)

1. 打开片段内容版本屏幕。

1. 选择片段中要配置可编辑字段的组件。

1. 组件属性窗格将在右侧打开。 选择&#x200B;**[!UICONTROL Editable fields]**&#x200B;选项卡，然后切换&#x200B;**[!UICONTROL Enable edition]**&#x200B;选项。

1. 窗格中列出了可为选定组件编辑的所有字段。 可供编辑的字段取决于所选的组件类型。

   在以下示例中，“单击此处”按钮URL配置为可编辑。

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL Overview]**&#x200B;以检查所有可编辑的字段及其默认值。

   在此示例中，按钮URL字段显示在组件中定义的默认值中。 在将片段添加到其内容后，用户可以自定义此值。

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. 完成时保存更改。

将片段添加到电子邮件后，用户可以自定义片段中配置的所有可编辑字段。

## 将可编辑字段添加到HTML组件和表达式片段 {#expression}

在HTML组件中，可以将以下类型的元素设置为可编辑：

* **文本内容**&#x200B;的一部分（例如，标题或CTA标签）。
* 完整的&#x200B;**URL**，用作链接目标或图像源。 不支持部分URL；变量必须表示整个URL值。
* 完整的&#x200B;**CSS属性值**（例如，全色值、全填充值或全宽值）。 不支持部分CSS属性值。

每个参数化CSS属性值必须刚好是`{{{varName}}}`：没有后缀、没有附加文本、没有多个变量以及单个属性内没有连接。

要参数化多侧属性（如填充），请执行以下任一操作：

* 将每一方声明为单独属性&#x200B;_（推荐）_，或
* 声明包含完整速记值的单个变量。

## 可编辑字段在HTML组件中的工作方式 {#components}

HTML组件中的可编辑字段是通过直接在组件的源代码中声明内联变量创建的。 每个变量都有一个唯一的ID和一个默认值。 然后，只要可编辑值出现在标记中，就会引用变量。

保存并发布片段后，在将片段添加到电子邮件时，在HTML组件中声明的每个变量都会自动显示为可编辑参数。

然后，电子邮件作者可以覆盖来自Email Designer的任何变量的默认值（例如，更改背景颜色、交换CTA URL或更新标题），而无需修改底层HTML。

## 语法参考 {#syntax}

可使用两种模式定义和引用可编辑字段：

### 声明变量 {#declaring}

使用内联声明定义具有唯一ID和默认值的变量：

```handlebars
{{#inline "variableID"}}default_value{{/inline}}
```

将`variableID`替换为可编辑字段的唯一标识符。 该ID在组件中必须唯一，且不得包含空格。

将`default_value`替换为电子邮件作者未覆盖它时应使用的值。

### 引用变量 {#referencing}

使用三大括号引用变量的值，无论该变量的值出现在标记中什么位置：

```handlebars
{{{variableID}}}
```

在HTML中，可多次引用同一变量ID。 所有引用都将解析为电子邮件作者设置的任何值（如果未提供覆盖，则解析为默认值）。

### 可选参数 {#optional}

内联声明支持可更改可编辑字段显示或处理方式的可选参数：

| 操作 | 参数 | 示例 |
|---|---|---|
| 使用&#x200B;**默认值**&#x200B;声明可编辑字段。 将片段添加到电子邮件时，除非作者覆盖它，否则使用此默认值。 | 在内联标记之间添加默认值。 | `{{#inline "editableFieldID"}}default_value{{/inline}}` |
| 为可编辑字段定义&#x200B;**标签**。 当电子邮件作者编辑片段的字段时，此标签显示在电子邮件Designer中。 | `name="title"` | `{{#inline "editableFieldID" name="title"}}default_value{{/inline}}` |
| 声明包含&#x200B;**图像源**&#x200B;的可编辑字段。 | `assetType="image"` | `{{#inline "editableFieldID" assetType="image"}}default_value{{/inline}}` |
| 声明包含需要跟踪的&#x200B;**URL**&#x200B;的可编辑字段。 | `assetType="url"` | `{{#inline "editableFieldID" assetType="url"}}default_value{{/inline}}` |

## 向HTML组件添加可编辑字段 {#adding-editable-fields}

要使可视片段中HTML组件的某些部分可编辑，请执行以下步骤：

1. 打开可视化片段以在Email Designer中进行编辑。
1. 从“组件”面板中将&#x200B;**HTML组件**&#x200B;添加到片段，或选择现有的HTML组件。
1. 选择HTML组件后，单击&#x200B;**显示源代码**&#x200B;以在个性化编辑器中打开HTML源视图。
1. 在个性化编辑器中，使用内联声明语法声明每个可编辑的变量。 为了提高可读性，请将所有变量声明放在组件的顶部，并为每个变量分配一个唯一ID。
1. 在应显示可编辑值的任意位置，使用`{{{variableID}}}`语法引用HTML标记中的每个变量。 同一变量可在同一组件中多次引用。
1. 保存HTML组件，然后保存片段。
1. 发布片段以使其可在电子邮件中使用。

## 在电子邮件中使用片段 {#using-fragment}

片段发布后，在其HTML组件中声明的所有变量将作为可编辑参数显示在电子邮件Designer中。

要在电子邮件中使用片段时自定义它们，请执行以下操作：

1. 在Marketo Engage Email Designer中打开或创建电子邮件。
1. 将已发布的片段添加到电子邮件画布。
1. 选择片段以打开其属性窗格。 可编辑字段列表显示在&#x200B;**可编辑字段**&#x200B;部分下，每个字段均标有其变量ID（或通过`name`参数指定的友好标签）。
1. 直接从属性窗格更新任何可编辑字段的值。 此更改仅适用于当前电子邮件；已发布的片段和引用该片段的其他电子邮件不受影响。
1. 保存电子邮件。

片段使用自定义值呈现，同时仍继承对已发布片段所做的任何未来结构更新。

### 示例：包含可编辑文本、颜色和URL的简单片段 {#example}

以下示例使用四个可编辑字段创建一个小型促销横幅：

* 背景颜色
* 标题文本
* CTA标签
* CTA URL

发布片段后，电子邮件作者可以在将片段添加到电子邮件时覆盖这些值中的任意值。

**简单可编辑的横幅**

```html
<!-- Define editable variables -->
{{#inline "bgColor"}}#0057FF{{/inline}}
{{#inline "headlineText"}}Example Headline{{/inline}}
{{#inline "ctaText"}}Learn More{{/inline}}
{{#inline "ctaUrl" assetType="url"}}https://www.example.com{{/inline}}

<!-- Use the variables in the HTML -->
<table width="100%" cellpadding="0" cellspacing="0"
       style="background-color:{{{bgColor}}}; border-radius:8px;" >
  <tr>
    <td style="padding:30px; text-align:center; font-family:Arial,sans-serif;">
      <h2 style="color:#ffffff; font-size:24px; margin:0;">
        {{{headlineText}}}
      </h2>
      <a href="{{{ctaUrl}}}"
         style="display:inline-block; margin-top:16px; padding:12px 28px;
                background:#ffffff; color:{{{bgColor}}};
                font-weight:bold; border-radius:4px; text-decoration:none;">
        {{{ctaText}}}
      </a>
    </td>
  </tr>
</table>
```

在此示例中：

* `bgColor`被引用了两次：一次用于表背景颜色，另一次用于CTA文本颜色。 两个引用都解析为相同的值，因此单个编辑会传播到两个位置。
* 使用`assetType="url"`声明了`ctaUrl`，这表示应将该值作为跟踪的URL进行处理。

## 最佳做法 {#best-practices}

* 在变量的默认值中包含单位(`px`、`em`、`%`)，以使变量表示完整的CSS值。 这样可避免出现不支持的连接。
* 当可能需要单独编辑每一方时，首选每方longhand CSS属性(`padding-top`、`padding-right`、`padding-bottom`、`padding-left`)而非简写。
* 当需要跟踪URL时，使用`assetType="url"`声明该URL。
* 当可编辑字段携带图像源时，使用`assetType="image"`声明该字段。
* 通过将片段添加到草稿电子邮件来测试片段，并验证所有可编辑的字段是否都显示在属性窗格中，并在被覆盖时正确解析。

## 注意事项 {#things-to-know}

* HTML组件中的可编辑字段支持全文内容、完整URL和完整CSS属性值。 无法参数化部分URL和部分CSS属性值。
* 单个CSS属性值不能将变量与其他静态文本或其他变量组合在一起。 每个参数化属性值必须正好是一个变量引用。
* 变量ID在HTML组件中必须唯一，且不得包含空格。
* 现成的系统链接（如取消订阅链接和镜像页面URL）无法转换为可编辑字段。

<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->

>[!MORELIKETHIS]
>
>[片段](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}

---
solution: Marketo Engage
product: marketo
title: 标题
description: 了解如何使用可重复使用的主题和模块简化电子邮件创建，确保设计的一致性和效率。
feature: Email Designer
role: User
level: Beginner, Intermediate
hide: true
hidefromtoc: true
source-git-commit: 1cfb28f47ba3c168292b298e1fc7ab2ff638b412
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 4%

---

# 将主题应用于您的电子邮件内容 {#apply-email-themes}

>[!AVAILABILITY]
>
>此功能目前为 Beta 版，仅供 Beta 版客户使用。要加入 Beta 版计划，请联系 Adobe 代表。

对于主题，非技术用户能够通过添加标准模板<!-- to achieve brand specific results-->上的自定义样式来创建符合特定品牌和设计语言的可重用内容。

此功能使营销人员能够更快更轻松地利用具有视觉吸引力的品牌一致性电子邮件，同时提供高级自定义选项以满足独特的设计需求。

<!--What is the Enhanced Email Authoring Experience?

This feature introduces two key components to simplify and enhance email creation:

* **Theme Management System**: A centralized system for creating, customizing, and applying reusable themes to emails. Themes ensure consistent styling across campaigns and eliminate the need for repetitive manual styling.

* **Modules**: Pre-designed, reusable content blocks that abstract common email elements (e.g., titles, descriptions, images, and links). Modules are built using customizable low-level components, offering flexibility while maintaining design standards.

Key Benefits:

- **Consistency**: Ensure all emails align with your brand's design guidelines.
- **Efficiency**: Save time by reusing themes and modules across campaigns.
- **Customization**: Add custom CSS and mobile-specific styles for advanced designs.
- **Scalability**: Eliminate repetitive styling tasks, enabling faster email creation.-->

## 护栏和限制 {#themes-guardrails}

* 从头开始创建电子邮件时，您可以选择使用主题开始构建内容，以快速应用符合您的品牌和设计的特定样式。

  如果选择&#x200B;_手动样式_&#x200B;模式，除非重置电子邮件，否则无法应用任何主题。

* [片段](/help/marketo/product-docs/email-marketing/email-designer/fragments.md)在&#x200B;_使用主题_&#x200B;和&#x200B;_手动样式设置_&#x200B;模式之间不交叉兼容。

  要在应用主题的内容中使用片段，必须以&#x200B;_使用主题_&#x200B;模式创建此片段。

* 如果使用在HTML中创建的内容，您将处于[兼容模式](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html)，并且无法将主题应用于此内容。

  要充分利用Email Designer的所有功能，包括主题，您必须在&#x200B;_使用主题_&#x200B;模式下创建新内容，或转换您的[导入的HTML内容](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html)。

<!--If using a content created in Manual Styling mode or HTML, you cannot apply themes to this content. You must create a new content in Use Themes mode.

If you apply a theme to a content using a [fragment](../content-management/fragments.md) created in Manual Styling mode, the rendering may not be optimal.-->

## 创建主题 {#create-and-edit-themes}

要定义可在未来电子邮件内容中利用的主题，请执行以下步骤。

1. 若要开始，请创建新的[电子邮件模板](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template)。

1. 选择&#x200B;**[!UICONTROL Create or edit themes]**&#x200B;选项。

   `![](assets/theme-create.png)`

1. 您可以选择默认主题，也可以使用Adobe或自定义模板。 在此示例中，选择默认主题并单击&#x200B;**[!UICONTROL Create]**。

   `![](assets/theme-select.png)`

1. 在&#x200B;**[!UICONTROL General settings]**&#x200B;选项卡中，通过为品牌提供特定名称来开始定义主题。 您可以调整电子邮件的默认宽度，也可以导出当前主题以跨沙盒共享它。

   `<!--![](assets/theme-general-settings.png)-->`

1. 使用右侧的边栏浏览不同的选项卡并更新您的设计设置。

   `![](assets/theme-right-pane.png)`

1. 从&#x200B;**[!UICONTROL Colors]**&#x200B;选项卡：

   * 使用&#x200B;**[!UICONTROL Edit]**&#x200B;按钮可为您的品牌设置具有默认颜色的&#x200B;**[!UICONTROL Color palette]**。 选择&#x200B;**[!UICONTROL Preset]**&#x200B;以快速创建颜色方案，或单独调整主题的每种颜色。 您也可以同时使用这两种方法。

     `![](assets/theme-colors.gif)`

   * 单击&#x200B;**[!UICONTROL Add variant]**&#x200B;可创建多个颜色变体，如浅色和深色模式，其中每个变体都有自己的调色板和细微差别控件。

     `![](assets/theme-colors-variant.png)`

   * 对于每个变体，单击编辑图标以编辑任何单个元素。 您可以使用已创建的默认调色板或任何自定义颜色。

     `![](assets/theme-colors-edit-variant.gif)`

1. 在&#x200B;**[!UICONTROL Text settings]**&#x200B;中，您可以设置要用于整个主题的全局字体。 为了获得更细粒度的控件，您还可以编辑每个标题和段落类型以调整字体、大小、样式等。

   `![](assets/theme-text.png)`

1. 在&#x200B;**[!UICONTROL Spacing]**&#x200B;选项卡中，从列表中选择单个元素以在不同组件之间正确间隔该元素。

   `<!--![](assets/theme-spacing.png)-->`

1. 使用右侧的其他选项卡，您可以单独管理此主题的每个按钮元素、分隔条、其他图像格式和网格布局间距。

   `<!--![](assets/theme-buttons.png)-->`

1. 单击&#x200B;**[!UICONTROL Save]**&#x200B;存储此主题以供将来使用。

## 将主题应用到电子邮件 {#apply-themes}

要将默认或自定义样式主题应用于电子邮件，请执行以下步骤。

1. `In [!DNL Marketo Engage], [add an email](create-email.md) action to a journey or campaign, and [edit your email body](get-started-email-design.md#key-steps).`

1. 您可以选择以下操作之一：

   * `Select a built-in [email template](use-email-templates.md) to open the Email Designer. A default theme specific to each template is automatically applied.`

   * `Design a [new content from scratch](content-from-scratch.md) and select **[!UICONTROL Use Themes]** to start with a predefined styling theme.`

     `![](assets/theme-from-scratch.png)`

     >[!CAUTION]
     >
     >如果选择&#x200B;_手动样式_&#x200B;模式，除非重置电子邮件，否则无法应用任何主题。
     >
     >若要在[使用主题](/help/marketo/product-docs/email-marketing/email-designer/fragments.md)模式下使用&#x200B;_片段_，此片段必须已使用&#x200B;_使用主题_&#x200B;模式自行创建。

1. 进入电子邮件Designer后，单击右边栏上的&#x200B;**[!UICONTROL Themes]**&#x200B;按钮。 将显示默认主题或模板主题。 您可以在此主题的两个颜色变体之间切换。

   `![](assets/theme-default-hero.png)`

1. 单击当前使用的主题旁边的箭头。 此时将显示可用自定义主题和Adobe主题的列表。

   `![](assets/theme-hero-change.png)`

1. 单击&#x200B;**[!UICONTROL Custom themes]**&#x200B;并选择您创建的主题。

   `![](assets/theme-select-custom.png)`

1. 单击下拉列表外部。 新选择的自定义主题会自动将其样式应用于所有电子邮件组件。 您可以在两种颜色变体之间切换。

1. 选择某个组件后，您仍然可以使用专用图标解锁其样式。

   `![](assets/theme-unlock-style.png)`

您可以随时切换主题。 电子邮件内容保持不变，但样式将更新以反映新主题。

<!--
>[!NOTE]
> - Themes apply styles globally. Ensure your theme is finalized before applying it to multiple emails.
> - Switching themes may override custom styles applied to individual components.

>[!CAUTION]
> - When using fragments, the email's theme will override the fragment's styles. A warning will be displayed in the editor if there is a conflict.

## Example Use Cases {#example-use-cases}

### 1. Creating a New Theme
- A marketer creates a theme with their brand's colors, fonts, and button styles.
- The theme is saved and reused across multiple email campaigns.

### 2. Switching Themes
- A marketer applies a holiday-themed design to an existing email by switching to a pre-designed holiday theme.-->

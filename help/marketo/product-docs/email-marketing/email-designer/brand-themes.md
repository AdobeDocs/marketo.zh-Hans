---
solution: Marketo Engage
product: marketo
title: 标题
description: 描述。
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
exl-id: e6b576e5-3456-4bee-9383-b63cd6728620
source-git-commit: 6ff95c8c3b59239586982b10996e18e942509f8d
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 0%

---

# 品牌主题 {#brand-themes}

使用品牌主题，通过向电子邮件模板添加自定义样式，轻松创建符合特定品牌和设计语言的可重用内容。

此功能使营销人员能够更快更轻松地利用具有视觉吸引力的品牌一致性电子邮件，同时提供高级自定义选项以满足独特的设计需求。

## 注意事项 {#things-to-note}

* 从头开始创建电子邮件时，您可以选择使用主题开始构建内容，以快速应用符合您的品牌和设计的特定样式。 如果选择“经典”模式，除非重置电子邮件，否则无法应用任何主题。

* 片段在主题模式和经典模式之间不交叉兼容。 要在应用主题的内容中使用片段，必须在主题模式下创建片段。

* 更新主题不会自动层叠到使用它们的所有资源。 您需要编辑单个对象以刷新主题。

* 删除主题时，不会影响使用它们的资源。

## 创建品牌主题 {#create-a-brand-theme}

1. 按照步骤[创建电子邮件模板](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template)。

1. 在&#x200B;_设计模板_&#x200B;屏幕中，选择&#x200B;**创建或编辑主题**。

   ![](assets/brand-themes-1.png)

1. 选择默认主题作为从头开始创建的基础，然后单击&#x200B;**创建**。

   ![](assets/brand-themes-2.png)

1. 画布随即打开，可供您编辑主题的不同部分。

   ![](assets/brand-themes-3.png)

## 设置

可以通过右侧的图标访问所有设置选项。 让我们逐一回顾一下。

![](assets/brand-themes-4.png)

### 常规设置 {#general-settings}

命名主题并调整视区大小。

![](assets/brand-themes-5.png)

### 颜色 {#colors}

进行颜色调整时，请观察在主面板上生效的更改。

![](assets/brand-themes-6.png)

>[!NOTE]
>
>已根据默认主题为您配置了一组样本。

单击&#x200B;**编辑**。

![](assets/brand-themes-7.png)

您可以从预设中进行选择，也可以单独配置预设集中的每种颜色。 选择调色板后，可在不同的颜色设置下访问这些颜色。

![](assets/brand-themes-8.png)

编辑完毕后，单击后退箭头（![后退箭头图标](assets/icon-back-arrow.png)）返回。

要编辑变体，请单击其铅笔图标。

![](assets/brand-themes-.png)

>[!NOTE]
>
>您最多可以创建六个变体。

有多个元素可供自定义。

![](assets/brand-themes-.png)

变体设置分为以下类别：

* 常规
* 标题
* 段落
* 按钮

**常规**

这些设置允许您设置主体、结构、背景、容器、图像等的颜色。

![](assets/brand-themes-.png)

**标题**

设置每种标题类型的文本和边框颜色，从标题1到标题6。

![](assets/brand-themes-.png)

**段落**

设置最多三种段落类型的文本和边框颜色。

![](assets/brand-themes-.png)

**按钮**

为三种不同的按钮类型设置填充、边框和文本颜色：“主要”、“次要”和“第三”。

![](assets/brand-themes-.png)

### 文本设置 {#text-settings}

设置全局、标题和段落的字体类型和大小。

![](assets/brand-themes-.png)

**全局**

在“全局文本设置”下，在Standard和Google字体库之间选择“表单库”。

![](assets/brand-themes-.png)

在“标准”下，从不同的字体系列中进行选择。

![](assets/brand-themes-.png)

同样，在“Google Fonts”下，将显示从分别支持的字体中进行选择的选项。

**标题**

您可以在此为不同的标题类型设置字体库、系列、大小、文本样式和文本对齐。

屏幕快照

**段落**

您可以在此为不同的段落预设设置字体库、系列、大小、文本样式和文本对齐。

屏幕快照

### 间距和边框 {#spacing-and-border}

在此下，您可以为不同类型的结构或按钮设置填充和边距。  在第一个下拉菜单中选择类型，然后继续为该元素设置“填充”和/或“边距”。 如果适用，请逐一重复此操作。

屏幕快照

结构类型如下：

屏幕快照

示例元素的设置，如Container。

边距

屏幕快照

填充

屏幕快照

角

屏幕快照

边框

将边框切换为打开以显示用于设置大小、样式和位置的选项。

屏幕快照

样式的选项

屏幕快照

关于样式对框的影响的一些示例

```
TABLE

Type

Size and Style setting

Effect

Dashed

Dotted

Solid
```

调整边框是使用边框位置显示还是隐藏

示例：下面的示例中隐藏了Top。

```
TABLE

Position setting

Effect
```

为不同类型的结构重复设置边距、内边距、边角和边框类型的设置。

### 按钮设置 {#button-settings}

在此下，您可以设置有关按钮的不同元素（颜色除外），如按钮形状、按钮半径、按钮文本和按钮大小。 您可以为3个预设设置这些值 — “主”、“次”和“第三”。

屏幕快照

```
TABLE

Primary/Secondary/Tertiary    Allows settings for 3 presets of button configurations
Text > Font Library    Font library choice for button text
Text > Font family    Font family choice for button text
Text > Font size    Font size for button text
Text > Text styles    Text style (bold, italicized, underlined, strikethrough) for button text
Text > Text alignment    Alignment for button text
Border> Border size     Button border thickness
Border> Border style    Button border style (dashed, solid, dotted, etc.)
Border> Border radius    Button border corner curvature
SIZE > Height    Height setting for the button
SIZE > Width    Width setting for the button
```

### 分隔线设置 {#divider-settings}

在此下，您可以设置分隔线的行类型和容器设置。

屏幕快照

### 网格设置 {#grid-settings}

使用“列”间隙控制网格中的间距。

```
TABLE
```

完成后单击保存。

屏幕快照

## 编辑品牌主题 {#editing-brand-themes}

可在编辑器的模板选择面板中创建品牌主题。 您可以在创建新模板时访问此面板，或从编辑器中的Change Design访问此面板。

屏幕快照

单击“更改设计”。

屏幕快照

单击创建或编辑主题

屏幕快照

选择自定义主题以显示您的组织中创建的自定义主题列表。 选择一个主题，然后单击编辑。

屏幕快照

现在，画布已打开以进行编辑。

屏幕快照

修改右窗格中部分下的任何设置。

屏幕快照

完成后，单击保存。

屏幕快照

## 使用品牌主题 {#using-brand-themes}

由此创建/编辑的品牌主题已准备好在电子邮件、电子邮件模板和片段资产中使用。

Adobe Marketo Engage：已准备好在使用新电子邮件编辑器创建的电子邮件、电子邮件模板和片段资产中利用由此创建/编辑的品牌主题。

您可以在编辑器中创建结构和组件，并应用任何品牌主题及其任何变体。

### 在您的电子邮件中 {#in-your-emails}

从头开始创建电子邮件/电子邮件模板

* 从“创建电子邮件”/“创建电子邮件模板”开始，选择“从头开始设计”选项

* 在显示的模式中，选择“使用主题”

屏幕快照

注意：只有使用此选项创建的电子邮件才能利用上一部分中定义的品牌主题

* 此新选项显示在右侧栏中，允许您在电子邮件中使用品牌主题

屏幕快照

* 您可以从Adobe主题或为您的品牌创建的自定义主题中进行选择

屏幕快照

* 在画布中设计电子邮件内容并选择要应用于该内容的主题

* 一个电子邮件应仅包含一个品牌主题

* 对于在此资源中创建的任何组件，您可以从右侧窗格的“样式”选项卡中应用主题中可用的任何样式选项

* 例如，CTA可以配置为primary/secondary/tertiary

屏幕快照

* 例如，可选择文本组件以应用主题中定义的任何标题/段落样式

屏幕快照

* 请注意，现在“样式”选项卡的外观不同于传统的手动样式设置电子邮件，在手动样式设置电子邮件中，组件样式更具创意性

### 从模板创建电子邮件/电子邮件模板

* 在从预先存在的电子邮件模板创建电子邮件或电子邮件模板时，您可以利用主题，这些模板也是使用主题创建的

* 从“创建电子邮件”/“创建电子邮件模板”开始，从“保存的模板”部分选择使用主题创建的电子邮件模板之一

* 现在，已自动应用保存的电子邮件模板中使用的主题

屏幕快照

* 您还可以通过右侧栏中的“主题”选项更改此电子邮件/电子邮件模板中的主题

屏幕快照

* 您还可以将主题的任何变体应用于内容

屏幕快照

屏幕快照

### 在您的片段中 {#in-your-fragments}

从“创建新片段”开始

从右侧栏中的“主题”选项中，选择所需的主题并应用相同的主题

屏幕快照

此后在画布中创建的所有片段内容将采用所选主题

您还可以将主题的任何变体应用于内容

发布此片段后，此片段可用于使用主题创建的任何电子邮件/电子邮件模板

---
description: 深色模式 — Marketo文档 — 产品文档
title: 深色模式
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: f960d7918d97a2c5e3d16673bc4c5c592004ff1e
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 1%

---

# 深色模式 {#dark-mode}

设计电子邮件时，Email Designer允许您切换到&#x200B;**[!UICONTROL Dark mode]**&#x200B;视图。

在&#x200B;**[!UICONTROL Dark mode]**&#x200B;中，您可以定义在电子邮件客户端的深色模式打开时通过支持电子邮件客户端显示的特定自定义设置。

## 什么是深色模式？ {#what-is-dark-mode}

深色模式允许支持电子邮件客户端和应用程序为文本、按钮和其他UI元素显示具有更暗背景和更浅颜色的电子邮件。 它有助于减少眼睛疲劳、节省电池续航时间，并提高在弱光环境中的可读性，从而提供更舒适的观看体验。

## 护栏 {#guardrails}

不同电子邮件客户端的深色模式渲染可能大不相同。

在使用深色模式之前，请务必了解主要电子邮件客户端如何处理该模式。 有三种情况可以区分：

### 客户端不支持深色模式 {#not-supporting}

某些电子邮件客户端根本不支持此功能，例如：

* Yahoo！邮件
* AOL

无论您是否定义深色模式自定义设置，这些电子邮件客户端都不会显示任何深色模式渲染。

### 客户端应用自己的深色模式 {#default-support}

某些电子邮件客户端会系统地将其自己的默认深色模式应用于收到的所有电子邮件。 颜色、背景、图像等会自动调整为该电子邮件客户端指定的深色模式设置。 无法进行外部修改。

例如，这些客户端：

* Gmail(桌面Webmail、iOS、Android、Mobile Webmail)
* Outlook Windows
* Outlook Windows Mail

在这种情况下，如果您在电子邮件Designer中定义自定义深色模式设置，则电子邮件客户端设置会覆盖这些设置。

因此，虽然这些电子邮件客户端确实处理了深色模式，但您特定的深色模式设计将不会呈现。

### 支持自定义深色模式的客户端 {#custom-support}

其他电子邮件客户端提供了使用`@media (prefers-color-scheme: dark)`查询呈现自定义深色模式的选项，该查询是[!DNL Marketo Engage]电子邮件Designer使用的方法。

以下是处理此选项的主要客户端列表：

* Apple Mail macOS
* Apple Mail iOS
* Outlook macOS
* Outlook.com
* Outlook iOS
* Outlook Android

在这种情况下，应显示您在电子邮件Designer中定义的设置。

>[!NOTE]
>
>在[本节](#define-custom-dark-mode)中了解如何使用Email Designer定义自定义深色模式设置。

但是，可能会根据每个电子邮件客户端应用某些限制。 例如，如果存在图像，则某些客户端(如Apple Mail 16 (macOs 13))将不会生成深色模式。

为了获得最佳结果，请在您定位的电子邮件客户端中测试您的内容。 若要查看尽可能接近每个客户端最终结果的模拟，请使用Email Designer中的[电子邮件渲染](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md)功能。

## 电子邮件设计器中的深色模式 {#dark-mode-email-designer}

在Email Designer中，当涉及到深色模式时，需要考虑两个方面：

* 您可以预览默认深色模式在大多数支持的电子邮件客户端中的呈现方式。 [了解详情](#preview-dark-mode)

* 如果要覆盖支持电子邮件客户端的默认设置，可以在正在编辑的电子邮件中定义自定义深色模式设置。 [了解详情](#define-custom-dark-mode)

### 预览默认深色模式 {#preview-dark-mode}

要在Email Designer中访问深色模式并预览默认深色模式设置，请执行以下步骤。

1. 从电子邮件Designer主页中，选择&#x200B;**[!UICONTROL Design from scratch]**&#x200B;选项。

1. 将[结构和内容](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#add-structure-and-content)添加到您的电子邮件中。

1. 在右上方，启用&#x200B;**[!UICONTROL Dark mode]**&#x200B;切换开关。

   屏幕快照

1. 默认深色模式预览显示。

   屏幕快照

默认情况下， Email Designer深色模式预览会将“全色反色”配色方案应用于除图像和图标之外的所有元素。

这意味着它可以检测包含亮元素和暗元素的区域，并将它们反转，这样浅色背景变为深色，深色文本变为浅色，而深色背景变为浅色，浅色文本变为深色。

>[!CAUTION]
>
>最终渲染可能会因收件人的电子邮件客户端而异。 若要查看尽可能接近每个电子邮件客户端最终结果的模拟，请使用[电子邮件渲染](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md)选项。

### 定义自定义深色模式 {#define-custom-dark-mode}

切换到&#x200B;**[!UICONTROL Dark mode]**&#x200B;后，您可以选择编辑内容的特定样式元素，这些样式元素仅在收件人的电子邮件客户端中启用深色模式时显示，前提是它支持该功能。

>[!WARNING]
>
>深色模式的最终渲染取决于每个电子邮件客户端，因此结果可能因不同而异。 [了解详情](#guardrails)

为了利用Email Designer自定义深色模式样式，Journey Optimizer使用`@media (prefers-color-scheme: dark)` CSS查询，该查询会检测用户的电子邮件客户端是否设置为深色模式，并应用您的电子邮件中定义的深色主题设计。

要定义自定义深色模式设置，请执行以下步骤。

1. 确保切换到电子邮件Designer中的&#x200B;**[!UICONTROL Dark mode]**&#x200B;预览。 [了解如何操作](#preview-dark-mode)

1. 编辑任何样式颜色属性，如文本、背景、按钮等。

1. 您无法更改图像和图标的颜色，但只能为深色模式定义特定资产。 要执行此操作，请选择任意图像。 使用&#x200B;**[!UICONTROL Dark mode]**&#x200B;窗格中的专用切换开关切换到&#x200B;**[!UICONTROL Settings]**&#x200B;并选择其他资源。

   屏幕快照

1. 您随时可以&#x200B;**[!UICONTROL Switch to live view]**&#x200B;以查看您的内容在各种设备大小上的呈现方式。 从该视图中，选择屏幕顶部的深色模式切换开关以预览不同设备上内容的深色模式版本。

   屏幕快照

   >[!CAUTION]
   >
   >实时视图是一个通用预览，用于比较呈现在各种设备大小中的外观。 最终渲染可能会因收件人的电子邮件客户端而异。

1. 对深色模式的更改感到满意后，单击&#x200B;**[!UICONTROL Simulate Content]**。

   ![](assets/dark-mode-simulate.png)

1. 选择&#x200B;**[!UICONTROL Render email]**&#x200B;并连接到您的Litmus帐户。 您可以看到各种电子邮件客户端的最终深色模式渲染。 了解有关[电子邮件渲染](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md)的更多信息。

   >[!WARNING]
   >
   >虽然模拟与电子邮件在深色模式中的显示方式非常接近，但实际呈现方式可能会因电子邮件服务提供商或设备级设置的不同而有所不同。

## 最佳实践 {#best-practices}

随着主要电子邮件客户端采用深色模式的次数增加，必须考虑您的电子邮件在浅色和深色环境中的呈现方式 — 无论您是否使用[自定义深色模式](#define-custom-dark-mode)。

深色模式可以改变颜色、背景和图像 — 有时会覆盖设计选择。 要确保可视一致性、可访问性和品牌完整性，请遵循下面列出的最佳实践。

**优化您的图像和徽标**

* 将徽标和图标保存为具有透明背景的PNG，以避免在深色模式下显示白色框。

* 避免使用带有硬编码白色或浅色背景的图像。

* 如果无法使用透明度，请将图像置于设计中的纯色背景上，以防止尴尬的颜色反转。

**观看您的背景**

* 确保文本颜色和背景颜色之间的对比度足以在浅色和深色模式下阅读。

* 避免仅依赖背景颜色处理关键内容。 某些客户端在深色模式下会覆盖背景颜色，因此请确保关键信息仍然可见。

**在深色模式下设计可访问的内容**

* 使用颜色组合，易于区分色盲人士。

* 使用中间调调色板确保与明暗背景的对比度。

* 使用具有高对比度的无障碍颜色组合以提高可读性并符合Web内容无障碍准则(WCAG)标准。 使用WebAIM的对比度检查器等工具验证颜色对比度。

* 避免使用细字体，因为它可能会影响可读性。 如果您的品牌需要细字体，请在深色模式下将其粗体。

* 跳过纯黑色的纯白色，因为它可能会导致眼睛疲劳，并且可能会被一些电子邮件客户自动翻转。

* 如果不支持深色模式，请提供可访问的回退样式。

**在深色模式环境中测试电子邮件**

* 使用Email Designer的[深色模式预览](#preview-dark-mode)，该预览使用反转的配色方案来提早发现问题。

* 使用[电子邮件渲染](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md)选项，该选项可利用Litmus在主要电子邮件客户端(Apple Mail、Gmail、Outlook)间模拟您的设计，并查看颜色和图像在深色模式下的行为。

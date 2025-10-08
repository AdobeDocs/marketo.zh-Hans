---
title: 设计可访问的内容
description: 了解如何在Marketo Engage中为您的电子邮件设计无障碍内容。
feature: Email Designer
role: User
level: Beginner, Intermediate
keywords: 电子邮件、设计、辅助功能
source-git-commit: 753455b40ead039a56c595fa61ab9a95b7936382
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 0%

---

# 设计可访问的内容 {#accessible-content}

[欧洲无障碍法](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32019L0882){target="_blank"}是一项指令，旨在通过消除因成员国之间国家规则不同而造成的障碍，增强无障碍产品和服务的内部市场。

这项法规规定，所有数字通信，包括电子邮件、新闻稿、PDF和可下载内容，都应可供访问。 因此，在为收件人创建内容时，需要遵循特定准则，例如使用无障碍字体和可读格式，以及为图像提供替换文本。

Marketo Engage Email Designer根据Web内容无障碍准则(WCAG) 2.1，级别AA，允许您轻松遵守此指令。 下面列出了使用Marketo Engage设计无障碍内容的最佳实践。

>[!NOTE]
>
>本页旨在让所有收件人都能够访问您的内容，以便残障人士能够阅读、理解您在Marketo Engage中设计的电子邮件并与之交互。

## 确保文本可读性 {#text-readability}

利用&#x200B;**[!UICONTROL Styles]**&#x200B;组件的&#x200B;**[!UICONTROL Text]**&#x200B;选项卡确保文本可读，例如使用适当的颜色对比度和简单字体。

<!--![](assets/accessible-text-styles.png){width="80%"}-->

对于字体和文本，请确保遵循以下准则：

**字体选择**

* 使用Arial、Verdana、Tahoma、Helvetica或Open Sans等无衬线字体。
* 避免在正文内容中使用衬线、草稿或装饰性字体。
* 为了一致性和回退，请粘贴到有限的字体集（例如： `font-family: Arial, Helvetica, sans-serif;`）。

**字体大小**

* 确保正文的最小字体大小为16px。
* 为标题使用正确的层次结构。

**颜色对比度**

* 保持文本与背景之间的对比度至少为4.5:1。
* 对于大文本(≥24px或粗体18px)，请确保对比度至少为3:1。
* 避免在白色背景上使用浅灰色或淡色文本。
* 不要仅仅依靠颜色来传达含义。 使用下划线、图标等

**文本辅助功能**

* 避免在图像中使用文本。
* 请勿在正文中使用所有大写字母。
* 确保文本可以缩放到200%而不破坏布局。

## 确保可视辅助功能 {#visual-accessibility}

* 避免使用仅用于颜色指示器的重要信息。
* 为清楚起见，请使用文本标签或图标。
* 针对移动和响应式布局优化您的设计，确保按钮较大且间距适当。
* 定期跨设备和屏幕大小测试以保持可访问性。

在Marketo Engage中，可以使用Email Designer **[!UICONTROL Styles]**&#x200B;窗格中的样式参数和属性进一步细化内容中不同元素的大小和间距。

例如，您可以更新背景或更改边距、填充和对齐来提高可视辅助功能。

<!--![](assets/accessible-styles.png){width="80%"}-->

Marketo Engage Email Designer允许您预览和优化不同设备和屏幕大小的设计。 您随时可以&#x200B;**[!UICONTROL Switch to live view]**&#x200B;检查您的内容在各种设备大小上的呈现方式。

<!--![](assets/accessible-live-view.png){width="80%"}-->

>[!CAUTION]
>
>实时视图是一个通用预览，旨在比较内容在各种设备大小中的呈现方式。 最终渲染可能会因收件人的电子邮件客户端而异。

## 对图像使用替换文本 {#alt-text}

使用&#x200B;**[!UICONTROL Image]**&#x200B;组件为图像提供替换文本。

<!--![](assets/accessible-alt-text.png){width="90%"}-->

* 简洁而符合情境地描述图像的用途。
* 避免使用“图像……”等多余短语，并使用空替换文本作为装饰性图像。
* 对于具有意义的图标，提供有意义的标签；对于复杂的图像，使用简短的替换文本以及在其他位置使用更长的描述。

## 使用可读格式 {#readable-format}

使用电子邮件Designer的相关结构和内容组件以及&#x200B;**[!UICONTROL Styles]**&#x200B;窗格中的选项，以清晰、逻辑和简洁的方式整理您的内容，让所有人都可以访问。

<!--![](assets/accessible-components.png){width="100%"}-->

* 使用结构化、语义化的HTML，并带有适当的标题、段落、列表和表。
* 确保内容遵循从左至右、从上至下的逻辑流程。
* 使用简洁明了的语言。
* 为PDF和信息图形提供替代格式。
* 允许调整文本大小和重排，并确保在所有格式下均可使用足够的颜色对比度读取排版规则。

## 确保内容可读性 {#readability}

要读取，您的内容必须清晰、结构合理，并且可供所有人使用，包括患有视觉、认知或阅读障碍的人以及使用辅助技术的人。 创建无障碍内容时要考虑的一些要点包括：

* 将句子保留在20字或更少的范围内。
* 编辑您的文案以简明扼要。
* 使用主动语态使句子结构更简单。
* 避免使用某些人可能不熟悉的俚语、行话或地区性用语。

为了评估您的电子邮件可读性，您可以使用常用的[Flesch Reading Ease测试](https://support.microsoft.com/en-us/office/get-your-document-s-readability-and-level-statistics-85b4969e-e80a-4777-8dd3-f7fc3c8b3fd2){target="_blank"}，该测试可在Microsoft Word中找到，并以0至100的级数计算内容的阅读方便程度。

## 测试您的内容 {#test}

要验证内容的辅助功能，您可以使用Marketo Engage提供的测试功能。 它们并非专门用于检查您的内容是否完全可访问，但它们可以提供第一级别的验证。

* 使用测试配置文件预览内容。

* 使用[电子邮件渲染](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md){target="_blank"}选项，该选项可利用Litmus在主要电子邮件客户端(Apple Mail、Gmail、Outlook)间模拟您的设计，并查看文本、颜色和图像是否可以访问您的内容。<!--Litmus includes accessibility testing-->

* 在将内容发送到实际受众之前，请发送校样以测试内容的渲染。

<!--![](assets/accessible-simulate.png){width="90%"}-->

如果内容可可靠访问，要以更一致的方式签入，请访问特定的外部工具，例如：

* [WebAim对比度检查器](https://webaim.org/resources/contrastchecker/){target="_blank"}和[WAVE Web辅助功能评估工具](https://wave.webaim.org/){target="_blank"}用于评估对比度和符合性；

* 屏幕阅读器等辅助技术(例如：[NVDA](https://www.nvaccess.org/download/){target="_blank"}或iPhone上的[VoiceOver](https://support.apple.com/en-ie/guide/iphone/iph3e2e415f/ios){target="_blank"})可从视障用户的角度体验电子邮件。

## 使用深色模式 {#dark-mode}

[深色模式](/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md){target="_blank"}增强了对光线敏感或视觉障碍的用户的可视性，以改善观看体验。

<!--![](assets/accessible-dark-mode.png){width="90%"}-->

在深色模式下设计内容的一些最佳实践包括：

* 使用透明PNG或SVG
* 设置相应的元标记和CSS
* 提供可访问的回退样式（如果不支持深色模式）。

通过在浅色和深色模式下测试所有电子邮件内容和UI元素，确保您的电子邮件在深色模式下正确呈现。

## 使用特定属性进行辅助功能 {#attributes}

### 语言属性 {#language}

创建设计时，请在内容正文中包含`lang`（语言）和`dir`（文本方向）属性。 这些属性可帮助辅助技术（如屏幕阅读器）以适当的方式解释和展示您的内容。

* `lang`属性指示发送给辅助技术的电子邮件的语言，确保单词的发音正确。

  +++示例

  英语示例：

  ```
  <body lang="en">
  ```

  法语示例：

  ```
  <body lang="fr">
  ```

  +++

* `dir`属性指定文本方向。 大多数语言，包括英语和法语，从左至右(ltr)阅读，而阿拉伯语和希伯来语等语言从右至左(rtl)阅读。

  +++示例

  英语示例（从左至右）：

  ```html
  <body lang="en" dir="ltr">
  ```

  阿拉伯语示例（从右至左）：

  ```html
  <body lang="ar" dir="rtl">
  ```

  +++

屏幕阅读器依赖于`lang`属性来应用正确的发音规则，而文本方向可确保从左到右或从右到左语言的内容自然流动。 如果没有这些属性，用户可能会遇到阅读顺序混乱或发音错误的情况。 始终使用适当的`lang`和`dir`属性封装您的电子邮件正文。

>[!TIP]
>
>如果电子邮件包含多种语言，请将相应的语言属性分配给特定部分（如`<table>`或`<td>`块），以确保每个部分均可正确读取。

### 表格 {#tables}

在HTML内容中，表格通常用于布局。 默认情况下，屏幕阅读器将每`<table>`视为数据表，声明行、列和结构。 如果表仅用于格式化，这可能会造成混淆。

将`role="presentation"`（或`role="none"`）添加到布局表，以确保辅助型技术跳过其结构并仅关注实际内容。

+++示例 — 布局表（带`role="presentation"`）

```html
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="100%"> 
  <tr> 
    <td align="center"> 
      <h1>Hello World</h1> 
      <p>Welcome to our newsletter</p> 
    </td> 
  </tr> 
</table>
```

屏幕阅读器显示：
“你好，世界。 欢迎收看我们的新闻稿。” _（未提及行、列或表）_

+++

+++示例 — 数据表（不带`role="presentation"`）

```html
<table border="1" cellpadding="5" cellspacing="0">
  <tr>
    <th scope="col">Name</th>
    <th scope="col">Score</th>
  </tr>
  <tr> 
    <td>Peter</td>
    <td>19</td>
  </tr>
  <tr>
    <td>Parker</td>
    <td>62</td>
  </tr>
</table>
```

屏幕阅读器显示：
“带2列3行的表。”

“姓名，彼得。 分数，19。”

“姓名，帕克。 得分，62分。”

+++

>[!TIP]
>
>仅将`role="presentation"`用于布局表。 对于数据表，请保留语义`<table>`结构，以便屏幕阅读器可以正确声明标题和关系。

### 链接文本 {#links}

屏幕阅读器使用文本阅读链接。 如果链接仅标记为“单击此处”或“了解更多”，则使用辅助技术的用户将无法知道目标。 为确保辅助功能，他们需要清晰地指示目标或操作的描述性文本。

使用电子邮件Designer添加指向内容的链接并编辑标签，使其可见（可见）且具有描述性（清除用途）。 避免使用模糊的标签，如“此处”或“更多”。

<!--![](assets/accessible-link.png){width="70%"}-->

+++示例 — 良好链接（描述性）： 

```
<p>Learn more in the  
<a href="https://adobe.com/release-notes">August release notes</a>. 
</p>
```

屏幕阅读器显示：
“Link， 8月发行说明。”

+++

+++示例 — 错误链接（非描述性）

```
<p>Learn more about our new features.  
  <a href="https://adobe.com/release-notes">Click here</a>. 
</p>
```

屏幕阅读器显示：
“链接，单击此处。” *（未提供顺序不正确的上下文）*

+++

<!--for Landing Pages-->

<!--## Provide keyboard navigation and focus support {#keyboard}

Providing keyboard navigation and focus support allows people who cannot use a mouse to fully access and interact with content. It also improves overall usability by giving all users a clear and consistent way to move through information.

* Focus via keyboard
    * Ensure all interactive elements (such as buttons, checkboxes, links) have `tabindex="0"` so they are included in the natural tab order. 
    * Allow navigation using the Tab and arrow keys (↑ ↓ ← →), which should visibly highlight the focused element. 
* Custom focus styling 
    * Apply clear and distinguishable styles for focusing on actionable elements: 
        +++Example (CSS)

        ```
        [tabindex="0"] : focus { 
        outline: 2px solid #00AEEF;  /* Cyan border */ 
        background-color: #20CEFF;   /* Optional background */ 
        }
        ```
        
        +++

    * Ensure that focus indicators meet the WCAG 2.2 focus appearance standards, including: 
        * Minimum area: 2 CSS pixel thick outline.
        * Contrast ratio: ≥ 3:1 between focused and unfocused state. 

* Keyboard activation support 
    * Ensure checkboxes and buttons respond to the Enter and Space keys. 
    * Validate the interaction using the keyboard alone: 
        * Enter or Space should toggle checkboxes.
        * Enter or Space should trigger the buttons.-->

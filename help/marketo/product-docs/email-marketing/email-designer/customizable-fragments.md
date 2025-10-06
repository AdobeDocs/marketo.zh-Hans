---
solution: Marketo Engage
product: marketo
title: 可自定义的片段
description: 了解如何通过使其某些字段可编辑来自定义片段。
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
source-git-commit: cc6c04ca8a72f6efb0bec93cba084fe2993f53f0
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 1%

---

# 可自定义的片段 {#customizable-fragments}

在电子邮件或电子邮件模板中使用片段时，默认情况下会因继承而锁定这些片段。 这意味着对片段所做的任何更改都会自动传播到使用该片段的所有资源。 利用可自定义的片段，在将片段添加到电子邮件或电子邮件模板时，可以将片段中的特定字段定义为可编辑。 例如，假设您有一个带有横幅、一些文本和按钮的片段。 您可以将某些字段（如图像或按钮目标URL）指定为可编辑的。 这允许用户在将片段合并到其电子邮件/电子邮件模板中时修改这些元素，提供定制的体验而不影响原始片段。

利用可自定义的片段，您可以有效地管理和个性化内容，而无需创建全新的内容块或中断原始片段的继承。 这可以确保在片段级别所做的更改仍会传播，同时允许在电子邮件/电子邮件模板级别进行必要的自定义。

可视片段和表达式片段均可以标记为可自定义。 有关如何继续处理每种类型片段的详细说明，请参阅以下部分。

## 在可视片段中添加可编辑字段 {#visual}

要使可视片段的某些部分可编辑，请执行以下步骤：

>[!NOTE]
>
>可编辑的字段可添加到&#x200B;**图像**、**文本**&#x200B;和&#x200B;**按钮**&#x200B;组件中。 对于&#x200B;**HTML**&#x200B;组件，使用个性化编辑器添加可编辑的字段，类似于表达式片段。 [了解如何在HTML组件和表达式片段中添加可编辑字段](#expression)

1. 打开片段内容版本屏幕。

1. 选择片段中要配置可编辑字段的组件。

1. 组件属性窗格将在右侧打开。 选择&#x200B;**[!UICONTROL Editable fields]**&#x200B;选项卡，然后切换&#x200B;**[!UICONTROL Enable edition]**&#x200B;选项。

1. 窗格中列出了可为选定组件编辑的所有字段。 可供编辑的字段取决于所选的组件类型。

   在以下示例中，我们允许编辑“单击此处”按钮URL。

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL Overview]**&#x200B;以检查所有可编辑的字段及其默认值。

   在此示例中，按钮URL字段显示在组件中定义的默认值中。 在将片段添加到用户的内容后，用户可以自定义此值。

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. 完成时保存更改。

将片段添加到电子邮件后，用户将能够自定义片段中配置的所有可编辑字段。
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

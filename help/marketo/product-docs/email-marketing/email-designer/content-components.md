---
solution: Marketo Engage
product: marketo
title: 内容组件
description: 描述。
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: ca8644c43cfbdbaf7be9f21c5e440949b796cfdb
workflow-type: tm+mt
source-wordcount: '1154'
ht-degree: 0%

---

# 内容组件 {#content-components}

在创建电子邮件内容时，**[!UICONTROL Content components]**&#x200B;允许您使用原始组件进一步个性化电子邮件，这些组件一旦放入电子邮件中即可编辑。

您可以根据需要在一个或多个结构组件中添加任意数量的内容组件，这些组件定义电子邮件的布局。

## 添加内容组件 {#add-content-components}

要将内容组件添加到电子邮件并根据需要对其进行调整，请执行以下步骤。

1. 在电子邮件Designer中，使用现有内容或将&#x200B;**[!UICONTROL Structure components]**&#x200B;拖放到空内容中来定义电子邮件的布局。`[Learn how](content-from-scratch.md)`

1. 要访问&#x200B;**[!UICONTROL Content components]**&#x200B;部分，请从Email Designer左窗格中选择对应的按钮。

   屏幕快照

1. 将您选择的内容组件拖放到相关结构组件中。

   屏幕快照

   >[!NOTE]
   >
   >可以将多个组件添加到单个结构组件中，并添加到结构组件的每一列中。

1. 使用右侧的&#x200B;**[!UICONTROL Settings]**&#x200B;和&#x200B;**[!UICONTROL Style]**&#x200B;选项卡调整每个组件的属性和样式。 例如，可以更改每个组件的文本样式、填充或边距。`[Learn more about alignment and padding](alignment-and-padding.md)`

   屏幕快照

1. 通过&#x200B;**[!UICONTROL Content component]**&#x200B;的高级菜单，您可以根据需要轻松删除或复制任何内容组件。

   屏幕快照

## 容器 {#container}

要将特定样式应用于一组内容组件，您可以添加&#x200B;**[!UICONTROL Container]**&#x200B;组件，然后在其中添加所需的内容组件。 这允许您向容器应用不同的样式，这与应用于内部内容组件的样式不同。

例如，添加一个&#x200B;**[!UICONTROL Container]**&#x200B;组件，然后在该容器中添加一个[Button](#button)组件。 您可以为容器使用特定的背景，为按钮使用另一个背景。

屏幕快照

## 按钮 {#button}

使用&#x200B;**[!UICONTROL Button]**&#x200B;组件在电子邮件中插入一个或多个按钮，并将电子邮件受众重定向到其他页面。

1. 从&#x200B;**[!UICONTROL Content components]**，将&#x200B;**[!UICONTROL Button]**&#x200B;组件拖放到&#x200B;**[!UICONTROL Structure component]**&#x200B;中。

1. 单击新添加的按钮以个性化文本，并访问“电子邮件Designer”右窗格中的&#x200B;**[!UICONTROL Settings]**&#x200B;和&#x200B;**[!UICONTROL Styles]**&#x200B;选项卡。

   屏幕快照

1. 从&#x200B;**[!UICONTROL Link]**&#x200B;菜单中，添加单击按钮时要重定向到的URL。

1. 使用&#x200B;**[!UICONTROL Target]**&#x200B;下拉列表选择重定向受众的方式：

   * **[!UICONTROL None]**：在与单击链接相同的帧中打开该链接（默认）。
   * **[!UICONTROL Blank]**：在新窗口或选项卡中打开链接。
   * **[!UICONTROL Self]**：在单击链接的同一帧中打开该链接。
   * **[!UICONTROL Parent]**：在父框架中打开链接。
   * **[!UICONTROL Top]**：在窗口的整个正文中打开链接。

   屏幕快照

1. 您可以通过更改样式属性（如&#x200B;**[!UICONTROL Border]**、**[!UICONTROL Size]**、**[!UICONTROL Margin]**&#x200B;等）进一步个性化您的按钮。 从&#x200B;**[!UICONTROL Component settings]**&#x200B;窗格。

## 文本 {#text}

使用&#x200B;**[!UICONTROL Text]**&#x200B;组件将文本插入电子邮件，并使用&#x200B;**[!UICONTROL Styles]**&#x200B;选项卡调整样式（边框、大小、填充等）。

屏幕快照

1. 从&#x200B;**[!UICONTROL Content components]**，将&#x200B;**[!UICONTROL Text]**&#x200B;组件拖放到&#x200B;**[!UICONTROL Structure component]**&#x200B;中。

1. 单击新添加的组件以个性化文本，并访问Email Designer右侧窗格中的&#x200B;**[!UICONTROL Settings]**&#x200B;和&#x200B;**[!UICONTROL Styles]**&#x200B;选项卡。

1. 使用工具栏中可用的以下选项更改文本：

   屏幕快照

   * **[!UICONTROL Change text style]**：对您的文本应用粗体、斜体、下划线或删除线。
   * **更改对齐方式**：选择文字的左对齐、右对齐、居中对齐或两端对齐方式。
   * **[!UICONTROL Create list]**：在文本中添加项目符号或编号列表。
   * **[!UICONTROL Set heading]**：为您的文本添加最多六个标题级别。
   * **字体大小**：选择文本的字体大小（像素）。
   * **[!UICONTROL Change font color]**：选择字体的颜色。
   * **[!UICONTROL Insert link]**：向内容添加任何类型的链接。
   * **[!UICONTROL Edit image]**：将图像或资源添加到文本组件。`[Learn more about asset management](../integrations/assets.md)`
   * **[!UICONTROL Change font color]**：选择字体的颜色。
   * **[!UICONTROL Add personalization]**：添加个性化字段以自定义配置文件数据的内容。`[Learn more about content personalization](../personalization/personalize.md)`
   * **[!UICONTROL Show the source code]**：显示文本的源代码。 无法修改它。
   * **[!UICONTROL Enable conditional content]**：添加条件内容以将组件的内容调整到目标配置文件。`[Learn more about dynamic content](../personalization/get-started-dynamic-content.md)`
   * **[!UICONTROL Duplicate]**：添加文本组件的副本。
   * **[!UICONTROL Delete]**：从电子邮件中删除所选的文本组件。

1. 调整其他样式属性，如文本颜色、字体系列、边框、填充、边距等。 从&#x200B;**[!UICONTROL Styles]**&#x200B;选项卡。

   屏幕快照

## 分隔条 {#divider}

使用&#x200B;**[!UICONTROL Divider]**&#x200B;组件插入分隔线来组织电子邮件的布局和内容。

您可以从&#x200B;**[!UICONTROL Settings]**&#x200B;和&#x200B;**[!UICONTROL Styles]**&#x200B;选项卡中调整样式属性，例如线条的颜色、样式和高度。

屏幕快照

## HTML {#HTML}

使用&#x200B;**[!UICONTROL HTML]**&#x200B;组件复制并粘贴现有HTML的各个部分。 这使您能够创建免费的模块化HTML组件以重用某些外部内容。

1. 从&#x200B;**[!UICONTROL Content Components]**，将&#x200B;**[!UICONTROL HTML]**&#x200B;组件拖放到&#x200B;**[!UICONTROL Structure component]**&#x200B;中。

1. 单击新添加的组件，然后从上下文工具栏中选择&#x200B;**[!UICONTROL Show the source code]**&#x200B;以添加您的HTML。

   屏幕快照

1. 复制并粘贴要添加到电子邮件中的HTML代码，然后单击&#x200B;**[!UICONTROL Save]**。

   屏幕快照

>[!NOTE]
>
>为了仅使外部内容与Email Designer兼容，Adobe建议从头开始创建消息，并将现有电子邮件的内容复制到组件中。

## 图像 {#image}

使用&#x200B;**[!UICONTROL Image]**&#x200B;组件将图像文件从计算机插入到电子邮件内容中。

1. 从&#x200B;**[!UICONTROL Content components]**，将&#x200B;**[!UICONTROL Image]**&#x200B;组件拖放到&#x200B;**[!UICONTROL Structure component]**&#x200B;中。

   屏幕快照

1. 在&#x200B;**[!UICONTROL Settings]**&#x200B;选项卡中，单击&#x200B;**[!UICONTROL Browse]**&#x200B;以从资源中选择图像文件，或单击&#x200B;**[!UICONTROL Import media]**&#x200B;以将资源上传到Adobe Experience Manager Assets。

   要了解有关[!DNL Adobe Experience Manager Assets]的更多信息，请参阅[Adobe Experience Manager Assets文档](https://experienceleague.adobe.com/docs/experience-manager-assets-essentials/help/introduction.html?lang=zh-Hans){target="_blank"}。

   >[!NOTE]
   >
   > 为了确保您的链接保持活动状态并避免任何过期问题，我们建议使用Adobe Assets而不是依赖图像的源URL。

1. 您还可以使用&#x200B;**[!UICONTROL Find Adobe Stock photos]**&#x200B;选项直接在Adobe Stock中搜索。

1. 单击新添加的组件并设置图像属性：

   * **[!UICONTROL Image title]**&#x200B;允许您定义图像的标题。
   * **[!UICONTROL Alt text]**&#x200B;允许您定义链接到图像的描述。 此选项对应于alt HTML属性。

   屏幕快照

1. 您还可以选择&#x200B;**[!UICONTROL Find similar Stock photos]**。`[Learn more](../integrations/stock.md)`

1. 在&#x200B;**[!UICONTROL Styles]**&#x200B;选项卡中，调整其他样式属性，如边距、边框等。 或添加链接以将受众重定向到&#x200B;**[!UICONTROL Component settings]**&#x200B;窗格中的其他内容。

## 社交 {#social}

使用&#x200B;**[!UICONTROL Social]**&#x200B;组件将指向社交媒体页面的链接插入到您的电子邮件内容中。

1. 从&#x200B;**[!UICONTROL Content Components]**，将&#x200B;**[!UICONTROL Social]**&#x200B;组件拖放到&#x200B;**[!UICONTROL Structure component]**&#x200B;中。

1. 选择新添加的组件。

1. 在&#x200B;**[!UICONTROL Social]**&#x200B;选项卡的&#x200B;**[!UICONTROL Settings]**&#x200B;字段中，选择要添加或删除的社交媒体。

   屏幕快照

1. 通过专用字段选择图标的大小。

1. 单击每个社交媒体图标可配置受众将被重定向到的&#x200B;**[!UICONTROL URL]**。

   屏幕快照

1. 如果需要，您还可以从Assets中更改每个社交媒体的图标。

1. 调整其他样式属性，如样式、边距、边框等。 从&#x200B;**[!UICONTROL Styles]**&#x200B;选项卡。

## 优惠决策 {#offer-decision}

使用&#x200B;**[!UICONTROL Offer decision]**&#x200B;组件将选件插入到消息中。 `[decision management](../offers/get-started/starting-offer-decisioning.md)`引擎将选取要交付给客户的最佳选件。

1. 从&#x200B;**[!UICONTROL Content Components]**，将&#x200B;**[!UICONTROL Offer decision]**&#x200B;组件拖放到&#x200B;**[!UICONTROL Structure component]**&#x200B;中。

1. 单击&#x200B;**[!UICONTROL Add]**&#x200B;以选择您的&#x200B;**[!UICONTROL Offer decision]**。

   屏幕快照

1. 从下拉菜单中选择您的&#x200B;**[!UICONTROL Placements]**。  然后，选择要添加到内容中的&#x200B;**[!UICONTROL Offer decision]**&#x200B;并单击&#x200B;**[!UICONTROL Add]**。

   屏幕快照

1. 在&#x200B;**[!UICONTROL Offer decision]**&#x200B;选项卡中，您可以预览或更改插入的选件。

了解如何在`[this section](add-offers-email.md)`中将个性化优惠添加到电子邮件中。

>[!IMPORTANT]
>
>如果对历程消息中使用的优惠决策进行了更改，则需要取消发布该历程并重新发布。  这将确保将更改纳入历程的消息中，并且消息与最新更新一致。


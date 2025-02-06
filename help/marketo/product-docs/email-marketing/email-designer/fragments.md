---
title: 片段
description: 了解如何创建可视化内容片段，并将其用作电子邮件和电子邮件模板的可重用组件。
hide: true
hidefromtoc: true
exl-id: abc065a0-cd2f-4f0f-a5f2-228b833b99a8
source-git-commit: 92404e10771920862cd147c09e2ada37484e6118
workflow-type: tm+mt
source-wordcount: '2052'
ht-degree: 1%

---

# 片段

片段是可重用组件，可在一个或多个电子邮件和电子邮件模板中引用。 它通常是可快速插入到项目中的内容块（文本、图像或两者）。 利用此功能，您可以预构建多个自定义内容块以组合电子邮件内容，从而改进设计过程。 常见用例包括电子邮件的页眉/页脚内容块、事件邀请横幅、季节性消息等。

要在工作流中充分利用片段，请执行以下操作：

* _创建片段_ — 从头开始创建可视化片段，或从可视化内容编辑器中将内容另存为片段。
* _重用片段_ — 根据需要多次在内容中使用它们。

## 可视化片段 {#visual-fragments}

可视化片段是预定义的可视化块，可使用可视内容编辑器构建，可在多个电子邮件或电子邮件模板中重复使用。

## 访问和管理片段 {#access-and-manage-fragments}

要访问可视化片段，请转到Marketo Engage中的&#x200B;**设计工作室**。 在左侧的树中，单击&#x200B;**[!UICONTROL 片段（新）]**。

![访问片段](assets/access-and-manage-fragments-1.png){width="600" zoomable="yes"}

默认情况下，该表按&#x200B;_[!UICONTROL Modified]_&#x200B;列排序。 单击其他列标题以更改表的排序依据。 再次单击同一标题可在升序和降序之间切换。

### 查找和筛选

使用搜索栏按名称查找片段。 单击&#x200B;_筛选器_&#x200B;图标（![筛选器图标](assets/icon-filter.svg)）以显示可用的筛选器选项并选择所需的设置。

![筛选显示的片段](assets/access-and-manage-fragments-2.png){width="700" zoomable="yes"}

### 自定义列 {#customize-the-column-display}

通过单击右上角的&#x200B;_自定义表_&#x200B;图标（![自定义表图标](assets/icon-column-settings.svg)）自定义要在表中显示的列。

选择所需的列，然后单击&#x200B;**[!UICONTROL 应用]**。

![自定义表模式](assets/access-and-manage-fragments-3.png){width="400" zoomable="yes"}

### 片段状态 {#fragment-status}

片段状态决定了在电子邮件或电子邮件模板中使用的可用性，以及您可以对其进行的更改。

<table>
<tbody>
  <tr>
    <td><b>草稿</b></td>
    <td>创建片段时，它处于草稿状态。 在发布它以用于电子邮件或电子邮件模板之前，它仍为草稿。
    <p>可用操作：
    <li>编辑所有详细信息</li>
    <li>在可视设计器中编辑</li>
    <li>发布</li>
    <li>复制</li>
    <li>Delete</li>
  </td>
  <tr>
    <td><b>发布日期</b></td>
    <td>发布片段后，该片段将可用于电子邮件或电子邮件模板。 在可视设计器中无法修改已发布的片段内容。
    <p>可用操作：
    <li>编辑描述</li>
    <li>添加到电子邮件或模板</li>
    <li>创建草稿版本</li>
    <li>复制</li>
    <li>删除（如果未使用）</li>
    </td>
  </tr>
  <tr>
    <td><b>以草稿发布</b></td>
    <td>从已发布的片段创建草稿时，已发布的版本仍然可用于电子邮件或电子邮件模板，并且草稿内容可以在可视设计器中进行修改。 如果您发布草稿版本，它将替换当前已发布的版本，并且内容将在<i>所有</i>正在使用草稿的电子邮件和电子邮件模板中更新。 
    <p>可用操作：
    <li>编辑描述</li>
    <li>添加到电子邮件或模板</li>
    <li>在可视设计器中编辑草稿版本</li>
    <li>Publish草稿版本</li>
    <li>复制</li>
    <li>删除（如果未使用）</li>
    </td>
  </tr>
</tbody></table>

## 创建片段 {#create-fragments}

1. 要创建新的可视片段，请单击片段列表页面右上角的&#x200B;**[!UICONTROL 创建片段]**。

   ![创建片段按钮](assets/create-fragments-1.png){width="700" zoomable="yes"}

1. 为您的片段提供&#x200B;**[!UICONTROL 名称]**&#x200B;和可选的&#x200B;**[!UICONTROL 描述]**。

   _片段要求_

   * 名称：最多100个字符，必须是唯一的，不区分大小写
   * 描述：最多300个字符
   * 字符：可使用字母、数字和特殊字符
   * 保留字符为&#x200B;**_不允许_**： `\ / : * ? " < > |`

   ![创建片段模式](assets/create-fragments-2.png){width="400" zoomable="yes"}

1. 单击&#x200B;**[!UICONTROL 创建]**。

   ![创建片段模式](assets/create-fragments-3.png){width="400" zoomable="yes"}

   >[!NOTE]
   >
   >此时无法修改片段的&#x200B;**类型**。

   此时会打开可视设计器，并显示一个空画布。

1. 使用内容设计工具创建可视化片段内容：

   * [添加结构和内容](#add-structure-and-content)
   * [添加Assets](#add-assets)
   * [导航图层、设置和样式](#navigate-the-layers-settings-and-styles)
   * [使内容个性化](#personalize-content)
   * [编辑链接的URL跟踪](#edit-linked-url-tracking)

1. 随时单击&#x200B;**[!UICONTROL 保存]**&#x200B;以保存草稿片段。

1. 当您准备好在电子邮件或电子邮件模板中使用片段时，请单击&#x200B;**[!UICONTROL Publish]**。

### 添加结构和内容 {#add-structure-and-content}

{{$include /help/marketo/_includes/content-design-components.md}}

### 添加资源

{{$include /help/_includes/content-design-assets.md}}

### 导航图层、设置和样式

{{$include /help/_includes/content-design-navigation.md}}

### 使内容个性化

{{$include /help/_includes/content-design-personalization.md}}

### 编辑链接的URL跟踪

{{$include /help/_includes/content-design-links.md}}

## 查看片段详细信息 {#view-fragment-details}

单击列表页面中任何片段的名称以打开片段详细信息页面。 您可以选择编辑片段、重命名片段或更新其描述。 进行更新，然后单击名称或描述字段外部以保存更改。

>[!NOTE]
>
>如果电子邮件或电子邮件模板正在使用已发布的片段，则无法更改其名称或编辑内容。 如果要对片段进行更改，可以创建草稿版本。

![查看已发布片段的详细信息](assets/view-fragment-details-1.png){width="600" zoomable="yes"}

单击&#x200B;**[!UICONTROL 编辑片段]**&#x200B;以在可视内容编辑器中打开该片段。

单击左上角的&#x200B;_返回_&#x200B;箭头可随时退出视图，该箭头将返回到&#x200B;_片段_&#x200B;列表页面。

## 引用使用的视图片段 {#view-fragment-used-by-references}

在片段详细信息页面中，单击&#x200B;**[!UICONTROL 使用者]**&#x200B;选项卡以查看在Marketo Engage中使用片段的位置的详细信息。

>[!IMPORTANT]
>
>无法删除电子邮件或电子邮件模板当前正在使用的片段。

![由对片段的引用使用](assets/view-fragment-used-by-1.png){width="600" zoomable="yes"}

单击链接以打开相应的电子邮件或电子邮件模板，其中使用该片段。

## 删除片段 {#delete-fragments}

由于无法删除电子邮件或电子邮件模板当前正在使用的片段，因此，在启动片段移除之前，请务必检查&#x200B;_used-by_&#x200B;引用。 此外，删除操作无法撤消，因此在启动删除操作之前请检查。

您可以使用以下任一方法删除片段：

* 从右侧的片段详细信息中，单击&#x200B;**[!UICONTROL 删除]**。
* 从&#x200B;_[!UICONTROL 片段]_&#x200B;列表页面，单击片段旁边的省略号并选择&#x200B;**[!UICONTROL 删除]**。

此操作将打开确认对话框。 您可以通过单击&#x200B;**[!UICONTROL 取消]**&#x200B;或单击&#x200B;**[!UICONTROL 删除]**&#x200B;确认删除来中止该进程。

![删除片段对话框](assets/fragment-delete-dialog.png){width="400"}

## 编辑片段 {#edit-fragments}

对片段的编辑取决于其当前状态：

* 当片段处于&#x200B;_草稿_&#x200B;状态时，您可以编辑其任何详细信息和可视内容。
* 当片段处于&#x200B;_已发布_&#x200B;状态时，您可以编辑片段描述，但不能编辑名称。 无法编辑可视内容。
* 当片段处于&#x200B;_已发布，状态为_&#x200B;草稿时，编辑详细信息仅限于描述。 您还可以编辑草稿版本的可视内容。

>[!BEGINTABS]

>[!TAB 草稿]

1. 从&#x200B;_[!UICONTROL 片段]_&#x200B;列表页面，单击片段名称以将其打开。

   随后将显示可视内容的预览，其中片段详细信息位于右侧。

1. 进行所需的编辑。

   ![具有草稿状态的片段的详细信息](assets/fragment-draft-details.png){width="600" zoomable="yes"}

1. 要对可视设计器中的内容进行更改，请单击&#x200B;**[!UICONTROL 编辑片段]**。

   根据需要使用可视设计器工具：

   * [添加结构和内容](#add-structure-and-content)
   * [添加Assets](#add-assets)
   * [导航图层、设置和样式](#navigate-the-layers-settings-and-styles)
   * [使内容个性化](#personalize-content)
   * [编辑链接的URL跟踪](#edit-linked-url-tracking)

   单击&#x200B;**[!UICONTROL 保存]**，或单击&#x200B;**[!UICONTROL 保存并关闭]**&#x200B;以返回片段详细信息。

1. 如果片段符合您的条件并且您想在电子邮件或电子邮件模板中使用它，请单击&#x200B;**[!UICONTROL Publish]**。

>[!TAB 已发布]

1. 从&#x200B;_[!UICONTROL 片段]_&#x200B;列表页面，单击片段名称以将其打开。

   随后将显示可视内容的预览，其中片段详细信息位于右侧。

1. 如果需要，请修改说明。

   对于已发布的片段，无法更改所有其他详细信息。

1. 如果要更新内容，请单击右上方的&#x200B;**[!UICONTROL 创建草稿版本]**。

   在对话框中单击&#x200B;**[!UICONTROL 确定]**&#x200B;以在可视设计器中打开草稿版本。 您可以根据需要更改`image source`公斤 — 链接此处。

   ![创建草稿版本对话框](assets/fragments-create-draft-version.png){width="300"}

   根据需要使用可视设计器工具：

   * [添加结构和内容](#add-structure-and-content)
   * [添加Assets](#add-assets)
   * [导航图层、设置和样式](#navigate-the-layers-settings-and-styles)
   * [使内容个性化](#personalize-content)
   * [编辑链接的URL跟踪](#edit-linked-url-tracking)

   单击&#x200B;**[!UICONTROL 保存]**，或单击&#x200B;**[!UICONTROL 保存并关闭]**&#x200B;以返回片段详细信息。

1. 当草稿片段符合您的条件并且您想要使更改可用于电子邮件或电子邮件模板时，请单击&#x200B;**[!UICONTROL Publish]**。

   发布草稿版本时，草稿版本会替换当前已发布的版本，并且内容会在电子邮件和电子邮件模板中更新（该模板已在使用中）。

>[!TAB 已发布草稿]

有两种方法可以打开草稿版本以从&#x200B;_[!UICONTROL 片段]_&#x200B;列表页面进行编辑：

* 单击片段名称旁边的&#x200B;_更多_&#x200B;图标(**...**)，然后选择&#x200B;**[!UICONTROL 打开草稿版本]**。

  ![打开草稿版本](assets/fragments-create-draft-version.png){width="300"}

* 单击片段名称以将其打开。 然后，单击右上方的&#x200B;**[!UICONTROL 打开草稿版本]**。

  将显示草稿版本的可视内容预览，其中片段详细信息位于右侧。

要更新内容，请执行以下操作：

1. 单击右上方的&#x200B;**[!UICONTROL 编辑片段]**。 根据需要使用可视设计器工具：

   * [添加结构和内容](#add-structure-and-content)
   * [添加Assets](#add-assets)
   * [导航图层、设置和样式](#navigate-the-layers-settings-and-styles)
   * [使内容个性化](#personalize-content)
   * [编辑链接的URL跟踪](#edit-linked-url-tracking)

   单击&#x200B;**[!UICONTROL 保存]**，或单击&#x200B;**[!UICONTROL 保存并关闭]**&#x200B;以返回片段详细信息。

1. 当草稿片段符合您的条件并且您想要使更改可用于电子邮件或电子邮件模板时，请单击&#x200B;**[!UICONTROL Publish]**。

   发布草稿版本时，草稿版本会替换当前已发布的版本，并且内容会在电子邮件和电子邮件模板中更新（该模板已在使用中）。

>[!ENDTABS]

## 重复片段 {#duplicate-fragments}

您可以使用以下任一方法复制片段：

* 从&#x200B;_[!UICONTROL 片段]_&#x200B;列表页面，单击片段名称旁边的&#x200B;_更多_&#x200B;图标(**...**)，然后选择&#x200B;**[!UICONTROL 复制]**。
* 在片段详细信息页面的右上方，单击&#x200B;**[!UICONTROL ...更多]**&#x200B;并选择&#x200B;**[!UICONTROL 复制]**。

![复制片段](assets/fragment-details-duplicate.png){width="600" zoomable="yes"}

在对话框中，输入唯一名称和可选描述。 单击&#x200B;**[!UICONTROL 复制]**&#x200B;以完成操作。

![输入复制的片段的名称和描述](assets/fragment-duplicate-dialog.png){width="400"}

然后，复制的片段出现在&#x200B;_片段_&#x200B;列表中。

## 从电子邮件或模板内容保存新片段 {#save-a-new-fragment-from-email-or-template-content}

在可视内容编辑器中创建/编辑电子邮件或电子邮件模板时，可以将全部或部分内容另存为片段，以便重用。

1. 要将内容另存为片段，请单击&#x200B;**[!UICONTROL 更多]**，然后选择&#x200B;**[!UICONTROL 另存为片段]**。

1. 选择要包含在片段中的不同元素。

   按住Shift或Control按钮选择多个结构。

   您只能选择彼此相邻的结构，并且接口不允许您选择非相邻元素。

1. 选择内容后，单击右上方的&#x200B;**[!UICONTROL 创建]**。

1. 在对话框中，输入片段的名称和可选描述，然后单击&#x200B;**[!UICONTROL 创建]**。

   然后，片段将显示在&#x200B;_片段_&#x200B;列表页面中，并可用于电子邮件和电子邮件模板。

## 将可视化片段添加到您的电子邮件或模板内容 {#add-visual-fragments-to-your-email-or-template-content}

片段设计用于重用。 您最多可以在电子邮件或电子邮件模板中添加30个，并且它们只能嵌套至一个级别。

* [向电子邮件添加片段](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#add-fragments)

* [向电子邮件模板添加片段](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#add-fragments)

片段的内容在结构中动态更新，以呈现内容在电子邮件中如何显示的可视化。

>[!TIP]
>
>如果希望片段占据电子邮件中的整个水平布局，请添加[!UICONTROL 1:1列]结构，然后将片段拖放到其中。

保存电子邮件/电子邮件模板后，在选择&#x200B;_[!UICONTROL 使用者]_&#x200B;选项卡时，该模板会显示在片段详细信息页面中。 添加的片段在电子邮件或模板中不可编辑 — 发布的源片段定义内容。

## 电子邮件和模板创作期间的片段操作 {#fragment-actions-during-email-and-template-authoring}

将片段添加到电子邮件或电子邮件模板时，无法在电子邮件或模板中编辑其内容。 但是，您可以应用以下操作：

* **[!UICONTROL 删除]** — 这将从当前电子邮件或电子邮件模板内容中删除片段（片段源不受影响）。
* **[!UICONTROL 刷新]** — 这将刷新当前电子邮件或电子邮件模板中片段的内容。 当您想要反映在添加到电子邮件或电子邮件模板之后对片段进行的任何最近编辑时，刷新很有用。
* **[!UICONTROL 重复]** — 这会在编辑器的同一电子邮件或电子邮件模板中复制片段。 复制的片段将添加到原始片段的正下方。
* **[!UICONTROL 打开片段]** — 这将打开一个新的浏览器选项卡，其中包含片段编辑器页面和详细信息。
* **[!UICONTROL 中断继承]** — 这将中断片段从源的继承（及其更改）。 使用此操作可以在电子邮件或电子邮件模板中作为独立的可编辑内容使用片段内容。 此操作还会从原始片段的&#x200B;_Used By_&#x200B;引用中删除电子邮件或电子邮件模板。

在编辑器页面上选择片段时，可以从右侧的上下文工具栏和属性面板中执行这些操作。

![将操作应用于所选片段](assets/fragment-actions-email-authoring.png){width="600" zoomable="yes"}

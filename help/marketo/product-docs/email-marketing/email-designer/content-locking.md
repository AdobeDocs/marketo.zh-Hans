---
solution: Marketo Engage
product: marketo
title: 锁定电子邮件模板中的内容
description: 了解如何在电子邮件模板中锁定内容。
level: Beginner, Intermediate
feature: Email Designer
exl-id: 7ccff4f0-5db5-4dd7-91e0-d2081b74ad18
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 8%

---

# 锁定电子邮件模板中的内容 {#lock-content-email-templates}

Marketo Engage允许您通过锁定整个模板或特定结构/组件来锁定电子邮件模板中的内容。 这样可防止无意中编辑或删除内容，让您更好地控制模板自定义，并提高电子邮件营销活动的效率和可靠性。

>[!AVAILABILITY]
>
>具有创建内容模板权限的用户可以启用内容锁定。

可在&#x200B;**结构**&#x200B;级别或&#x200B;**组件**&#x200B;级别应用内容锁定。

* 锁定结构时：

   * 该结构中的所有内容也将被锁定。
   * 无法向结构添加任何内容。
   * 默认情况下，无法删除结构。 您可以通过启用“允许删除”选项来覆盖此限制。
   * 可以将锁定结构中的各个内容组件设置为可编辑。

* 当结构可编辑（结构未锁定）时：

   * 可以将各个内容组件锁定在该结构内。
   * 默认情况下，如果组件已锁定，或者选择了“仅可编辑的内容锁定”，则无法删除组件。 您可以通过启用“允许删除”选项来覆盖此限制。

## 锁定电子邮件模板 {#lock-an-email-template}

### 启用内容锁定 {#enable-content-locking}

无论您是要创建新模板还是要编辑现有模板，都可以直接在Email Designer中为电子邮件模板启用内容锁定。

1. 打开或创建电子邮件模板，并在电子邮件Designer中访问内容编辑屏幕。

1. 在右侧的&#x200B;**[!UICONTROL Body]**&#x200B;窗格中，启用&#x200B;**[!UICONTROL Governance]**&#x200B;选项。

1. 从&#x200B;**[!UICONTROL Mode]**&#x200B;下拉列表中，为模板选择所需的锁定模式：

   * **[!UICONTROL Content locking]**：锁定模板中内容的特定部分。 默认情况下，所有结构和组件都变为可编辑状态。 然后，您可以选择性地锁定各个元素。
   * **[!UICONTROL Read only]**：锁定模板的整个内容，防止进行任何修改。

   ![](assets/content-locking-1.png){width="800" zoomable="yes"}

1. 如果您选择了&#x200B;**[!UICONTROL Content locking]**&#x200B;模式，则可以进一步定义用户与模板的交互方式。 启用&#x200B;**[!UICONTROL Enable content edition]**&#x200B;选项并选择下列选项之一：

   * **[!UICONTROL Allow structure & content addition]**：用户可以在现有结构之间添加结构，并在可编辑的结构中添加内容组件或片段。

   * **[!UICONTROL Allow content addition only]**：用户可以在可编辑的结构中添加内容组件或片段，但无法添加或复制结构。

1. 选择锁定模式后，您可以定义在选择&#x200B;**[!UICONTROL Content locking]**&#x200B;模式时要锁定的结构和/或组件：

   * [了解如何锁定结构](#lock-structures)
   * [了解如何锁定组件](#lock-components)

   如果选择&#x200B;**[!UICONTROL Read only]**&#x200B;模式，则可以继续完成并保存模板。

在设计模板时，您可以通过选择模板正文随时调整&#x200B;**[!UICONTROL Governance]**&#x200B;设置。 为此，请单击位于右侧窗格顶部的导航边栏中的&#x200B;**[!UICONTROL Body]**&#x200B;链接。

![](assets/content-locking-2.png){width="800" zoomable="yes"}

### 锁定结构 {#lock-structures}

要在模板中锁定结构，请执行以下操作：

1. 选择要锁定的结构。

1. 在&#x200B;**[!UICONTROL Lock type]**&#x200B;下拉列表中选择&#x200B;**[!UICONTROL Locked]**。

   ![](assets/content-locking-3.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >默认情况下，用户不能删除已锁定的结构。您可以通过启用&#x200B;**[!UICONTROL Allow delete]**&#x200B;选项来覆盖此限制。

锁定结构后，无法再复制内容组件或片段或将其添加到其中。 缺省情况下，锁定结构内的所有元件也被锁定。 要使组件在锁定的结构中可编辑，请执行以下操作：

1. 选择要解锁的组件。

1. 启用&#x200B;**[!UICONTROL Use specific locking]**&#x200B;选项。

1. 在&#x200B;**[!UICONTROL Lock type]**&#x200B;下拉列表中选择&#x200B;**[!UICONTROL Editable]**。 要在锁定样式时允许编辑内容，请选择&#x200B;**[!UICONTROL Editable content only]**。 [了解如何锁定组件](#lock-components)

   ![](assets/content-locking-4.png){width="800" zoomable="yes"}

### 锁定组件 {#lock-components}

要在结构内锁定特定组件，请执行以下操作：

1. 选择组件并在右窗格中启用&#x200B;**[!UICONTROL Use specific locking]**&#x200B;选项。

1. 从&#x200B;**[!UICONTROL Lock type]**&#x200B;下拉列表中，选择首选锁定选项：

   ![](assets/content-locking-5.png){width="800" zoomable="yes"}

   * **[!UICONTROL Editable content lock only]**：锁定组件的样式，但允许编辑内容。
   * **[!UICONTROL Locked]**：完全锁定组件的内容和样式。

   >[!NOTE]
   >
   >**[!UICONTROL Editable]**&#x200B;锁定类型允许用户编辑组件，即使在锁定的结构内也是如此。 [了解如何锁定结构](#lock-structures)

1. 默认情况下，用户无法删除锁定的组件。 您可以通过激活&#x200B;**[!UICONTROL Allow delete]**&#x200B;选项来启用删除。

### 识别锁定的内容 {#identify-locked-content}

要轻松识别模板中锁定的结构和组件，请使用左侧菜单中的&#x200B;**[!UICONTROL Navigation tree]**。 此菜单提供了所有模板元素的可视化概述，其中以锁图标突出显示锁定的项目，以铅笔图标突出显示可编辑的项目。

在以下示例中，为模板正文启用了管理。 *结构2*&#x200B;已锁定，并且&#x200B;*组件1*&#x200B;可编辑，而&#x200B;*结构3*&#x200B;已完全锁定。

![](assets/content-locking-6.png){width="800" zoomable="yes"}

## 使用具有已锁定内容的模板 {#use-templates-with-locked-content}

使用包含锁定内容的模板时，右侧窗格中会显示&#x200B;**[!UICONTROL Governance enabled]**&#x200B;消息。

根据应用于模板的锁定类型，您可以对模板的结构和组件执行不同的操作。要快速识别模板中的所有可编辑区域，请启用&#x200B;**[!UICONTROL Highlight editable areas]**&#x200B;选项。

例如，在下面的模板中，除了已锁定的顶部图像之外，所有区域都可以编辑，这意味着您无法编辑或删除它。

![](assets/content-locking-7.png){width="800" zoomable="yes"}

以下是已设置的电子邮件编辑和相关内容锁定配置的一些示例：

<table>
<thead>
  <tr>
    <th>内容锁定类型</th>
    <th>模板配置</th>
    <th>电子邮件编辑</th>
  </tr></thead>
<tbody>
  <tr>
    <td>只读内容模板</td>
    <td><img src="assets/locking-sample-read-only-conf.png" width="166" height="60" class="modal-image"></td>
    <td><img src="assets/locking-sample-read-only.png" width="92" height="34" class="modal-image"></td>
  </tr>
  <tr>
    <td>完整内容可编辑，但用户无法添加任何结构或组件</td>
    <td><img src="assets/locking-sample-no-addition-conf.png" width="166" height="68" class="modal-image"></td>
    <td><img src="assets/locking-sample-no-addition.png" width="92" height="36" class="modal-image"></td>
  </tr>
  <tr>
    <td>无法删除的锁定结构</td>
    <td><img src="assets/locking-sample-structure-locked-conf.png" width="166" height="45" class="modal-image"></td>
    <td><img src="assets/locking-sample-structure-locked.png" width="92" height="25" class="modal-image"></td>
  </tr>
  <tr>
    <td>具有锁定样式且无法删除的组件。 用户只能修改内容。</td>
    <td><img src="assets/locking-sample-content-only-conf.png" width="166" height="61" class="modal-image"></td>
    <td><img src="assets/locking-sample-content-only.png" width="92" height="33" class="modal-image"></td>
  </tr>
  <tr>
    <td>锁定结构中的可编辑组件。</td>
    <td><img src="assets/locking-sample-editable-component-conf.png" width="166" height="43" class="modal-image"></td>
    <td><img src="assets/locking-sample-editable-component.png" width="92" height="23" class="modal-image"></td>
  </tr>
</tbody>
</table>

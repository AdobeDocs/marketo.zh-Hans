---
description: 电子邮件创作 — Marketo文档 — 产品文档
title: 电子邮件创作
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 1f899044d0eb872d4b91fa341cb8b28e1556a045
workflow-type: tm+mt
source-wordcount: '1477'
ht-degree: 1%

---

# 电子邮件创作 {#email-authoring}

了解如何在新的Marketo Engage电子邮件Designer中创建、个性化和预览电子邮件。

>[!IMPORTANT]
>
>本文仅适用新Marketo Engage电子邮件编辑器测试版的成员。 请不要传播。

## 创建电子邮件 {#create-an-email}

1. 通过[Adobe Experience Cloud](https://experiencecloud.adobe.com/){target="_blank"}登录Marketo Engage。

1. 在“我的Marketo”中，选择&#x200B;**设计工作室**。

   ![](assets/create-an-email-1.png)

1. 在树中选择&#x200B;**电子邮件（新编辑器）**。

   ![](assets/create-an-email-2.png)

1. 单击&#x200B;**创建电子邮件**&#x200B;按钮。

   ![](assets/create-an-email-3.png)

1. 输入电子邮件名称和主题行。 单击&#x200B;**创建**。

   ![](assets/create-an-email-4.png)

就是这样。 现在该设计您的电子邮件了。

## 选择您的内容类型 {#choose-your-content-type}

1. 在刚刚创建的电子邮件中，单击&#x200B;**添加电子邮件内容**。

   ![](assets/choose-your-content-type-1.png)

1. 加载&#x200B;_创建电子邮件_&#x200B;页面。 您可以从以下几个选项中进行选择：

* [使用可视电子邮件编辑器从头开始设计](#design-from-scratch)

* [通过HTML或zip文件导入您自己的HTML](#import-html)

* [选择现有模板](#choose-a-template)（我们的一个示例或您已保存的示例）

### 从头开始设计 {#design-from-scratch}

在电子邮件编辑器中从头开始时，请使用以下选项来定义您的内容。

1. 在&#x200B;_创建电子邮件_&#x200B;页面中，选择&#x200B;**从头开始设计**。

1. 将[结构和内容](#add-structure-and-content)添加到您的电子邮件中。

1. 添加[图像](#add-assets)。

1. [个性化](#personalize-content)您的内容。

1. 查看链接并[编辑跟踪](#edit-url-tracking)。

### 导入HTML {#import-html}

您可以导入现有HTML内容来设计电子邮件。 内容可以是：

* 具有合并样式表的HTML文件

* 包含HTML文件、样式表(.css)和图像的.zip文件

>[!NOTE]
>
>.zip文件结构没有限制。 但是，引用必须是相对的，并且适合.zip文件夹的树结构。

1. 在“设计模板”页中，选择&#x200B;**导入HTML**。

1. 拖放所需的HTML或.zip文件（或从您的计算机中选择一个文件），然后单击&#x200B;**导入**。

   ![](assets/authoring-import-your-html-1.png)

>[!NOTE]
>
>上传HTML内容后，您的内容将处于兼容模式。 在此模式下，您只能个性化文本、添加链接或向内容添加资产。

您可以使用[可视电子邮件编辑器工具](#add-structure-and-content)对导入的内容进行所需的更改。

### 选择模板 {#choose-a-template}

有两种类型的模板可供选择。

* **示例模板**：Marketo Engage提供了四个现成的电子邮件模板。

* **保存的模板**：这些模板是您使用“模板”菜单从头创建的模板，或者您创建并选择另存为模板的电子邮件。

>[!BEGINTABS]

>[!TAB 示例模板]

选择其中一个现成的模板，以抢先一步进行电子邮件模板设计。

1. 默认情况下，“示例模板”选项卡处于打开状态。

1. 选择要使用的模板。

   ![](assets/authoring-sample-templates-1.png)

1. 单击&#x200B;**使用此模板**。

   ![](assets/authoring-sample-templates-2.png)

1. 使用可视内容设计器根据需要编辑内容。

>[!TAB 已保存模板]

1. 单击&#x200B;**保存的模板**&#x200B;选项卡，然后选择所需的模板。

   ![](assets/authoring-saved-templates-1.png)

1. 单击&#x200B;**使用此模板**。

   ![](assets/authoring-saved-templates-2.png)

1. 使用可视内容设计器根据需要编辑内容。

>[!ENDTABS]

## 添加结构和内容 {#add-structure-and-content}

1. 要开始创建或修改内容，请将项目从“结构”拖放到画布上。 在右侧的窗格中编辑其设置。

   >[!TIP]
   >
   >选择n：n列组件以定义所选列数（3到10之间）。 您还可以通过移动列下方的箭头来定义每列的宽度。

   ![](assets/authoring-add-structure-and-content-1.png)

   >[!NOTE]
   >
   >每个列大小不能小于结构组件总宽度的10%。 只能删除空列。

1. 从内容部分中，将所需项目拖放到一个或多个结构组件中。

   ![](assets/authoring-add-structure-and-content-2.png)

1. 可通过“设置”或“样式”选项卡自定义每个组件。 更改字体、文本样式、边距等。

### 添加Assets {#add-assets}

```
ADD ASSETS OR ADD IMAGES? WHAT OTHER ASSETS CAN YOU ADD?
```

```
Access assets stored in the Assets library. IMAGES AND FILES ONLY? - For now, only from Marketo Images and Files section!!!
```

1. 要访问您的图像，请单击资产选择器图标。

   屏幕快照

1. 将所需的图像拖放到结构组件中。

   屏幕快照

   >[!NOTE]
   >
   >要替换现有图像，请选择该图像，然后在右侧的“设置”选项卡中单击&#x200B;**选择资产**。

单击启用条件内容以添加动态内容，并根据条件规则将内容调整到目标用户档案。



如果需要，您可以通过单击高级菜单中的“切换到代码编辑器”，进一步个性化电子邮件。 这允许您编辑电子邮件源代码，例如添加跟踪或自定义HTML标签。

注意
切换到代码编辑器后，无法还原到此电子邮件的可视设计器。

内容准备就绪后，单击模拟内容按钮以检查渲染。 您可以选择桌面视图或移动设备视图。

准备就绪后，单击保存

### 图层、设置和样式 {#layers-settings-styles}

```
ARE THEY CALLED LAYERS OR COMPONENTS - NILESH WILL CHECK
```

打开导航树以访问特定结构及其列/组件以进行更细粒度的编辑。 要访问，请单击导航树图标。

![](assets/authoring-layers-settings-styles-1.png)

下面的示例概述了在由列组成的结构组件内调整填充和垂直对齐的步骤。

1. 直接在画布中选择结构组件中的列，或使用左侧显示的&#x200B;_导航树_。

1. 在列工具栏中，单击&#x200B;_[!UICONTROL 选择列]_&#x200B;工具，然后选择要编辑的工具。

   也可以从结构树中选择它。 该列的可编辑参数显示在右侧的&#x200B;_[!UICONTROL 设置]_&#x200B;和&#x200B;_[!UICONTROL 样式]_&#x200B;选项卡中。

   ![](assets/authoring-layers-settings-styles-2.png)

1. 要编辑列属性，请单击右侧的&#x200B;_[!UICONTROL 样式]_&#x200B;选项卡，然后根据需要进行更改：

   * 对于&#x200B;**[!UICONTROL 背景]**，根据需要更改背景颜色。

     清除透明背景的复选框。 启用&#x200B;**[!UICONTROL 背景图像]**&#x200B;设置以使用图像作为背景，而不是纯色。

   * 对于&#x200B;**[!UICONTROL 对齐方式]**，请选择&#x200B;_Top_、_Middle_&#x200B;或&#x200B;_Bottom_&#x200B;图标。
   * 对于&#x200B;**[!UICONTROL 内边距]**，定义所有边的内边距。

     如果要调整边距，请选择&#x200B;**[!UICONTROL 每边不同的边距]**。 单击&#x200B;_锁定_&#x200B;图标中断同步。

   * 展开&#x200B;**[!UICONTROL 高级]**&#x200B;部分以定义列的内联样式。

   ![](assets/authoring-layers-settings-styles-3.png)

1. 根据需要重复这些步骤以调整组件中其他列的对齐和填充。

1. 保存更改。

### 使内容个性化 {#personalize-content}

令牌在新编辑器中的工作方式与在旧编辑器中的工作方式相同，但图标的外观不同。 以下示例概述了如何使用回退文本添加名字令牌。

1. 选择文本组件。 将光标放在您希望令牌出现的位置，然后单击&#x200B;**添加个性化**&#x200B;图标。

   ![](assets/authoring-personalize-content-1.png)

1. 单击所需的[令牌类型](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}。

   ![](assets/authoring-personalize-content-2.png)

1. 找到所需的令牌，然后单击&#x200B;**...**&#x200B;图标（改为单击+图标可添加不含回退文本的令牌）。

   ![](assets/authoring-personalize-content-3.png)

   >[!NOTE]
   >
   >“回退文本”是适用于默认值的新编辑器术语。 示例： ``{{lead.First Name:default=Friend}}``。 如果所选字段中没有人员的值，则建议使用此字段。

1. 设置您的回退文本，然后单击&#x200B;**添加**。

   ![](assets/authoring-personalize-content-4.png)

1. 单击&#x200B;**保存**。

### 编辑URL跟踪 {#edit-url-tracking}

有时，您不希望通过电子邮件在链接上启用Marketo跟踪URL。 当目标页面不支持URL参数并且可能导致链接断开时，这将很有用。

1. 单击链接图标以显示电子邮件中的所有URL。

   ![](assets/authoring-edit-url-tracking-1.png)

1. 单击铅笔图标可编辑任何所需链接的跟踪。

1. 单击&#x200B;**跟踪类型**&#x200B;下拉列表并进行选择。

   ![](assets/authoring-edit-url-tracking-2.png)

   ```
   LABEL? - just what URL shows as (ex: my site)
   
   TAGS? - NILESH WILL CHECK ON HOW THEY WORK
   ```

   <table><tbody>
     <tr>
       <td><b>不使用mkt_tok跟踪</b></td>
       <td>定义</td>
     </tr>
     <tr>
       <td><b>使用mkt_tok跟踪</b></td>
       <td>定义</td>
     </tr>
     <tr>
       <td><b>不跟踪</b></td>
       <td>定义</td>
     </tr>
   </tbody>
   </table>

1. 完成后单击&#x200B;**保存**。

## 检查警报 {#check-alerts}

设计内容时，如果缺少关键设置，屏幕右上角会显示警报。

警报有两种类型：

**个警告**

警告指代建议和最佳实践，例如：

* **电子邮件正文中不存在选择退出链接**：虽然取消订阅链接是必需的，但最佳做法是将它们添加到电子邮件正文中。

>[!NOTE]
>
>[操作电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)（非营销）不需要添加取消订阅选项。

* **HTML的文本版本为空**：您必须为无法显示HTML内容时定义电子邮件正文的文本版本。

* **电子邮件正文中存在空链接**：验证电子邮件中的所有链接是否正确。

* **电子邮件大小已超出100KB的限制**：若要获得最佳投放，请确保电子邮件大小不超过100KB。

**个错误**

在解决错误之前，您无法发送或测试电子邮件：

* **主题行缺失**：需要电子邮件主题行。

* **邮件的电子邮件版本为空**：当尚未配置电子邮件内容时，会发生此错误。

## 测试电子邮件 {#test-your-email}

定义消息内容后，您可以使用测试用户档案对其进行预览、发送校样并控制它在常用桌面、移动和基于Web的客户端中的呈现方式。 如果插入个性化内容，则可以使用测试用户档案数据检查该内容在消息中的显示方式。

要预览电子邮件内容，请单击&#x200B;**模拟内容**，然后添加测试用户档案，以使用测试用户档案数据检查邮件。

![](assets/test-your-email-1.png)

## 引用电子邮件 {#reference-an-email}

在新编辑器中创建电子邮件后，您可以在智能营销活动和/或智能列表中引用该电子邮件，就像您在处理任何其他电子邮件时所做的那样。

* 按照常规步骤](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)，[在智能列表中引用它。

* 按照常规步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)，[在Smart Campaign中引用它。

>[!NOTE]
>
>只能引用保存的电子邮件。 新电子邮件编辑器中没有“已批准”状态。

>[!MORELIKETHIS]
>
>[电子邮件模板](/help/marketo/product-docs/email-marketing/general/beta-new-email-editor/email-templates.md){target="_blank"}：了解如何在新的编辑器中创建、设计和访问电子邮件模板。

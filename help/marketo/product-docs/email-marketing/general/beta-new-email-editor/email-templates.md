---
description: 电子邮件模板 — Marketo文档 — 产品文档
title: 电子邮件模板
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 832635c9e029754ce094e4137724bcc956dbcd35
workflow-type: tm+mt
source-wordcount: '1672'
ht-degree: 1%

---

# 电子邮件模板 {#email-templates}

为了加快并改进设计过程，您可以创建独立的电子邮件模板以轻松重用自定义内容。

>[!IMPORTANT]
>
>本文仅适用新Marketo Engage电子邮件编辑器测试版的成员。 请不要传播。

>[!NOTE]
>
>新电子邮件编辑器中的电子邮件模板只能用于在新电子邮件编辑器中创建电子邮件。 在旧电子邮件编辑器中无法引用它们。

## 创建电子邮件模板 {#create-an-email-template}

1. 通过[Adobe Experience Cloud](https://experiencecloud.adobe.com/){target="_blank"}登录Marketo Engage。

1. 在“我的Marketo”中，选择&#x200B;**设计工作室**。

   ![](assets/create-an-email-template-1.png)

1. 在树中选择&#x200B;**电子邮件模板（新编辑器）**。

   ![](assets/create-an-email-template-2.png)

1. 单击&#x200B;**创建模板**&#x200B;按钮。

   ![](assets/create-an-email-template-3.png)

1. 输入模板名称和可选说明。 单击&#x200B;**创建**。

   ![](assets/create-an-email-template-4.png)

## 设计模板 {#design-your-template}

在&#x200B;_设计模板_&#x200B;页面中，可以从几个选项中进行选择。 [从头开始设计](#design-from-scratch)、[导入您自己的HTML](#import-html)或[选择现有模板](#choose-a-template)（我们的示例之一或您已保存的示例）。

![](assets/design-your-template-1.png)

### 从头开始设计 {#design-from-scratch}

通过简单的拖放操作添加和移动结构元素来定义内容。

1. 在&#x200B;_设计模板_&#x200B;页面中，选择&#x200B;**从头开始设计**。

1. 添加[结构和内容](#add-structure-and-content)。

### 导入您的HTML {#import-your-html}

您可以导入现有HTML内容来设计电子邮件模板。 内容可以是：

* 具有合并样式表的HTML文件

* 包含HTML文件、样式表(.css)和图像的.zip文件

>[!NOTE]
>
>.zip文件结构没有限制。 但是，引用必须是相对的，并且适合.zip文件夹的树结构。

1. 在&#x200B;_设计模板_&#x200B;页中，选择&#x200B;**导入HTML**。

1. 拖放所需的HTML或.zip文件（或从您的计算机中选择一个文件），然后单击&#x200B;**导入**。

   ![](assets/import-your-html-1.png)

   >[!NOTE]
   >
   >上传HTML内容后，您的内容将处于兼容模式。 在此模式下，您只能个性化文本、添加链接或向内容添加资产。

1. 若要利用Email Designer内容组件，请单击&#x200B;**HTML转换器**&#x200B;选项卡，然后单击&#x200B;**转换**。

   屏幕快照

   >[!CAUTION]
   >
   >在HTML文件中使用`<table>`标记作为第一层可能会导致样式丢失，包括顶层标记中的背景和宽度设置。

现在，您可以根据需要使用可视电子邮件编辑器对导入的文件进行个性化设置。

### 选择模板 {#choose-a-template}

有两种类型的模板可供选择。

* 示例模板：Marketo Engage提供了四个现成的电子邮件模板。

* 保存的模板：这些是使用“模板”菜单从头创建的模板，或者您创建并选择另存为模板的电子邮件。

>[!BEGINTABS]

>[!TAB 示例模板]

选择其中一个现成的模板，以抢先一步进行电子邮件模板设计。

1. 默认情况下，“示例模板”选项卡处于打开状态。

1. 选择要使用的模板。

   ![](assets/sample-templates-1.png)

1. 单击&#x200B;**使用此模板**。

   ![](assets/sample-templates-2.png)

1. 使用可视内容设计器根据需要编辑内容。

>[!TAB 已保存模板]

1. 单击&#x200B;**保存的模板**&#x200B;选项卡，然后选择所需的模板。

   ![](assets/saved-templates-1.png)

1. 单击&#x200B;**使用此模板**。

   ![](assets/saved-templates-2.png)

1. 使用可视内容设计器根据需要编辑内容。

>[!ENDTABS]

## 添加结构和内容 {#add-structure-and-content}

1. 要开始创建或修改内容，请将项目从“结构”拖放到画布上。 在右侧的窗格中编辑其设置。

   >[!TIP]
   >
   >选择n：n列组件以定义所选列数（3到10之间）。 您还可以通过移动列下方的箭头来定义每列的宽度。

   ![](assets/add-structure-and-content-1.png)

   >[!NOTE]
   >
   >每个列大小不能小于结构组件总宽度的10%。 只能删除空列。

1. 从内容部分中，将所需项目拖放到一个或多个结构组件中。

   ![](assets/add-structure-and-content-2.png)

1. 可通过“设置”或“样式”选项卡自定义每个组件。 更改字体、文本样式、边距等。

屏幕快照

### 添加Assets {#add-assets}

```
ADD ASSETS OR ADD IMAGES? WHAT OTHER ASSETS CAN YOU ADD??
```

```
Access assets stored in the Assets library. IMAGES AND FILES ONLY?
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
ARE THEY CALLED LAYERS OR COMPONENTS
```

打开导航树以访问特定结构及其列/组件以进行更细粒度的编辑。 要访问，请单击导航树图标。

![](assets/layers-settings-styles-1.png)

下面的示例概述了在由列组成的结构组件内调整填充和垂直对齐的步骤。

1. 直接在画布中选择结构组件中的列，或使用左侧显示的&#x200B;_导航树_。

1. 在列工具栏中，单击&#x200B;_[!UICONTROL 选择列]_&#x200B;工具，然后选择要编辑的工具。

   也可以从结构树中选择它。 该列的可编辑参数显示在右侧的&#x200B;_[!UICONTROL 设置]_&#x200B;和&#x200B;_[!UICONTROL 样式]_&#x200B;选项卡中。

   ![](assets/layers-settings-styles-2.png)

1. 要编辑列属性，请单击右侧的&#x200B;_[!UICONTROL 样式]_&#x200B;选项卡，然后根据需要进行更改：

   * 对于&#x200B;**[!UICONTROL 背景]**，根据需要更改背景颜色。

     清除透明背景的复选框。 启用&#x200B;**[!UICONTROL 背景图像]**&#x200B;设置以使用图像作为背景，而不是纯色。

   * 对于&#x200B;**[!UICONTROL 对齐方式]**，请选择&#x200B;_Top_、_Middle_&#x200B;或&#x200B;_Bottom_&#x200B;图标。
   * 对于&#x200B;**[!UICONTROL 内边距]**，定义所有边的内边距。

     如果要调整边距，请选择&#x200B;**[!UICONTROL 每边不同的边距]**。 单击&#x200B;_锁定_&#x200B;图标中断同步。

   * 展开&#x200B;**[!UICONTROL 高级]**&#x200B;部分以定义列的内联样式。

   ![](assets/layers-settings-styles-3.png)

1. 根据需要重复这些步骤以调整组件中其他列的对齐和填充。

1. 保存更改。

### 使内容个性化 {#personalize-content}

令牌在新编辑器中的工作方式与在旧编辑器中的工作方式相同，但图标的外观不同。

1. 选择文本组件并单击&#x200B;**添加个性化**&#x200B;图标。

   屏幕快照

1. 单击所需的[令牌类型](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}。

   屏幕快照

1. 单击+或……向空格添加令牌。

   屏幕快照

   >[!NOTE]
   >
   >“回退文本”是适用于默认值的新编辑器术语。 示例：``{{lead.First Name:default=Friend}}``

1. 完成后单击&#x200B;**保存**。

### 编辑URL跟踪 {#edit-url-tracking}

有时，您不希望通过电子邮件在链接上启用Marketo跟踪URL。 当目标页面不支持URL参数并且可能导致链接断开时，这将很有用。

1. 单击链接图标以显示电子邮件中的所有URL。

   屏幕快照

1. 单击铅笔图标可编辑任何所需链接的跟踪。

   屏幕快照

   ```
   LABEL?
   
   TAGS?
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

### 查看选项 {#view-options}

利用可视电子邮件编辑器中提供的视图和内容验证选项。

* 使用预设的缩放选项放大/缩小内容。

* 在桌面、移动设备或纯文本/纯文本中查看内容。

   * 单击实时视图（眼睛）图标可跨设备预览内容。

   * 选择其中一个现成的设备或输入自定义维度以预览您的内容。

### 更多选项 {#more-options}

在内容编辑器的&#x200B;**更多**&#x200B;选项中，您可以执行以下操作：

屏幕快照

* **重置模板**：选择此项可将可视电子邮件设计器画布清除为空白并重新启动内容生成。

* **更改您的设计**：返回到&#x200B;_设计您的模板_&#x200B;页面。 从此处，您可以按照[设计模板](#design-your-template)部分中概述的步骤执行任何操作。

* **导出HTML**：将可视画布中的内容以HTML格式下载到本地系统，并打包为zip文件。

## 查看模板详细信息 {#view-template-details}

在&#x200B;_电子邮件模板_&#x200B;列表页中，单击电子邮件模板名称以查看其详细信息。

屏幕快照

可以编辑名称和描述等基本详细信息。 在编辑的字段外单击，以保存更改。

单击&#x200B;**更多**&#x200B;可快速删除或复制您的模板。

如果有任何活动警报（电子邮件模板的错误/警告），请单击警报以查看相关信息。

>[!NOTE]
>
>虽然这些警报不禁止使用电子邮件模板创建电子邮件，但信息可提供在电子邮件可用于投放之前可能不起作用的内容和所需更新的可见性。

## 查看引用使用的电子邮件模板 {#email-template-used-by-references}

在电子邮件模板摘要中，单击&#x200B;**使用者**&#x200B;选项卡查看在Marketo Engage中使用此电子邮件模板位置的详细信息。

屏幕快照

## 编辑电子邮件模板 {#edit-email-templates}

此操作可从以下位置执行：

* 详细信息选项卡 — 单击&#x200B;**编辑电子邮件模板**。

* _电子邮件模板_&#x200B;列表页面 — 单击所需电子邮件模板的“更多操作”图标（三个圆点），然后选择“编辑”。

```
THE SECOND ONE DOESN'T WORK IN MARKETO?? JUST LISTS DUPE AND DELETE
```

此操作会将您引导至&#x200B;_根据电子邮件模板的上次保存状态设计您的模板_&#x200B;页面或可视内容编辑器页面。 在此处，您可以根据需要编辑电子邮件模板内容。 有关编辑选项的信息，请参阅创建电子邮件模板。

## 重复的电子邮件模板 {#duplicate-email-templates}

复制电子邮件模板的方法有两种：

* 从右侧的电子邮件模板详细信息中，单击&#x200B;**更多**&#x200B;并选择&#x200B;**复制**。

屏幕快照

* 在&#x200B;_电子邮件模板_&#x200B;列表页面中，单击所需电子邮件模板的“更多操作”图标（三个圆点），然后选择&#x200B;**复制**。

在对话框中，输入唯一名称和可选描述。 完成后单击&#x200B;**复制**。

然后，复制的电子邮件模板出现在&#x200B;_电子邮件模板_&#x200B;列表页中。

## 删除电子邮件模板 {#delete-email-templates}

可通过两种方式删除电子邮件模板。

>[!CAUTION]
>
>无法撤消删除电子邮件模板的操作。

* 从右侧的电子邮件模板详细信息中，单击&#x200B;**更多**&#x200B;并选择&#x200B;**删除**。

屏幕快照

* 在&#x200B;_电子邮件模板_&#x200B;列表页面中，单击所需电子邮件模板的“更多操作”图标（三个圆点），然后选择&#x200B;**删除**。

## 批量操作 {#bulk-actions}

从&#x200B;_电子邮件模板_&#x200B;列表页面中，选中左侧的复选框以选择多个模板。 底部会显示一条横幅。

**删除**：一次最多可以删除20个模板。 确认对话框允许您中止操作或确认删除。

>[!MORELIKETHIS]
>
>[电子邮件创作](/help/marketo/product-docs/email-marketing/general/beta-new-email-editor/email-authoring.md){target="_blank"}：了解如何在新的编辑器中创建、设计和引用电子邮件。

---
description: GenAI功能 — Marketo文档 — 产品文档
title: GenAI功能
feature: Interactive Webinars
exl-id: 3e0a41b0-7ff3-4676-bafc-4e7a0725a737
source-git-commit: 6350137c2abfb46a0a8451772a8dc08391f3e4b5
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# GenAI功能 {#gen-ai-features}

为您的录制的网络研讨会自动生成章节和摘要，使受众更容易访问和导航这些章节和摘要。

* **自动生成章节**： AI支持的技术为您的网络研讨会内容创建章节。

* **AI生成的摘要**：获取网络研讨会的自动文本摘要。

* **基于人工智能的博客生成**：允许您从网络研讨会自动生成品牌博客内容。

* **可编辑内容**：如果需要，可使用手动和AI支持的编辑功能修改生成的章节和摘要。

* **轻松集成**：通过将HTML代码复制到您选择的网页编辑器，轻松地将章节和摘要添加到您的登陆页面。

## 启用GenAI {#enable-genai}

>[!PREREQUISITES]
>
>在使用这些功能之前，必须首先接受Adobe GenAI条款和条件。 如果您尚未这样做，请联系Adobe客户团队（您的客户经理）以了解详细信息。

在您接受Adobe GenAI条款和条件后，下一步是为个人用户启用它。 为此，请转到&#x200B;**[!UICONTROL Admin]** > **[!UICONTROL Interactive Webinars]**，并选择哪些用户应有权访问GenAI。

![](assets/gen-ai-features-1.png){width="800" zoomable="yes"}

## 如何访问 {#how-to-access}

1. 导航到Marketo Engage交互式网络研讨会中的“概述”页面。

1. 进行按需网络研讨会后，等待30到60分钟，让AI处理您的录制。 当“生成”按钮可用时，该按钮将变为可单击状态。

1. 单击 **[!UICONTROL View GenAI Content]**。

   ![](assets/gen-ai-features-2.png){width="800" zoomable="yes"}

1. 此时将打开一个新选项卡，其中显示AI生成的章节和文本摘要。

## 编辑生成的内容 {#edit-generated-content}

1. 查看生成的章节和摘要。

1. 如果需要更改，请单击&#x200B;**[!UICONTROL Edit]**&#x200B;按钮。

   进行修改：

   * 编辑摘要和/或章节标题中的文本。

   * 如有必要，可通过编辑时间戳字段中的值来调整时间戳。

   * 通过选择不需要的章节并单击&#x200B;**[!UICONTROL Delete]**&#x200B;来删除它们。

   * 通过选择两个连续章节并单击&#x200B;**[!UICONTROL Merge]**&#x200B;将其合并。

      * AI会生成一个包含两个选定章节的复合章节

      * 要合并多个章节，必须一次合并两个

     ![](assets/gen-ai-features-3.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >* 如果需要，您可以使用&#x200B;_竖起缩略图_ ![竖起缩略图图标](assets/icon-thumbs-up.png)或&#x200B;_竖下缩略图_ ![竖下缩略图图标](assets/icon-thumbs-down.png)图标来评价生成的章节/摘要的质量。 您还可以通过单击标记图标![标记图标](assets/icon-flag.png)来标记任何有问题的内容。
   >
   >* 如果您对初始摘要不满意，可以单击&#x200B;**[!UICONTROL Regenerate summary]**&#x200B;按钮，并生成另一个版本。

1. 单击屏幕右上方的&#x200B;**[!UICONTROL Save]**&#x200B;按钮保存更改。

## 使用生成的内容 {#use-generated-content}

复制要使用的内容后，将其粘贴到所选编辑器(例如，Marketo Engage登陆页面编辑器)中进行任何所需的调整。

### 摘要 {#summary}

**复制HTML** — 单击“**[!UICONTROL Copy HTML]**”按钮获取所有文本，并在表中使用HTML代码设置文本格式。

**仅限文本** — 如果只想复制文本，只需突出显示它并选择Ctrl/Cmd+C（或右键单击）进行复制。

### 章节 {#chapters}

**复制HTML** — 单击“**[!UICONTROL Copy HTML]**”按钮，在视频播放器中格式化所有录制及其章节。

## 定位受众

利用Smart Campaign/List过滤器和/或触发器查看每个查看者观看了哪些内容，观看了多少次等，从而实现个性化的跟进。

![](assets/gen-ai-features-4.png){width="800" zoomable="yes"}

* **触发器**： _点击网页上的链接_，_访问网页_

* **筛选器**：_已点击网页上的链接_，_已访问网页_

“链接”是章节的名称，“网页”是承办On Demand网络研讨会的页面。

>[!TIP]
>
>使用[约束](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"}进一步优化目标受众。

## 注意事项 {#things-to-note}

* 删除或合并章节仅影响章节栈栈，不影响视频内容本身。 这些操作是永久性的。

* GenAI功能非常灵活，可与各种网页编辑器一起使用，而不仅仅是Marketo Engage中的编辑器。

* 只有研讨厅的会议才可供产生博客。 只有拥有“活动模块”或“研讨会（共享房间/活动）”许可证的客户才能使用研讨会房间。

* 始终预览您的更改以确保所需的功能和外观。

* 删除网络研讨会也会删除GenAI内容。

* 如果您想在不删除网络研讨会的情况下删除GenAI内容，请联系Adobe客户团队（您的客户经理），或发送数据删除请求到：`marketo-webinar-genai-alerts@adobe.com`。

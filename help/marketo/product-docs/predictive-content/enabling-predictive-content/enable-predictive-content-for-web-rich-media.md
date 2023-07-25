---
unique-page-id: 7514956
description: 为Web富媒体启用预测内容 — Marketo文档 — 产品文档
title: 为Web富媒体启用预测内容
exl-id: 030f1dd7-8fe7-4c82-be5e-052f0a259e3c
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# 为Web富媒体启用预测内容 {#enable-predictive-content-for-web-rich-media}

预测内容通过机器学习和预测分析为您的Web访客提供最相关的内容。 借助Web富媒体，您可以使用文本描述和图像来增强内容，并在网站上嵌入多个预测性内容推荐。

>[!NOTE]
>
>建议您在测试和使用预测内容之前，为每个类别和每个源（电子邮件、富媒体、条形图）启用超过5个内容。 更多内容为您提供更好的预测结果。

>[!PREREQUISITES]
>
>在启用预测内容之前，您必须：
>
>* **准备预测内容**
>
>   * [编辑电子邮件的预测内容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"} 或
>   * [编辑富媒体的预测内容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"} 或
>   * [编辑推荐栏的预测内容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [批准预测内容的标题](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

准备好富媒体的内容标题、描述和图像后，您可以启用单个或多个内容片段。

1. 要启用单个标题，请单击标题以打开编辑器。 单击富媒体，然后检查 **启用富媒体中的预测内容** 框并单击 **保存**.

   ![](assets/image2017-10-3-9-3a50-3a29.png)

1. 对于多段内容，在 **预测内容** 页面，选中标题旁边的复选框。

   ![](assets/image2017-10-3-10-3a0-3a42.png)

1. 单击 **内容操作** 下拉菜单并选择 **为Web富媒体启用**.

   ![](assets/image2017-10-3-10-3a2-3a6.png)|

## 自定义Javascript代码并将其嵌入您的网站  {#customize-the-javascript-code-and-embed-it-into-your-website}

请参阅有关富媒体推荐模板的文档 [在Marketo开发人员网站上](https://developers.marketo.com/documentation/websites/rtp-rich-media-recommendations-api){target="_blank"}. 以下说明如何自定义网站的模板。

将JavaScript代码粘贴到网站中您希望显示模板的位置。

**模板示例**

* 模板1：三个水平内容片段，带有图像、标题和描述
* 模板2：三个垂直内容片段，带有图像、标题和描述

以下是富媒体推荐模板1的示例：

![](assets/image2015-6-1-17-3a8-3a33.png)

以下是富媒体推荐模板2的示例：

![](assets/image2015-12-20-10-3a35-3a12.png)

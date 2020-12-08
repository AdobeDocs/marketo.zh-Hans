---
unique-page-id: 4720108
description: 启用内容推荐栏- Marketo Docs —— 产品文档
title: 启用内容推荐栏
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---


# 启用内容推荐栏 {#enable-the-content-recommendation-bar}

内容推荐引擎使用预测分析和机器学习算法向每个Web访客提供相关内容。 推荐引擎可预测哪些内容在每个访客下效果最佳。 引擎的内容在Recommendations页面下进行监控，帮助您优化内容ROI。

>[!NOTE]
>
>**先决条件**
>
>在启用预测性内容之前，您必须：
>
>* [准备您的预测性内容](http://docs.marketo.com/display/docs/edit+predictive+content)
>* [批准预测内容的标题](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## 启用和自定义内容推荐栏 {#enable-and-customize-the-content-recommendation-bar}

1. 转到“ **内容设置**”。

   ![](assets/settings-dropdown-hand.png)

1. 单击 **“栏**”。

   ![](assets/content-settings-bar-hand.png)

1. 要为URL启用推荐栏，只需单击“开 **启** ”，然 **后保存**。

   ![](assets/bar-enable.png)

1. 要自定义URL，请为推荐栏选择颜色、样式、格式、箭头以及要包括或排除该栏的页面。 自定义以适合您的网站品牌。 单击 **保存**。

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**包含／排除显示URL**
   >
   >    * 显示URL应为域的路径
   >    * 不包括http://或https://
   >    * 使用*表示通配符
   * 使用分号作为分隔符
   * 示例：/contact_us*;*action=logout*
   * 此字段区分大小写


## 推荐栏注意事项 {#recommendation-bar-considerations}

* 您至少需要一个内容片段，使推荐栏在Recommendations **页面** 上设置为“开启”，以便推荐引擎能够工作。 如果未启用任何内容，且“栏”设 **置为**“打开”，则箭头效果将显示在网页的右下方，但不会显示建议的内容。

* 推荐引擎中运行的内容越多，算法就越能测试和了解哪些内容最适合。 我们建议从10到20个内容片段开始运行并保持活动状态，并不断添加新内容。
* 您为推荐启用的内容片段应包括RTP Javascript标签。 这有助于算法跟踪和优化推荐内容。

>[!NOTE]
**相关文章**
* [为Web富媒体启用预测内容](enable-predictive-content-for-web-rich-media.md)


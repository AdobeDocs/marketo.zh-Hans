---
unique-page-id: 4720108
description: 启用内容推荐栏 — Marketo Docs — 产品文档
title: 启用内容推荐栏
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---


# 启用内容推荐栏{#enable-the-content-recommendation-bar}

内容推荐引擎使用预测分析和机器学习算法向每个Web访客提供相关内容。 推荐引擎预测哪些内容在每个访客中表现最佳。 引擎的内容在Recommendations页面下进行监控，帮助您优化内容ROI。

>[!PREREQUISITES]
>
>在启用预测内容之前，您必须：
>
>* [准备预测内容](https://docs.marketo.com/display/docs/edit+predictive+content)
>* [批准预测内容的标题](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## 启用和自定义内容推荐栏{#enable-and-customize-the-content-recommendation-bar}

1. 转到&#x200B;**内容设置**。

   ![](assets/settings-dropdown-hand.png)

1. 单击&#x200B;**Bar**。

   ![](assets/content-settings-bar-hand.png)

1. 要为URL启用推荐栏，只需单击&#x200B;**On**，然后单击&#x200B;**Save**。

   ![](assets/bar-enable.png)

1. 要自定义URL，请为推荐栏选择颜色、样式、格式、箭头以及要包括或排除该栏的页面。 自定义以适合您的网站品牌。 单击&#x200B;**保存**。

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**包含/排除显示URL**
   >
   >    * 显示URL应为域的路径
   >    * 不要包含https://或https://
   >    * 使用*表示通配符
   * 使用分号作为分隔符
   * 示例：/contact_us*;*action=logout*
   * 此字段区分大小写


## 建议栏注意事项{#recommendation-bar-considerations}

* 您至少需要一个内容片段，以使推荐引擎在Recommendations页面上设置为&#x200B;**On**&#x200B;的推荐栏能够正常工作。 如果未启用任何内容，且“栏”设置为&#x200B;**On**，则“箭头”效果将显示在网页右下方，但不显示推荐的内容。

* 推荐引擎中运行的内容越多，算法就越能测试和了解哪些内容最适合。 我们建议从10到20个内容片段开始运行并处于活动状态，并不断添加新内容片段。
* 您为推荐启用的内容片段应包含RTP Javascript标签。 这有助于算法跟踪和优化推荐内容。

>[!MORELIKETHIS]
* [为Web富媒体启用预测内容](enable-predictive-content-for-web-rich-media.md)


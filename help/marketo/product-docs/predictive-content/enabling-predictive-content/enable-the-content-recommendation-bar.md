---
unique-page-id: 4720108
description: 启用内容推荐栏 — Marketo文档 — 产品文档
title: 启用内容推荐栏
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# 启用内容推荐栏 {#enable-the-content-recommendation-bar}

内容推荐引擎使用预测分析和机器学习算法向每个Web访客提供相关内容。 推荐引擎可预测每个访客表现最佳的内容。 引擎的内容在Recommendations页面下进行监控和控制，从而帮助您优化内容ROI。

>[!PREREQUISITES]
>
>在启用预测内容之前，您必须：
>
>* **准备预测内容**
   >
   >   * [编辑电子邮件的预测内容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) 或
   >   * [编辑富媒体的预测内容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) 或
   >   * [编辑推荐栏的预测内容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [批准预测内容的标题](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## 启用和自定义内容推荐栏 {#enable-and-customize-the-content-recommendation-bar}

1. 转到 **内容设置**.

   ![](assets/settings-dropdown-hand.png)

1. 单击 **条形图**.

   ![](assets/content-settings-bar-hand.png)

1. 要为URL启用推荐栏，只需单击 **开** 然后 **保存**.

   ![](assets/bar-enable.png)

1. 要自定义URL，请为推荐栏选择颜色、样式、格式、箭头以及要包含或排除该栏的页面。 自定义以适合您的网站品牌。 单击 **保存**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**包含/排除显示URL**
   >
   >* 显示URL应为域的路径
   >* 请勿包含https://或https://
   >* 使用 &#42; 用于通配符
   >* 使用分号作为分隔符
   >* 示例：/contact_us&#42;; &#42;action=logout&#42;
   >* 此字段区分大小写


## 推荐栏注意事项 {#recommendation-bar-considerations}

* 推荐栏设置为 **开** 在Recommendations页面上，以便推荐引擎正常工作。 如果未启用任何内容，且“栏”设置为 **开**，则“箭头”效果将显示在网页右下方，但不会显示推荐的内容。

* 推荐引擎中运行的内容越多，算法测试和了解哪些内容效果最好。 我们建议从运行和激活的10到20个内容片段开始，并继续添加新内容片段。
* 您为推荐启用的内容片段应包含RTP Javascript标记。 这有助于算法跟踪和优化推荐内容。

>[!MORELIKETHIS]
>
>[为Web富媒体启用预测内容](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)

---
unique-page-id: 4720125
description: 将RTP与Google Universal Analytics集成 — Marketo文档 — 产品文档
title: 将RTP与Google Universal Analytics集成
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# 将RTP与Google Universal Analytics集成 {#integrate-rtp-with-google-universal-analytics}

## 简介 {#intro}

利用Google Universal Analytics (GUA)与Marketo Real-Time Personalization (RTP)的第一和个性化数据，更好地衡量和分析您的在线营销工作。

本文说明如何设置Marketo实时个性化(RTP)平台并将其与Google Universal Analytics (GUA)帐户相集成。 RTP数据可以附加到您的GUA帐户，以便您查看和查看访问您网站的组织、行业、固件和RTP区段的性能。

**Google Universal Analytics**

利用RTP数据的Google Universal Analytics，您可以更好地了解B2B用户如何与您的在线内容进行交互，并有助于衡量个性化营销活动并从中获得更好的结果。 [详细了解Google Universal Analytics](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1).

>[!NOTE]
>
>**仅适用于Google Tag Manager用户**
>
>无需执行编码或特殊配置。 确保完成以下核对清单：
>
>* RTP维度是在Google Universal Analytics中创建的
>* [Google Tag Manager中正确安装了RTP标记](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* 已在RTP的帐户设置中启用Google Universal Analytics集成
>* [Google Universal Analytics标记已在Google Tag Manager中正确配置](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Google Tag Manager标记已正确安装您的网站](https://developers.google.com/tag-manager/quickstart)

## 在GUA中设置自定义Dimension {#set-up-custom-dimensions-in-gua}

1. 在Google Analytics中，

   1. 转到 **管理员**
   1. 选择 **帐户。**
   1. 选择 **属性。**
   1. 选择 **自定义定义** 和 **自定义Dimension**.
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. 添加新的自定义维度。 单击 **+新建自定义Dimension**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. 添加以下内容 **自定义Dimension：**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>自定义Dimension名称</strong></p></td> 
   <td><p><strong>范围</strong></p></td> 
   <td><p><strong>活跃</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP组织</strong></p></td> 
   <td><p>会话</p></td> 
   <td><p align="center">✓ “ ”标签</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP行业</strong></p></td> 
   <td><p>会话</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP类别</strong></p></td> 
   <td><p>会话</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP组</strong></p></td> 
   <td><p>会话</p></td> 
   <td><p align="center">✓</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**自定义Dimension名称** 必须与上表中的定义完全相同（否则，GUA中的自定义RTP仪表板和报告将无法正确显示）

1. 添加 **名称**. 选择作用域为 **会话**. 单击&#x200B;**创建**。

   ![](assets/image2014-11-29-11-3a12-3a51.png)

您的自定义Dimension列表应如下所示。

![](assets/image2014-11-29-11-36-50-version-2.png)

在GUA中激活自定义Dimension后，转到RTP平台以在RTP中启用这些维度。

## 在您的RTP帐户中激活GUA集成 {#activate-the-gua-integration-in-your-rtp-account}

1. 在RTP平台中，转到 **帐户设置。**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 下 **帐户设置**，单击 **域**.
1. 下 **分析**，单击 **Google Universal Analytics**.
1. 翻转 **日期** 将此数据从RTP附加到Google Universal Analytics的相关自定义Dimension和事件。
1. 输入 **索引号** 与GUA中的索引号对齐的维度的值。
1. 单击 **保存**.

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>自定义Dimension的索引号可以在GUA中的“自定义Dimension”下找到。
>
>示例： RTP行业索引编号等于1，RTP组织索引编号等于2。

## 删除Google Analytics中的旧仪表板 {#remove-old-dashboards-in-google-analytics}

1. 在Google Analytics中。 转到 **报表。**
1. 单击 **功能板。**
1. 选择 **仪表板** （RTP B2B或RTP性能）
1. 单击 **删除仪表板**.

![](assets/image2014-11-29-11-3a42-3a55.png)

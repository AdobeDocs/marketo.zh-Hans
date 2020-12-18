---
unique-page-id: 4720125
description: 将RTP与Google Universal Analytics集成- Marketo Docs —— 产品文档
title: 将RTP与Google Universal Analytics集成
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# 将RTP与Google Universal Analytics{#integrate-rtp-with-google-universal-analytics}集成

## 简介{#intro}

将Google Universal Analytics(GUA)与Marketo Real-Time Personalization&#39;s(RTP)的云图和个性化数据结合使用，以更好地衡量和分析您的在线营销工作。

本文介绍如何设置Marketo实时个性化(RTP)平台并将其与Google Universal Analytics(GUA)帐户集成。 RTP数据可附加到您的GUA帐户，以便您视图和查看访问您网站的组织、行业、图形和RTP区段的性能。

**Google Universal Analytics**

利用RTP数据的Google Universal Analytics，您可以更好地了解B2B用户如何与您的在线内容交互，并帮助衡量和从您的个性化活动中获得更好的结果。 [阅读有关Google Universal Analytics的更多信息](https://support.google.com/analytics/answer/2790010/?hl=en&amp;authuser=1)。

>[!NOTE]
>
>**`For Google Tag Manager Users Only`**
>
>无需进行编码或特殊配置。 确保您完成以下核对清单：
>
>* `RTP dimensions are created in Google Universal Analytics`
>* [RTP标签正确安装在Google标签管理器中](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* `Google Universal Analytics Integration is enabled in the RTP's Account Settings`
>* [Google Universal Analytics标签在Google标签管理器中正确配置](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Google标签管理器标签正确安装了您的网站](https://developers.google.com/tag-manager/quickstart)

>



## 在GUA {#set-up-custom-dimensions-in-gua}中设置自定义Dimension

1. 在Google Analytics,

   1. 转至&#x200B;**Admin**
   1. 选择&#x200B;**帐户。**
   1. 选择&#x200B;**属性。**
   1. 选择**自定义定义**和&#x200B;**自定义Dimension。**

      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. 添加新的自定义维。 单击&#x200B;**+新建自定义Dimension**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. 添加以下&#x200B;**自定义Dimension:**

<table> 
 <tbody> 
  <tr> 
   <td><p><strong>自定义Dimension名</strong></p></td> 
   <td><p><strong>范围</strong></p></td> 
   <td><p><strong>活动</strong></p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP组织</strong></p></td> 
   <td><p>会话</p></td> 
   <td><p align="center">选定</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP行业</strong></p></td> 
   <td><p>会话</p></td> 
   <td><p align="center">选定</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP类别</strong></p></td> 
   <td><p>会话</p></td> 
   <td><p align="center">选定</p></td> 
  </tr> 
  <tr> 
   <td><p><strong>RTP组</strong></p></td> 
   <td><p>会话</p></td> 
   <td><p align="center">选定</p></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**自定** 义Dimension名称必须与上表中的定义完全相同(否则GUA中的自定义RTP仪表板和报表将无法正确显示)

1. 添加**名称。 **将范围选为&#x200B;**会话。** 单击 **创建。**

   ![](assets/image2014-11-29-11-3a12-3a51.png)

您的自定义Dimension列表应当如下。

![](assets/image2014-11-29-11-36-50-version-2.png)

在GUA中激活自定义Dimension后，转到RTP平台以在RTP中启用这些维。

## 在RTP帐户{#activate-the-gua-integration-in-your-rtp-account}中激活GUA集成

1. 在RTP平台中，转到&#x200B;**帐户设置。**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 在&#x200B;**帐户设置**&#x200B;下，单击&#x200B;**域。**
1. 在**Analytics下，**单击&#x200B;**Google Universal Analytics**。
1. 打开&#x200B;****&#x200B;相关自定义Dimension和事件，将此数据从RTP附加到Google Universal Analytics。
1. 在GUA中输入与索引编号对齐的维的&#x200B;**索引编号**。
1. 单击&#x200B;**保存**。

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>自定义Dimension的索引编号可以在GUA的自定义Dimension下找到。
>
>示例：RTP行业索引编号等于1,RTP组织索引编号等于2。

## 删除Google Analytics{#remove-old-dashboards-in-google-analytics}中的旧仪表板

1. Google Analytics。 转至&#x200B;**报告。**
1. 单击&#x200B;**仪表板。**
1. 选择**仪表板**（RTP B2B或RTP性能）
1. 单击&#x200B;**删除仪表板**。

![](assets/image2014-11-29-11-3a42-3a55.png)


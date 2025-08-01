---
unique-page-id: 4720125
description: 将RTP与Google Universal Analytics集成 — Marketo文档 — 产品文档
title: 将RTP与Google Universal Analytics集成
exl-id: e8fc8730-c91d-44ad-8843-aa5b38f1ebd1
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 2%

---

# 将RTP与[!DNL Google Universal Analytics]集成 {#integrate-rtp-with-google-universal-analytics}

## 简介 {#intro}

利用[!DNL Google Universal Analytics] (GUA)和[!DNL Marketo Real-Time Personalization]的(RTP)固件和个性化数据，更好地衡量和分析您的在线营销工作。

此帖子说明如何设置和将[!DNL Marketo Real-Time Personalization] (RTP)平台与[!DNL Google Universal Analytics] (GUA)帐户集成。 RTP数据可附加到您的GUA帐户，以便您查看和查看访问您网站的组织、行业、固件和RTP区段的性能。

**[!DNL Google Universal Analytics]**

包含RTP数据的[!DNL Google Universal Analytics]可以让您更好地了解B2B用户如何与您的在线内容进行交互，并帮助衡量您的个性化营销活动并从中获得更好的结果。 [阅读有关 [!DNL Google Universal Analytics]](https://support.google.com/analytics/answer/2790010/?hl=en&authuser=1)的更多信息。

>[!NOTE]
>
>**仅适用于Google Tag Manager用户**
>
>无需执行编码或特殊配置。 确保完成以下核对清单：
>
>* RTP维度是在[!DNL Google Universal Analytics]中创建的
>* 已在Google Tag Manager中正确安装[RTP标记](https://docs.marketo.com/display/public/DOCS/Implementing+RTP+using+Google+Tag+Manager)
>* 已在RTP的帐户设置中启用[!DNL Google Universal Analytics]集成
>* 已在Google Tag Manager中正确配置[[!DNL Google Universal Analytics] 标记](https://support.google.com/tagmanager/answer/6107124?hl=en)
>* [Google Tag Manager标记已正确安装您的网站](https://developers.google.com/tag-manager/quickstart)

## 在GUA中设置自定义维度 {#set-up-custom-dimensions-in-gua}

1. 在Google Analytics中，

   1. 转到&#x200B;**[!UICONTROL Admin]**
   1. 选择&#x200B;**[!UICONTROL Account].**
   1. 选择&#x200B;**[!UICONTROL Property].**
   1. 选择&#x200B;**[!UICONTROL Custom Definitions]**&#x200B;和&#x200B;**[!UICONTROL Custom Dimensions]**。
      ![](assets/image2014-11-29-11-3a2-3a32.png)

1. 添加新的自定义维度。 单击 **[!UICONTROL +New Custom Dimension]**

   ![](assets/image2014-11-29-11-3a8-3a16.png)

1. 添加以下&#x200B;**[!UICONTROL Custom Dimensions]：**

<table>
 <tbody>
  <tr>
   <td><p><strong>自定义Dimension名称</strong></p></td>
   <td><p><strong>范围</strong></p></td>
   <td><p><strong>活动</strong></p></td>
  </tr>
  <tr>
   <td><p><strong>RTP组织</strong></p></td>
   <td><p>会话</p></td>
   <td><p align="center">✓</p></td>
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
>**自定义Dimension名称**&#x200B;必须与上表中的定义完全相同（否则将无法正确显示归国的自定义RTP功能板和报告）

1. 添加&#x200B;**[!UICONTROL Name]**。 选择作用域为&#x200B;**[!UICONTROL Session]**。 单击 **[!UICONTROL Create]**。

   ![](assets/image2014-11-29-11-3a12-3a51.png)

您的自定义Dimension列表应如下所示。

![](assets/image2014-11-29-11-36-50-version-2.png)

在GUA中激活自定义维度后，转到RTP平台以在RTP中启用这些维度。

## 在您的RTP帐户中激活GUA集成 {#activate-the-gua-integration-in-your-rtp-account}

1. 在RTP平台中，转到&#x200B;**[!UICONTROL Account Settings]。**

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 在&#x200B;**[!UICONTROL Account Settings]**&#x200B;下，单击&#x200B;**[!UICONTROL Domain]**。
1. 在&#x200B;**[!UICONTROL Analytics]**&#x200B;下，单击&#x200B;**[!UICONTROL Google Universal Analytics]**。
1. 将&#x200B;**[!UICONTROL On]**&#x200B;相关的自定义维度和事件转换为将此数据从RTP附加到[!DNL Google Universal Analytics]。
1. 输入与GUA中索引号对齐的维度的&#x200B;**[!UICONTROL Index number]**。
1. 单击 **[!UICONTROL Save]**。

![](assets/image2014-11-29-11-31-23-version-2.png)

>[!NOTE]
>
>自定义Dimension的索引号可以在GUA中的“自定义维度”下找到。
>
>示例： RTP-Industry Index Number equals 1， RTP-Organization Index Number equals 2.

## 删除Google Analytics中的旧仪表板 {#remove-old-dashboards-in-google-analytics}

1. 在Google Analytics中。 转到&#x200B;**[!UICONTROL Reporting].**
1. 单击&#x200B;**[!UICONTROL Dashboards].**
1. 选择&#x200B;**[!UICONTROL Dashboard]**（RTP B2B或RTP性能）
1. 单击 **[!UICONTROL Delete Dashboard]**。

![](assets/image2014-11-29-11-3a42-3a55.png)

---
unique-page-id: 2949158
description: 将RTP与Google Analytics集成 — Marketo文档 — 产品文档
title: 将RTP与Google Analytics集成
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
feature: Web Personalization
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# 将RTP与Google Analytics集成 {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics现在是操作标准，并且Google中的所有资产都已升级到Universal Analytics。
>
>本文会介绍如何使用旧的Google Standard Analytics，但我们建议您切换到Universal Analytics。
>
>如果您尚未使用[analytics.js跟踪代码](https://developers.google.com/analytics/devguides/collection/analyticsjs/)，Google强烈建议您重新标记网站以使用它。 Google将弃用以下内容：
>
>* ga.js
>* urchin.js
>* WAP/服务器端片段
>* YT/MO
>* 自定义变量
>* 用户定义的变量
>
>了解如何将[Web Personalization与Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)集成

## 简介 {#introduction}

使用从Marketo Real-Time Personalization (RTP)到Google Analytics (GA)帐户的直接数据流，从新的角度分析您的Web分析。 根据组织、行业和RTP促销活动衡量GA中的Web访问量。 查看量度，例如GA中的行业类型或RTP区段，以及它们如何根据不同的流量源（社交、付费、有机）执行和生成商机，分析促销活动的点击率，以及衡量个性化促销活动对您网站的影响。 利用这一能力，从您的RTP帐户中获得最大的好处

**RTP Audience Analytics**

通过集成，您可以在GA帐户中创建一个新维度。 RTP通过以下方式自动增强您的功能板：

1. 组织和行业
1. RTP中的自定义区段
1. Account-Based Marketing列表

关注您的关键B2B潜在客户。 按目标行业和细分市场分析渠道。

## 渠道报表 {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

RTP B2B仪表板可帮助您根据垂直和RTP分段了解访客的细分情况。 您可以根据金融业和不同的营销活动（付费、免费、社交）来查看访客表现。 仪表板还提供RTP区段执行情况的高级概述，并深入显示访问您网站的排名最前的组织。

## 行为流量 {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

行为流量报表（请参阅图像）可可视化访客从一个页面或事件前往下一个页面或事件的路径。 本图示例展示了金融行业所有访客的路径。 此报表可帮助您发现哪些内容可让访客持续参与您的网站。

## RTP性能 {#rtp-performance}

衡量您的RTP促销活动，并将其与您的整体网站平均值关联。 了解这些营销活动如何影响您的网站量度，并使用此数据将您的个性化工作集中在正确的目标上。 生成自定义报告以更好地了解个性化营销活动的执行情况。

![](assets/image2014-11-28-16-3a47-3a0.png)

## 使用Google Analytics设置RTP {#setting-up-rtp-with-google-analytics}

1. 将电子邮件<rtp.ga2@gmail.com>作为读取和分析用户添加到您的GA帐户。 有关详细信息，请参阅[此处](https://support.google.com/analytics/answer/2884495?hl=en)。

1. 在您的RTP帐户中。 转到&#x200B;**[!UICONTROL Account Settings]**。

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. 在&#x200B;**[!UICONTROL Account Settings]**、**[!UICONTROL Domain]**&#x200B;和&#x200B;**[!UICONTROL Analytics]**&#x200B;下。

1. 单击&#x200B;**Google Analytics**。

1. 打开相关的&#x200B;**自定义变量**&#x200B;和&#x200B;**事件**&#x200B;以将此数据从RTP附加到Google Analytics。

1. 输入&#x200B;**插槽**&#x200B;编号以发送自定义变量数据（默认值为1,2）。

![](assets/image2014-11-28-17-3a0-3a17.png)

1. 单击 **[!UICONTROL Save]**。

>[!NOTE]
>
>若要将区段数据发送到GA，请在RTP平台的[[!UICONTROL Edit Segment]页面](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)下选中复选框&#x200B;**[!UICONTROL Send Event to Google Analytics on Segment Match]**。

## 使用RTP数据设置Google Analytics报表 {#setting-up-google-analytics-reports-with-rtp-data}

在Google Analytics中，您可以使用功能板、GA分段和报表来查看RTP数据：

* [功能板](https://support.google.com/analytics/answer/1068216?hl=en)提供网站性能的概述。
* GA区段用于在GA界面中过滤访客，并查看每个区段的流量。 在[此处](https://support.google.com/analytics/answer/3124493?hl=en)查看如何生成区段。
* 正在创建[自定义报告](https://support.google.com/analytics/answer/1033013?hl=en)以查看和/或设置计划的电子邮件。 在&#x200B;**[!UICONTROL Customization]** > **[!UICONTROL New Custom Report]**&#x200B;下查看。

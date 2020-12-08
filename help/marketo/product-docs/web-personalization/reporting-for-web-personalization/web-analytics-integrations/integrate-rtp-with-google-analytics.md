---
unique-page-id: 2949158
description: 将RTP与Google Analytics集成- Marketo Docs —— 产品文档
title: 将RTP与Google Analytics集成
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---


# 将RTP与Google Analytics集成 {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics现在是操作标准，Google中的所有属性已升级到Universal Analytics。
>
>本文介绍如何使用旧版Google Standard Analytics，但建议您切换到Universal Analytics。
>
>如果您尚未使用analytics.js [跟踪代码](https://developers.google.com/analytics/devguides/collection/analyticsjs/),Google强烈建议您重新标记网站以使用它。 Google正在弃用以下内容：
>
>* ga.js
>* urchin.js
>* WAP/服务器端片段
>* YT /月
>* 自定义变量
>* 用户定义的变量

>
>
了解如何将Web个 [性化与通用分析相集成](integrate-rtp-with-google-universal-analytics.md)

## 简介 {#introduction}

使用从Marketo实时个性化(RTP)到Google Analytics(GA)帐户的直接数据流，从新角度分析您的网络分析。 根据组织、行业和RTP活动，在GA中衡量您的Web访问。 视图指标，如GA中的行业类型或RTP段，以及它们如何根据不同的流量源（社交、付费、有机）执行和生成潜在客户，分析活动的点击率，并衡量个性化活动对您网站的影响。 利用此功能，从您的RTP帐户获得最大益处

**RTPAudience Analytics**

通过集成，您的GA帐户将拥有一个新维度。 RTP可通过以下方式自动增强仪表板:

1. 组织和行业
1. RTP中的自定义段
1. 基于帐户的营销列表

专注于您的关键B2B潜在客户。 按目标行业和细分分析渠道。

## 渠道报告 {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

RTP B2B仪表板可帮助您根据垂直和RTP分段了解访客的细分。 您可以根据金融业和不同的营销活动（付费、有机、社交）来查看访客绩效。 该仪表板还提供RTP区段执行情况的高级概述，并深入探讨，以显示访问您网站的顶级组织。

## 行为流 {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

行为流报告（请参阅图像）可视化访客从一个页面或事件到下一个页面的路径。 图例显示了所有金融部门访客的路径。 此报告可帮助您发现哪些内容可让访客与您的网站保持互动。

## RTP性能 {#rtp-performance}

衡量您的RTP活动并将它们与您的整个站点平均值关联。 了解这些活动如何影响您的网站指标，并使用此数据将您的个性化工作重点放在正确的目标上。 生成自定义报告以更好地了解您的个性化活动的表现。

![](assets/image2014-11-28-16-3a47-3a0.png)

## 使用Google Analytics设置RTP {#setting-up-rtp-with-google-analytics}

1. 以阅读和 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#0674727628616734466b67746d6372692865696b)分析用户身份添加电子邮件到您的GA帐户。 有关详细信息，请参 [阅此处](https://support.google.com/analytics/answer/2884495?hl=en)。
1. 在RTP帐户中。 转到“帐 **户设置**”。

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. 在“帐 **户设置**”、“ **域** ”和“ **分析”下**
1. 单击**Google Analytics。**
1. 打开相关的 **自定义变** 量 **和事件** ，将RTP中的此数据追加到Google Analytics。
1. 输入插 **槽号** ，以发送自定义变量数据（默认值为1,2）。

![](assets/image2014-11-28-17-3a0-3a17.png)

单击 **保存**。

>[!NOTE]
>
>要向GA发送段事件，请在RTP平台的“编 [辑段”页](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) ，选中复选框“将段 **发送到Google Analytics匹配”**。

## 使用RTPGoogle Analytics设置数据报告 {#setting-up-google-analytics-reports-with-rtp-data}

在Google Analytics中，您可以使用仪表板、GA分段和报告来视图RTP数据：

* [仪表板](https://support.google.com/analytics/answer/1068216?hl=en) 提供网站性能概述。
* GA段用于过滤GA接口中的访客，并视图每个段的流量。 了解如何在此处构建 [区段](https://support.google.com/analytics/answer/3124493?hl=en)。
* 创建 [自定义报告](https://support.google.com/analytics/answer/1033013?hl=en) ，以视图和／或设置定时电子邮件。 请参阅“自定义”>“新建自定义报告”下。

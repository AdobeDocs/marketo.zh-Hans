---
unique-page-id: 2949160
description: 与Adobe Analytics集成 — Marketo文档 — 产品文档
title: 与 Adobe Analytics 集成
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 1%

---

# 与 Adobe Analytics 集成 {#integrate-with-adobe-analytics}

## 简介 {#intro}

通过查看Adobe Analytics帐户中的组织、行业和[!DNL Marketo Real-Time Personalization] (RTP)促销活动数据，从B2B角度分析Web分析。

本文档启用[!DNL Marketo Real-Time Personalization] (RTP)与Adobe Adobe Analytics之间的集成。 利用来自RTP的数据，可检测和分析所有访问您网站的行业细分和组织中的趋势，并衡量RTP促销活动的有效性，从而提供见解和分析，以获得最佳结果。

您可以通过查看每个区段中的新访客与回访访客数量等量度，分析促销活动的点击率，并发现哪些行业和自定义区段以及实时促销活动产生了最佳的转化商机，来实现这一点。 利用这一能力，从您的RTP帐户中获得最大的好处。

## RTP AUDIENCE ANALYTICS {#rtp-audience-analytics}

通过RTP - AA集成，您的网站分析界面中新增了一个维度。 RTP会自动通过以下方式增强您的Web分析功能板：

1. 组织和行业数据
1. 自定义的RTP区段
1. 指定帐户列表(Account-Based Marketing)

这增强了您的B2B数据，并允许您通过优化以下内容来关注相关访客：

1. 出站渠道
1. 内容
1. 重定向

## 渠道报表 {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

RTP功能板可帮助您了解访客如何根据纵向和RTP区段进行细分。 您可以根据行业以及与行业相关的不同营销活动（付费、免费、社交）来查看访客表现。 仪表板还提供了访客根据其行业类型查看哪些网站区域的高级概述。

## 行为报表 {#behavioral-report}

可以在Adobe Analytics中根据组织、行业和RTP区段数据创建各种行为报表。 这些流量报表可可视化访客从一个页面或事件转到下一个页面或事件的路径。 此报表可帮助您发现哪些内容可让访客持续参与您的网站。

## RTP性能 {#rtp-performance}

在Adobe Analytics的自定义链接下查看RTP促销活动展示和转化。

此自定义链接报表将按以下命名格式显示营销活动的展示次数和转化次数：

* 展示ISegment： [RTP段名称]，ICampaign： [RTP促销活动名称]
* 转换ISegment： [RTP区段名称]，ICampaign： [RTP促销活动名称]

![](assets/custom-links-report.png)

## 在Adobe Analytics中设置 {#set-up-in-adobe-analytics}

该集成使用Adobe Analytics提供的JavaScript API。 在集成中使用自定义转化变量(eVar)、自定义事件（事件）和流量变量。 必须从AA Admin中启用“全部”。 您必须在A中设置转化变量、自定义事件和流量变量，否则您将看不到包中的数据，即使您在RTP中启用了它。

完成以下步骤以在AA中设置这些变量：

1. 转到AA帐户中的&#x200B;**[!UICONTROL Admin Tools]**。
1. 选择要与集成一起使用的&#x200B;**[!UICONTROL Report Suite]**。
1. 在&#x200B;**[!UICONTROL Edit Settings]**&#x200B;下，转到&#x200B;**[!UICONTROL Conversion]**&#x200B;并选择&#x200B;**[[!UICONTROL Conversion Variables]](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**。
选择[转化变量](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar)编号（我们推荐）：

   1. 适用于行业自定义转化的Evar # 20
   1. 适用于组织自定义转化的Evar # 21

   >[!NOTE]
   >
   >如果选择了这些#，请选择另一个可用号码。 将此号码与“RTP帐户设置”中的插槽编号对齐。

   1. 将状态更改为_[!UICONTROL Enabled_]。

      1. 将名称更改为&#x200B;**行业**&#x200B;和&#x200B;**组织**。 （它将显示在报表包中。）

      1. 将“过期时间”字段更改为&#x200B;**[!UICONTROL Visit]**。

1. 在&#x200B;**[!UICONTROL Edit Settings]**&#x200B;下，转到&#x200B;**[!UICONTROL Conversion]**&#x200B;并选择&#x200B;**[[!UICONTROL Success Events]](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**。

   1. 选择自定义成功事件事件编号（我们推荐）：

      1. RTP营销活动的event20
      1. event21用于RTP段

      >[!NOTE]
      >
      >如果选择了这些#，请选择另一个可用号码。 将此号码与“RTP帐户设置”中的插槽编号对齐。

      1. 将两个事件名称更改为&#x200B;**RTP营销活动**&#x200B;和&#x200B;**RTP区段**。 这是将显示在报表包中的名称。

   1. 选择类型为&#x200B;**计数器（无子关系）**&#x200B;的字段

1. 在&#x200B;**[!UICONTROL Edit Settings]**&#x200B;下，转到&#x200B;**[流量](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)**&#x200B;并选择&#x200B;**[流量变量](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**。

   1. 选择流量变量属性# （我们推荐）：

      1. 属性# 20 — 名称：RTP区段组织
      1. 属性# 21 — 名称： RTP区段行业
      1. 属性# 25 — 名称：Campaign组织
      1. 属性# 26 — 名称： RTP Campaign行业

      >[!NOTE]
      >
      >如果选择了这些#，请选择另一个可用号码。 将此编号与RTP帐户设置中的插槽编号对齐)

      1. 更改4个属性名称。 这是将显示在报表包中的名称。

   1. 选择[!UICONTROL Enabled]的&#x200B;**[!UICONTROL Enabled]**&#x200B;字段。

   1. 选择[!UICONTROL Path Reports]的&#x200B;**[!UICONTROL Enabled]**&#x200B;字段。

## 在[!DNL Marketo Real-Time Personalization] (RTP)中设置 {#set-up-in-marketo-real-time-personalization-rtp}

1. 在RTP平台中，转到&#x200B;**[!UICONTROL Account Settings]**。

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 在&#x200B;**[!UICONTROL Account Settings]**&#x200B;下，单击&#x200B;**[!UICONTROL Domain]**。
1. 在&#x200B;**[!UICONTROL Analytics]**&#x200B;下，单击&#x200B;**Adobe Analytics**。
1. 将&#x200B;**[!UICONTROL On]**&#x200B;转化、自定义和流量变量切换。
1. 分配转换、事件和流量变量&#x200B;**插槽编号**&#x200B;以匹配在AA中创建的插槽编号
1. 单击 **[!UICONTROL Save]**。

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>我们推荐的时隙设置为
>
>**转化变量**
>
>* [!UICONTROL Industry Custom Conversions] — 插槽20
>* [!UICONTROL Organization Custom Conversions] — 插槽21
>
>**自定义事件**
>
>* [!UICONTROL Campaign Custom Event] — 插槽20
>* [!UICONTROL Segment Custom Event] — 插槽21
>
>**流量变量**
>
>* [!UICONTROL Segment Organization Traffic Variable] — 插槽20
>* [!UICONTROL Segment Industry Traffic Variable] — 插槽21
>* [!UICONTROL Campaign Organization Traffic Variable] — 插槽22
>* [!UICONTROL Campaign Industry Traffic Variable] — 插槽23
>
>**确保这些插槽编号与AA中创建的变量和事件编号一致。**

## 报告 {#reports}

根据组织名称、行业和RTP区段以及实时营销活动数据创建增强的SiteAdobe Analytics报表。

AA中的自定义报告和功能板示例包括：

* 按行业或定义的区段列出的绩效（基于帐户的指定列表）
* 按KPI绩效的行业细分
* 每个组织查看的页面数
* 根据组织、行业、细分市场了解营销渠道表现

**报告示例 —**

**热门行业报告**

![](assets/top-industries-report.png)

**组织报表**

![](assets/image2014-11-29-12-3a29-3a42.png)

**正在创建RTP仪表板**

创建一个[新仪表板](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html)，名为&#x200B;**RTP仪表板**。 此仪表板有助于了解访客根据纵向和RTP区段进行的细分。

1. 单击&#x200B;**[!UICONTROL Dashboard]，**&#x200B;单击&#x200B;**[!UICONTROL Add Dashboard]**。

1. 命名仪表板&#x200B;**RTP仪表板**。

1. 选择&#x200B;**仪表板大小** 3 x 2， 2 x 2。

1. 创建[缩图报表](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3)并将[内容添加到功能板](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard)。

将行业缩图报表添加到功能板

1. 转到&#x200B;**[!UICONTROL Custom Conversions]**，单击&#x200B;**[!UICONTROL Industry]**。

1. 将图形配置为&#x200B;**饼图**。

1. 单击&#x200B;**[!UICONTROL Dashboard]**，添加&#x200B;**[!UICONTROL Reportlet]**。

1. 将报告命名为&#x200B;**热门行业**。

1. 放在仪表板&#x200B;**RTP仪表板**&#x200B;中。

1. 创建&#x200B;**新**。

将区段缩图报表添加到功能板

1. 转到&#x200B;**[!UICONTROL Site Metrics]**。 单击&#x200B;**[!UICONTROL Custom Events]**，**[!UICONTROL Segments]**。

1. 将图形配置为&#x200B;**垂直条**。

1. 单击&#x200B;**[!UICONTROL Dashboard]**，添加&#x200B;**[!UICONTROL Reportlet]**。

1. 将报表命名为&#x200B;**热门区段**。

1. 放在仪表板&#x200B;**RTP仪表板**&#x200B;中。

1. 创建&#x200B;**新**。

您的缩图报表将显示在功能板中。

## 在Adobe Analytics中查看展示次数和点击次数（转化） {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. 单击&#x200B;**[!UICONTROL Custom]链接**。

   ![](assets/sitecatalyst1-1.png)

1. 搜索展示次数以查看表示营销活动展示次数的区段和营销活动名称。
   ![](assets/sitecatalyst1.png)

1. 搜索转化以查看表示促销活动点击数的区段和促销活动名称。

   ![](assets/sitecatalyst2.png)

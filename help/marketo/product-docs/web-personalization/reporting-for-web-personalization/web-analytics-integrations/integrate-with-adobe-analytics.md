---
unique-page-id: 2949160
description: 与Adobe Analytics集成 — Marketo文档 — 产品文档
title: 与Adobe Analytics集成
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---

# 与Adobe Analytics集成 {#integrate-with-adobe-analytics}

## 简介 {#intro}

通过查看Adobe Analytics帐户中的组织、行业和Marketo实时个性化(RTP)促销活动数据，从B2B角度分析Web分析。

本文档支持将Marketo实时个性化(RTP)与AdobeAdobe Analytics相集成。 RTP数据将允许您检测和分析访问您网站的所有行业区段和组织的趋势，并衡量RTP促销活动的有效性，从而提供洞察和分析以获得最佳结果。

您可以通过以下方式实现这一点：查看每个区段中新访客数与回访访客数之类的量度，分析促销活动的点击率，发现哪些行业和自定义区段以及实时促销活动生成了最佳转化潜在客户。 利用此功能，从您的RTP帐户中获得最大的好处。

## RTPAudience Analytics {#rtp-audience-analytics}

通过RTP - AA集成，您的Web分析界面中有一个新维度。 RTP会通过以下功能自动增强您的Web分析功能板：

1. 组织和行业数据
1. 自定义的RTP区段
1. 指定帐户列表(Account-Based Marketing)

这可增强您的B2B数据，并允许您通过优化以下各项来重点关注相关访客：

1. 出站渠道
1. 内容
1. 重定位

## 渠道报表 {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

RTP仪表板有助于您了解根据垂直行业和RTP区段划分访客的情况。 您可以根据行业以及与行业相关的不同营销活动（付费、免费、社交）来查看访客的效果。 功能板还根据访客的行业类型提供了访客正在查看的网站区域的高级概述。

## 行为报表 {#behavioral-report}

可以在Adobe Analytics中根据组织、行业和RTP区段数据创建不同的行为报告。 这些流量报表可显示访客从一个页面或事件到下一页面的路径。 此报表可帮助您发现哪些内容可让访客持续参与您的网站。

## RTP性能 {#rtp-performance}

在Adobe Analytics的自定义链接下查看RTP促销活动展示和转化。

此自定义链接报表将以下命名格式显示营销活动的展示次数和转化次数：

* 展示区段： [RTP区段名称]，促销活动： [RTP促销活动名称]
* 转化区段： [RTP区段名称]，促销活动： [RTP促销活动名称]

![](assets/custom-links-report.png)

## 在Adobe Analytics中设置 {#set-up-in-adobe-analytics}

该集成使用Adobe Analytics提供的JavaScript API。 集成中使用自定义转化变量(eVar)、自定义事件（事件）和流量变量。 必须从AA管理员中启用所有。 您必须在AA中设置转化变量、自定义事件和流量变量，否则即使在RTP中启用了该变量，您也无法在包中查看数据。

完成以下步骤以在AA中设置这些变量：

1. 转到 **管理工具** 在您的AA帐户中。
1. 选择 **报表包** 与集成一起使用时，不会将其标记为问题。
1. 在 **编辑设置**，转到 **转化** 选择 **[转化变量](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   选择 [转化变量](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) 数字（我们建议）：

   1. 用于行业自定义转化的Evar # 20
   1. 用于组织自定义转化的Evar # 21

   >[!NOTE]
   >
   >如果取得这些#，请选择另一个可用的编号。 将此数字与RTP帐户设置中的时隙数相一致。

   1. 将状态更改为 _已启用_.

      1. 将名称更改为 **行业** 和 **组织**. （这是报表包中的显示方式。）

      1. 将“过期时间”字段更改为 **访问**.


1. 在 **编辑设置** 转到 **转化** 选择 **[成功事件](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

   1. 选择自定义成功事件事件编号（我们建议）：

      1. 用于RTP促销活动的event20
      1. 用于RTP区段的event21

      >[!NOTE]
      >
      >如果取得这些#，请选择另一个可用的编号。 将此数字与RTP帐户设置中的时隙数相一致。

      1. 将两个事件名称更改为 **RTP营销活动** 和 **RTP区段**. 这是将在报表包中显示的名称。
   1. 选择要变为 **计数器（无子关系）**



1. 在 **编辑设置** 转到 **[流量](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)** 选择 **[流量变量](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. 选择流量变量属性#（我们建议）：

      1. 属性# 20 — 名称：RTP区段组织
      1. 属性# 21 — 名称：RTP区段行业
      1. 属性# 25 — 名称：营销活动组织
      1. 属性# 26 — 名称：RTP促销活动行业

      >[!NOTE]
      >
      >如果取得这些#，请选择另一个可用的编号。 将此数字与RTP帐户设置中的时隙数相一致)

      1. 更改4个属性名称。 这是将在报表包中显示的名称。
   1. 选择要启用的字段 **已启用**.

   1. 选择路径报表字段 **已启用**.



## 在Marketo实时个性化(RTP)中设置 {#set-up-in-marketo-real-time-personalization-rtp}

1. 在RTP平台中，转到 **帐户设置**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 在 **帐户设置**，单击 **域**.
1. 在 **Analytics中，单击** **Adobe Analytics**.
1. 转 **开** “转化”、“自定义”和“流量”变量切换。
1. 分配转化、事件和流量变量 **槽号** 以匹配在AA中创建的插槽号
1. 单击 **保存**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>我们推荐的插槽设置为
>
>**转化变量**
>
>* 行业自定义转化 — 插槽20
>* 组织自定义转化 — 插槽21
>
>**自定义事件**
>
>* 促销活动自定义事件 — 插槽20
>* 区段自定义事件 — 插槽21
>
>**流量变量**
>
>* 区段组织流量变量 — 插槽20
>* 区段行业流量变量 — 插槽21
>* 促销活动组织流量变量 — 插槽22
>* 促销活动行业流量变量 — 插槽23
>
>**确保这些插槽编号与AA中创建的变量和事件编号一致。**

## 报告 {#reports}

根据组织名称、行业和RTP区段以及实时促销活动数据创建增强的SiteAdobe Analytics报表。

AA中自定义报表和功能板的示例包括：

* 按行业或定义的区段（基于帐户的命名列表）的性能
* 按KPI绩效划分行业细分
* 每个组织查看的页面数
* 按组织、行业、区段划分的营销渠道绩效

**— 报表示例 —**

**热门行业报表**

![](assets/top-industries-report.png)

**组织报表**

![](assets/image2014-11-29-12-3a29-3a42.png)

**创建RTP仪表板**

创建 [新仪表板](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html)，调用 **RTP仪表板**. 此功能板将帮助了解根据垂直行业和RTP区段划分的访客。

1. 单击 **功能板、** 单击 **添加功能板**.

1. 命名功能板 **RTP仪表板**.

1. 选择 **仪表板大小** 3 x 2, 2 x 2。

1. 创建 [缩图报表](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) 添加 [功能板内容](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard).

将行业缩图报表添加到功能板

1. 转到 **自定义转化**，单击 **行业**.

1. 将图形配置为 **饼图**.

1. 单击 **功能板**，添加 **缩图报表**.

1. 命名报表 **热门行业**.

1. 置于功能板中 **RTP仪表板**.

1. 创建 **新建**.

将区段缩图报表添加到功能板

1. 转到 **网站量度**. 单击 **自定义事件**, **区段**.

1. 将图形配置为 **垂直条**.

1. 单击 **功能板**，添加 **缩图报表**.

1. 命名报表 **热门区段**.

1. 置于功能板中 **RTP仪表板**.

1. 创建 **新建**.

您的缩图报表将显示在功能板中。

## 在Adobe Analytics中查看展示次数和点击次数（转化） {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. 单击 **自定义链接**.

   ![](assets/sitecatalyst1-1.png)

1. 搜索“展示次数”以查看表示营销活动展示次数的“区段”和“营销活动名称”。\
   ![](assets/sitecatalyst1.png)

1. 搜索“转化”以查看表示促销活动点击次数的区段和促销活动名称。

   ![](assets/sitecatalyst2.png)

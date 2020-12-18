---
unique-page-id: 2949160
description: 与Adobe Analytics集成- Marketo Docs —— 产品文档
title: 与Adobe Analytics集成
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---


# 与Adobe Analytics集成{#integrate-with-adobe-analytics}

## 简介{#intro}

从B2B的角度分析您的网络分析，在您的Adobe Analytics帐户中查看组织、行业和营销实时个性化(RTP)活动数据。

此文档支持Marketo实时个性化(RTP)与AdobeAdobe Analytics之间的集成。 通过RTP活动，您可以检测和分析所有行业细分和组织访问您网站的趋势并衡量RTP分析的有效性，从而提供洞察和以获得最佳结果。

您可以通过以下方式实现这一点：查看每个细分中新访客数与退回数，分析活动的点击率，发现哪些行业和定制细分以及实时活动生成了转化率最高的潜在客户。 利用此功能，您可以从RTP帐户中获得最大益处。

## RTPAudience Analytics{#rtp-audience-analytics}

通过RTP - AA集成，您的Web分析界面中具有新的维度。 RTP可通过以下方式自动增强Web分析仪表板:

1. 组织和行业数据
1. 自定义RTP段
1. 指定帐户列表（基于帐户的营销）

这可增强您的B2B数据，并允许您通过优化以下各项来专注于相关访客:

1. 出站渠道
1. 内容
1. 重新定位

## 渠道报告{#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

RTP仪表板可帮助您根据垂直和RTP段了解访客细分。 您可以根据行业和与行业相关的不同营销活动（付费、有机、社交）来查看访客绩效。 该仪表板还根据访客所在行业的类型，提供您正在查看的站点部分的高级概述。

## 行为报告{#behavioral-report}

在Adobe Analytics，可以根据组织、行业和RTP段数据创建不同的行为报告。 这些流报表可视化访客从一个页面或事件到下一个页面的路径。 此报告可帮助您发现哪些内容可让访客与您的网站保持互动。

## RTP性能{#rtp-performance}

视图Adobe Analytics自定义链接下的RTP活动印象和转换。

此自定义链接报告将以下命名格式显示活动的展示次数和转换率：

* 印象区段：[RTP段名称],ICampaign:[RTP活动名称]
* 转换区段：[RTP段名称],ICampaign:[RTP活动名称]

![](assets/custom-links-report.png)

## 在Adobe Analytics设置{#set-up-in-adobe-analytics}

该集成使用Adobe Analytics优惠的JavaScript API。 集成中使用自定义转换变量(eVar)、自定义事件(事件)和流量变量。 必须从AA管理员中启用所有组件。 您必须在AA中设置转换变量、自定义事件和流量变量，否则即使在RTP中启用数据，您也无法在套件中查看数据。

完成以下步骤以在AA中设置这些变量：

1. 转到AA帐户中的&#x200B;**管理工具**。
1. 选择要与集成一起使用的&#x200B;**报表包**。
1. 在&#x200B;**编辑设置下，**&#x200B;转至&#x200B;**转换**&#x200B;并选择** [转换变量](http://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**。\
   选择[转换变量](http://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar)编号（我们建议）:

   1. 

      1. 行业自定义转化的Evar # 20
      1. 组织自定义转换的Evar # 21

         >[!NOTE]
         >
         >如果这些#被采用，请选择其他可用编号。 将此编号与RTP帐户设置中的插槽编号对齐。

      1. 将状态更改为*已启用*

         1. 将“名称”更改为&#x200B;**Industry**&#x200B;和&#x200B;**Organization**。 （这是报表包中的显示方式。）

         1. 将“过期时间”字段更改为&#x200B;**访问。**

1. 在“**编辑设置&#x200B;**”下，转至**&#x200B;转换&#x200B;**并选择“** [成功事件](http://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**”。

1. 选择自定义成功事件事件编号（我们建议）:

   1. 事件20用于RTP活动
   1. 事件21 for RTP段

      >[!NOTE]
      >
      >如果这些#被采用，请选择其他可用编号。 将此编号与RTP帐户设置中的插槽编号对齐。

   1. 将两个事件名称更改为&#x200B;**RTP活动**&#x200B;和&#x200B;**RTP段**。 这是将显示在报表包中的名称。

1. 选择类型* *字段，使其成为&#x200B;**计数器（无子关系）**

1. 在&#x200B;**编辑设置**&#x200B;下，转到** [流量](http://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable) **并选择** [流量变量](http://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**。

   1. 选择流量变量属性#（我们建议）:

      1. 属性编号20 —— 名称：RTP段组织
      1. 属性编号21 —— 名称：RTP段行业
      1. 属性编号25 —— 名称：活动组织
      1. 属性编号26 —— 名称：RTP活动行业

         >[!NOTE]
         >
         >如果这些#被采用，请选择其他可用编号。 将此编号与RTP帐户设置中的插槽编号对齐)

      1. 更改4个属性名称。 这是将显示在报表包中的名称。
   1. 选择“启用”字段以&#x200B;**启用**
   1. 选择“路径报告”字段以&#x200B;**启用**


## 在Marketo实时个性化(RTP)中设置{#set-up-in-marketo-real-time-personalization-rtp}

1. 在RTP平台中，转到&#x200B;**帐户设置**。

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. 在&#x200B;**帐户设置**&#x200B;下，单击&#x200B;**域**。
1. 在“**分析”下，单击** **Adobe Analytics**。
1. 打开**转换、自定义和流量变量切换。
1. 分配转换、事件和流量变量&#x200B;**插槽编号**&#x200B;以匹配在AA中创建的插槽编号
1. 单击&#x200B;**SAVE**。

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>我们推荐的插槽设置是
>
>**转换变量**
>
>* 行业自定义转化——第20位
>* 组织自定义转换——插槽21

>
>
**自定义事件**
>
>* 活动自定义事件-插槽20
>* 区段自定义事件-插槽21

>
>
**流量变量**
>
>* 段组织流量变量——插槽20
>* 细分行业流量变量——插槽21
>* 活动组织流量变量——插槽22
>* 活动行业流量变量——插槽23

>
>
**确保这些插槽编号与在AA中创建的变量和事件编号对齐。**

## 报告{#reports}

根据组织名称、行业和RTP细分以及实时活动数据创建增强的SiteAdobe Analytics报告。

AA中的自定义报告和仪表板示例包括：

* 按行业或定义的细分表现(基于帐户的指定列表)
* 按KPI表现划分的行业
* 每个组织查看的页面数
* 按组织、行业、细分进行的营销渠道绩效

**报告示例**

**热门行业报告**

** ![](assets/top-industries-report.png)

**

**组织报告**

![](assets/image2014-11-29-12-3a29-3a42.png)

**创建RTP仪表板**

创建名为&#x200B;**RTP仪表板**&#x200B;的[新仪表板](http://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html)。 此仪表板将帮助您了解根据垂直市场和RTP细分的访客。

1. 单击&#x200B;**仪表板,**&#x200B;单击**添加仪表板**

1. 命名仪表板&#x200B;**RTP仪表板**
1. 选择&#x200B;**仪表板大小** 3 x 2、2 x 2
1. 创建[reportlet](http://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3)并将[内容添加到仪表板](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard)

向仪表板添加行业报告

1. 转至&#x200B;**自定义转换**，单击&#x200B;**Industry**

1. 将图形配置为&#x200B;**饼图**
1. 单击&#x200B;**仪表板**，添加&#x200B;**Reportlet**

1. 将报告命名为&#x200B;**Top Industries**
1. 置入仪表板&#x200B;**RTP仪表板**
1. 创建&#x200B;**新建**。

将区段报表添加到仪表板

1. 转至**网站指标，**单击&#x200B;**自定义事件，区段**

1. 将图形配置为&#x200B;**垂直条**
1. 单击&#x200B;**仪表板**，添加&#x200B;**Reportlet**

1. 将报告命名为&#x200B;**顶部区段**
1. 置入仪表板&#x200B;**RTP仪表板**
1. 创建&#x200B;**新建。**

您的报表将显示在仪表板中。

## Adobe Analytics{#view-impressions-and-clicks-conversions-in-adobe-analytics}的视图印象和点击（转换）

1. 单击“自定义链接”。

   ![](assets/sitecatalyst1-1.png)

1. 搜索视图区段的展示数和表示活动展示数的活动名称。\
   ![](assets/sitecatalyst1.png)

1. 搜索“转换为视图段”和活动名称，它们表示活动的点击次数。

   ![](assets/sitecatalyst2.png)


---
unique-page-id: 7504676
description: 了解期间成本 — Marketo文档 — 产品文档
title: 了解期间成本
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 了解期间成本 {#understanding-period-costs}

## 概述 {#overview}

期间成本是指您在特定月份花在项目上的钱。

>[!NOTE]
>
>**示例**
>
>如果你花1000美元聘请一位插图师，为今年7月推出的电子书做插图，那么电子书计划在7月将有1000美元的时段成本。
>
>如果您每月在Google Adwords上花费200美元 — Google Adwords程序的时段成本为200美元 **每月**.

>[!NOTE]
>
>[了解项目群](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[了解计划会员资格](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## 期间成本的计算方式 {#how-period-costs-are-calculated}

想象一下发生在三月的事件，就像一个网络研讨会。 1月和2月的广告会提前招募新人。 活动结束后，当人们在4月和5月下载网络研讨会时，也会获得新的联系人。

1. 单周期成本归因于3月……

   ![](assets/graph1.png)

   ...之前和之后几个月添加的联系人将 *仅限* 数到三月。

   ![](assets/graph2.png)

1. 期间成本归因于一月、二月及三月……

   ![](assets/graph3.png)

   ...仅在3月之后几个月内添加的联系人将计为3月。

   ![](assets/graph4.png)

1. 期间成本归于一月及四月……

   ![](assets/graph5.png)

   ...1月到3月新增的联系人将计为1月。 4月和5月新增的联系人将计为4月。

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >总之，没有定义期间成本的月份将“回滚”到定义的最后一个月份。 如果没有前期成本，则月份将“前转”到已定义的下一个月份。 如果尚未定义期间成本 _任意_ 月，RCE中的报告将不可用于该计划。

   >[!MORELIKETHIS]
   >
   >* [在程序中使用期间成本](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [按期间成本筛选项目报告](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)

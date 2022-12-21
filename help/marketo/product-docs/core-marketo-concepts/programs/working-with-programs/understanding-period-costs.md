---
unique-page-id: 7504676
description: 了解期间成本 — Marketo文档 — 产品文档
title: 了解期间成本
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 了解期间成本 {#understanding-period-costs}

## 概述 {#overview}

期间成本是指您在某个计划的特定月份花费的资金。

>[!NOTE]
>
>**示例**
>
>如果你花1000美元为7月份推出的电子书聘请插画师，电子书计划在7月份的时段成本将为1000美元。
>
>如果您每月在Google Adwords上花费200美元，则Google Adwords计划的时段成本为200美元 **每月**.

>[!NOTE]
>
>[了解程序](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[了解计划会员资格](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## 期间成本的计算方式 {#how-period-costs-are-calculated}

想象一下，3月将举行一次网络研讨会。 新人员在一、二月份从广告业预先获取。 在活动结束后，用户也会在4月和5月下载网络研讨会，从而获得新的联系人。

1. 单个期间成本应归因于3月……

   ![](assets/graph1.png)

   ...在遗嘱前后的月份中添加的联系人 *仅* 数到三月。

   ![](assets/graph2.png)

1. 期间成本应归因于1月、2月和3月……

   ![](assets/graph3.png)

   ...仅在3月之后的月份添加的联系人将计入3月份。

   ![](assets/graph4.png)

1. 期间成本归因于1月和4月……

   ![](assets/graph5.png)

   ...在1月到3月添加的联系人将计入1月。 在4月和5月添加的联系人将计入4月。

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >总之 — 没有定义期间成本的月份将“向后”滚动到定义的最后一个月份。 如果没有前期成本，则月份将被“前转”到已定义的下一个月份。 如果尚未为 _any_ 月后，该计划将无法使用RCE报告。

   >[!MORELIKETHIS]
   >
   >* [在程序中使用期间成本](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [按期间成本筛选程序报表](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)


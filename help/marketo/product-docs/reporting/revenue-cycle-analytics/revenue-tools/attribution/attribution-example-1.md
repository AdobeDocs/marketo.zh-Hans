---
unique-page-id: 7514126
description: 归因示例1 - Marketo文档 — 产品文档
title: 归因示例1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 归因示例1 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11 |弗雷德被（商展）收购
* 4月15日 | Margo出席（网络研讨会） — 成功
* 4月22日 | Fred与机会关联（角色）
* 4月22日 | Opportunity创建费用为$3,000

| 项目名称 | （商展） | （网络研讨会） |
|---|---|---|
| (FT)已创建权限 | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT)管道已创建 | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT)韩冠廷 | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT)已获得的收入 | `<pre>0</pre>` | `<pre>0</pre>` |

**显示答案**

>[!NOTE]
>
>**说明**
>
>首先要了解的是，某些类型是COUNTS，而其他类型是CURRENCY。 创建的选项是一个计数，一个整数。 Pipeline是一种货币。 在Marketo中，货币将符合您的管理员区域设置。
>
>商展获得全部点数的原因是Margo未与机会中的角色相关联。 没有角色，没有功劳。

>[!NOTE]
>
>**归因规则**
>
>1. 点数平均拆分
>1. 你不能给予比你挣得更多的信用
>1. 你不能为过去发生的事而沾沾自喜

尝试所有示例，您将会成为归因专家！

>[!MORELIKETHIS]
>
>* [归因示例2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [归因示例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [归因示例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

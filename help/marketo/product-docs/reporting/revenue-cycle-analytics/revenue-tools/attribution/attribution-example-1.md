---
unique-page-id: 7514126
description: 归因示例1 - Marketo Docs — 产品文档
title: 归因示例1
translation-type: tm+mt
source-git-commit: fa4ab03b98ac922e10c6daf3647dc460c12244d3
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---


# 归因示例1 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日 | Fred被（贸易展）收购
* 4月15日 |参加研讨会（网络研讨会） — 成功
* 4月22日 | Fred与业务机会关联（角色）
* 4月22日 |为3,000美元创建了业务机会

| 项目名称 | （贸易展） | （网络研讨会） |
|---|---|---|
| (FT)已创建 | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT)管线已创建 | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT)奥普蒂·元 | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT)收入赢 | `<pre>0</pre>` | `<pre>0</pre>` |

**显示答案**

>[!NOTE]
>
>**解释**
>
>首先，要了解某些类型是COUNTS，而其他类型是CURRENCY。 创建的选项是一个计数，一个整数。 管道是一种货币。 在Marketo中，货币将符合您的管理员区域设置设置。
>
>Tradeshow获得所有信用的原因是，Margo没有与机会中的角色关联。 没有角色，没有信用。

>[!NOTE]
>
>**归因规则**
>
>1. 信用被平均分配
>1. 你不能比你挣的更多
>1. 你不能因为过去发生的事而自责


请试用所有示例，您将成为归因专家！

>[!MORELIKETHIS]
>
>* [归因示例2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [归因示例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [归因示例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)


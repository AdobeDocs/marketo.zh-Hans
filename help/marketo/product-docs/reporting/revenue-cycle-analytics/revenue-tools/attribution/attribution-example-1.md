---
unique-page-id: 7514126
description: 归因示例1 - Marketo文档 — 产品文档
title: 归因示例1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 归因示例1 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日 | Fred由（贸易展）收购
* 4月15日 | Margo出席（网络研讨会） — 成功
* 4月22日 | Fred与业务机会相关联（角色）
* 4月22日 |为3,000美元创建了Opportunity

| 项目名称 | （贸易展） | （网络研讨会） |
|---|---|---|
| (FT)已创建选件 | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT)管道已创建 | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT)奥普蒂元 | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT)收入赢得 | `<pre>0</pre>` | `<pre>0</pre>` |

**显示答案**

>[!NOTE]
>
>**说明**
>
>首先，要了解某些类型是COUNTS，其他类型是CURRENCY。 “已创建的选项”是一个计数，一个整数。 管道是一种货币。 在Marketo中，货币将符合您的管理员区域设置设置。
>
>Tradeshow收到所有点数的原因是Margo没有与机会中的角色关联。 没有角色，没有信用。

>[!NOTE]
>
>**归因规则**
>
>1. 信用被平均拆分
>1. 你的信用不能比你挣的多
>1. 你不能为过去发生的事而点名


请尝试所有示例，您将成为归因专家！

>[!MORELIKETHIS]
>
>* [归因示例2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [归因示例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [归因示例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)


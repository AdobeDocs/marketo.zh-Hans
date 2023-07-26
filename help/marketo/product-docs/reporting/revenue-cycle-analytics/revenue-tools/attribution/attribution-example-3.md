---
unique-page-id: 7514149
description: 归因示例3 - Marketo文档 — 产品文档
title: 归因示例3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# 归因示例3 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11 | Steve下载（内容） — 成功
* 4月22日 | Opportunity创建费用为3,000美元（Steve和Jason都有角色）
* 4月25日 | Jason出席（网络研讨会） — 成功
* 4月30日 |商机非赢即败

| 归因量度 | (内容) | （网络研讨会） |
|---|---|---|
| (MT)已创建权限 | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT)管道已创建 | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT)韩元(Opty) | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)已获得的收入 | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**显示答案**

>[!NOTE]
>
>**说明**
>
>记住归因规则#3。 Jason在创建选件后获得了项目成功。 因此，网络研讨会不能因为机会的创造而获得点数。 只有奥提赢了。
>
>因此，(Content)对于商机的创建和管道拥有100%的点数，但对于赢得的商机只有50%的点数。

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
>* [归因示例1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [归因示例2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [归因示例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

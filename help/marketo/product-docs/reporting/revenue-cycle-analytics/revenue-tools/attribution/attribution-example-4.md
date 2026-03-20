---
unique-page-id: 7514151
description: 了解Marketo Engage中的归因示例4，包括归因示例4归因示例。 使用本指南完成您的下一步。
title: 归因举例 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 3%

---

# 归因举例 4 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日|米歇尔下载电子书（内容） — 成功
* 4月15日| John出席（网络研讨会） — 成功
* 4月22日| (Opportunity 1)创建价为$3,000
* 4月24日| (Opportunity 2)创建价5,000 USD
* 4月25日| John和Michelle与&#x200B;**两个**&#x200B;选项相关联
* 4月29日| [Opty 1]未结

| 项目名称 | （内容） | （网络研讨会） |
|---|---|---|
|   | （商机1） | （商机2） | （商机1） | （商机2） |
| (MT)已创建权限 | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)管道已创建 | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT)韩元(Opty) | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT)已获得的收入 | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**显示答案**

>[!NOTE]
>
>**解释**
>
>如果您有多个机会和多个人员且计划取得成功，则必须在人员和计划之间平分点数。 但是，请注意，机会1和2的点数未合并。 每个报表均属于不同的信用评估。
>
>如果涉及很多人，Marketo会自动计算将功劳给予的机会的比例。

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
>* [归因示例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)

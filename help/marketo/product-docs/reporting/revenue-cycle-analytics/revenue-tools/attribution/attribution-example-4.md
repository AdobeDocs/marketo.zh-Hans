---
unique-page-id: 7514151
description: 归因示例4 - Marketo文档 — 产品文档
title: 归因示例4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# 归因示例4 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日 |米歇尔下载电子书（内容） — 成功
* 4月15日 | John出席（网络研讨会） — 成功
* 4月22日 |（机会1）创建成本为3,000美元
* 4月24日 |（机会2）创建成本为5,000美元
* 4月25日 |约翰和米歇尔是个 **两者** 选项
* 4月29日 | [商机1] 为已关闭 — 已关闭

| 项目名称 | (内容) | （网络研讨会） |
|---|---|---|
|   | （商机1） | （商机2） | （商机1） | （商机2） |
| (MT)已创建的权限 | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)管道已创建 | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT)韩圜 | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT)已获得的收入 | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**显示答案**

>[!NOTE]
>
>**说明**
>
>如果您有多个机会和多个成功实施项目的人员，则必须在人员和项目之间平分点数。 但是，请注意，机会1和2的点数未合并。 每一项都是独特的信用评估。
>
>如果涉及很多人，Marketo会自动计算应给予点数的机会分数。

>[!NOTE]
>
>**归因规则**
>
>1. 点数平均拆分
>1. 你不能给予比你所得更多的评价
>1. 你不能把过去发生的事情归功于自己

尝试所有示例，您将成为归因专家！

>[!MORELIKETHIS]
>
>* [归因示例1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [归因示例2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [归因示例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)

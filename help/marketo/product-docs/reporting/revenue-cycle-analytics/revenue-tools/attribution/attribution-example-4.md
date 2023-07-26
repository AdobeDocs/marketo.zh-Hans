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

* 4月11 |米歇尔下载电子书（内容） — 成功
* 4月15日 | John attends（网络研讨会） — 成功
* 4月22日 | （机会1）创建成本为3,000美元
* 4月24日 | （机会2）创建成本为5,000美元
* 4月25日 |约翰和米歇尔关联到 **两者** 选项
* 4月29日 | [商机1] 是非公开赢家

| 项目名称 | (内容) | （网络研讨会） |
|---|---|---|
|   | （商机1） | （商机2） | （商机1） | （商机2） |
| (MT)已创建权限 | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)管道已创建 | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT)韩元(Opty) | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT)已获得的收入 | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**显示答案**

>[!NOTE]
>
>**说明**
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

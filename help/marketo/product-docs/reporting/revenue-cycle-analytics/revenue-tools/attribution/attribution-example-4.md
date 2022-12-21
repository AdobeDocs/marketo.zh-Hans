---
unique-page-id: 7514151
description: 归因示例4 - Marketo文档 — 产品文档
title: 归因示例4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# 归因示例4 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日 | Michelle下载电子书（内容） — 成功
* 4月15日 | John出席（网络研讨会） — 成功
* 4月22日 |（机会1）为3,000美元创建
* 4月24日 |（机会2）为$5,000创建
* 4月25日 | John和Michelle与 **both** 奥普蒂
* 4月29日 | [第1项] 是闭原

| 项目名称 | (内容) | （网络研讨会） |
|---|---|---|
|  | （第1项） | （第2项） | （第1项） | （第2项） |
| (MT)已创建选件 | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)管道已创建 | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT)Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT)赢得的收入 | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**显示答案**

>[!NOTE]
>
>**说明**
>
>当您拥有多个机会和多个获得项目成功的人员时，您必须在人员和项目之间分配点数。 但是，请注意，机会1和机会2的点数不会合并。 每个评级都是一个不同的信用评估。
>
>当涉及许多人时，Marketo会自动计算机会的分数，以给予点数。

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
>* [归因示例1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [归因示例2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [归因示例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)


---
unique-page-id: 7514151
description: 归因示例4 - Marketo Docs — 产品文档
title: 归因示例4
translation-type: tm+mt
source-git-commit: fa4ab03b98ac922e10c6daf3647dc460c12244d3
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# 归因示例4 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日 | Michelle下载电子书（内容） — 成功
* 4月15日 | John参加（网络研讨会） — 成功
* 4月22日 |(Opportunity 1)为$3,000创建
* 4月24日 |(Opportunity 2)，创建价为5,000美元
* 4月25日 | John和Michelle与&#x200B;**两个** Optys关联
* 4月29日 | [ Opty 1]为Closed-Won

| 项目名称 | （内容） | （网络研讨会） |
|---|---|---|
|  | （第1项） | （第2名） | （第1项） | （第2名） |
| (MT)已创建 | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)已创建管道 | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT)奥佩蒂 | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT)收入赢 | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**显示答案**

>[!NOTE]
>
>**解释**
>
>当您拥有多个机会和多个成功项目的人时，您必须将信用分给人和项目。 但是，请注意，机会1和2的信用不会合并。 每项评估都是一个独特的信用评估。
>
>当许多人参与其中时，Marketo将自动计算给予信用的机会的分数。

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
>* [归因示例1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [归因示例2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [归因示例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)


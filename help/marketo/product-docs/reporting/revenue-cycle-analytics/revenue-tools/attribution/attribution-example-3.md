---
unique-page-id: 7514149
description: 归因示例3 - Marketo文档 — 产品文档
title: 归因示例3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# 归因示例3 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日 | Steve下载（内容） — 成功
* 4月22日 |为3,000美元创建了Opportunity（Steve和Jason都有角色）
* 4月25日 | Jason出席（网络研讨会） — 成功
* 4月30日 |机会是闭门的

| 归因量度 | (内容) | （网络研讨会） |
|---|---|---|
| (MT)已创建选件 | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT)管道已创建 | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT)Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)赢得的收入 | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**显示答案**

>[!NOTE]
>
>**说明**
>
>请记住归因规则#3。 产品创建后，Jason获得了项目成功。 因此，网络研讨会无法因创建商机而获得点数。 只有奥普蒂赢了。
>
>因此，（内容）对于创建和管道的选项具有100%的点数，但对于赢得的选项仅具有50%的点数。

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
>* [归因示例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)


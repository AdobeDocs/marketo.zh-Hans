---
unique-page-id: 7514149
description: 归因示例3 - Marketo Docs — 产品文档
title: 归因示例3
translation-type: tm+mt
source-git-commit: fa4ab03b98ac922e10c6daf3647dc460c12244d3
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---


# 归因示例3 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日 | Steve下载（内容） — 成功
* 4月22日 | Opportunity是为3,000美元（Steve和Jason都有角色）而创建的
* 4月25日 | Jason出席（网络研讨会） — 成功
* 4月30日 |机会是闭门的

| 归因量度 | （内容） | （网络研讨会） |
|---|---|---|
| (MT)已创建 | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT)已创建管道 | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT)奥佩蒂 | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)收入赢 | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**显示答案**

>[!NOTE]
>
>**解释**
>
>记住归因规则#3。 Jason在创建项目后取得了成功。 因此，网络研讨会无法因创建此机会而获得肯定。 只有奥普蒂赢了。
>
>因此，（内容）对于创建和管道的功能有100%的信用，但对于获得的功能只有50%的信用。

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
>* [归因示例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)


---
unique-page-id: 7514146
description: 归因示例2 - Marketo Docs — 产品文档
title: 归因示例2
translation-type: tm+mt
source-git-commit: fa4ab03b98ac922e10c6daf3647dc460c12244d3
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---


# 归因示例2 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日 | Bill is acquired by(Tradeshow)
* 4月15日 | Joan是由（网络研讨会）
* 4月22日 |(Opportunity 1)，创建价为6,000美元
* 4月24日 |(Opportunity 2)为10,000美元创建
* 4月25日 | Bill和Joan与&#x200B;**BOTH** Optys的角色关联
* 4月29日 |（机会1）为闭门原因

| 项目名称 | （贸易展） | （网络研讨会） |
|---|---|---|
| (FT)已创建 | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT)管线已创建 | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT)奥普蒂·元 | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT)收入赢 | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**显示答案**

>[!NOTE]
>
>**解释**
>
>由于Bill和Joan都与&#x200B;**BOTH**&#x200B;机会的角色关联，因此系统（根据规则）将信用平均地分配给它们。
>
>为每个项目创建的管道（8 000美元）是可以作为信贷提供的总管道（16 000美元）的一半。

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
>* [归因示例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [归因示例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)


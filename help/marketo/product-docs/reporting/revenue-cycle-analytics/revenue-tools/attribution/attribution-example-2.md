---
unique-page-id: 7514146
description: 了解Marketo Engage中的归因示例2，包括归因示例2归因示例。 使用本指南完成您的下一步。
title: 归因举例 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 4%

---

# 归因举例 2 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日| Bill被（贸易展）收购
* 4月15日| Joan被收购（网络研讨会）
* 4月22日| （机会1）创建价6,000美元
* 4月24日| （机会2）创建价$10,000
* 4月25日| Bill和Joan与&#x200B;**BOTH**&#x200B;选件的角色相关联
* 4月29日| （机会1）不胜枚举

| 项目名称 | （商展） | （网络研讨会） |
|---|---|---|
| (FT)已创建权限 | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT)管道已创建 | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT)韩冠廷 | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT)已获得的收入 | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**显示答案**

>[!NOTE]
>
>**解释**
>
>由于Bill和Joan都与&#x200B;**BOTH**&#x200B;机会中的角色相关联，因此系统（根据规则）将信用平均分配到他们之间。
>
>为每个项目创建的管道（8,000美元）是可用于贷记的总额（16,000美元）的一半。

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
>* [归因示例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [归因示例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

---
unique-page-id: 7514146
description: 归因示例2 - Marketo Docs —— 产品文档
title: 归因示例2
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# 归因示例2 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日 | Bill is appered by(Tradeshow)
* 4月15日 | Joan是由（网络研讨会）
* 4月22日 |(Opportunity 1)创建价格为6,000美元
* 4月24日 |(Opportunity 2)创建价格为10,000美元
* 4月25日 | Bill和Joan与**BOTH **Optys的角色关联
* 4月29日 |（机会1）是闭门的

| 项目名称 | （贸易展） | （网络研讨会） |
|---|---|---|
| (FT)创建的选项 | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT)管道创建 | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT)奥普蒂原 | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT)赢得收入 | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**显示答案**

>[!NOTE]
>
>**说明**
>
>由于Bill和Joan都与**BOTH **机会的角色相关联，因此系统（根据规则）将信用平均分配给他们。
>
>为每个项目创建的管道（8 000美元）是可以作为信贷提供的总管道（16 000美元）的一半。

>[!NOTE]
>
>**归因规则**
>
>1. 信用被平均分配
>1. 你不能给你比挣得多的学分
>1. 你不能因为过去发生的事而自责

>



<br> 

尝试所有示例，您将成为归因专家！

>[!NOTE]
>
>**相关文章**
>
>* [归因示例1](attribution-example-1.md)
>* [归因示例3](attribution-example-3.md)
>* [归因示例4](attribution-example-4.md)


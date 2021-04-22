---
unique-page-id: 557312
description: 智能列表过滤器操作员词汇表 — Marketo Docs — 产品文档
title: 智能列表过滤器运算符词汇表
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 智能列表过滤器运算符术语表{#smart-list-filter-operators-glossary}

运算符是智能列表的一部分，可帮助您实现特定。 它允许您用直接的语言描述过滤器或触发器。 对于每种类型的字段，可用的运算符都不同。

这里有一个词汇表，描述每组运算符。

## 日期字段{#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

选择运算符时，右侧将动态更改。

| 运算符 | 右侧 | 说明 |
|---|---|---|
| is | 单日期 | 确切日期匹配 |
| 不是 | 单日期 | 任何日期（指定的日期除外） |
| 之间 | 两个日期字段 | 包括两个指定日期和两个指定日期之间的任何日期 |
| 过去 | 自然语言输入* | 参见下图 |
| 以前 | 自然语言输入* | 参见下图 |
| 未来 | 自然语言输入* | 参见下图 |
| 以后 | 自然语言输入* | 参见下图 |
| 在时间帧中 | 预设（上一季度、昨天等） | 在选择列表中定义 |
| after | 单日期 | 指定日期后的所有记录 |
| 之前 | 单日期 | 指定记录之前的所有记录 |
| on或after | 单日期 | 与&quot;after&quot;相同，但包含 |
| 在或之前 | 单日期 | 与“之前”相同，但包含 |
| 为空 | 无 | 没有日期的所有记录 |
| 不为空 | 无 | 具有任何日期的所有记录 |

*自然语言输入很酷。 以下是您可以输入的一些模式：

* 1小时
* 82天
* 3周
* 14个月
* 1年

只需把号码和单位一起输入，就行了！

>[!NOTE]
>
>“在过去”**does**&#x200B;包含您创建智能列表的日期（直到该日期，而非之后）。

>[!CAUTION]
>
>当您使用日期字段过滤器（例如，出生日期、SFDC创建日期）创建智能列表并在&#x200B;**约束上或之前使用**&#x200B;之前的&#x200B;**或**&#x200B;时，智能列表还将包括在该日期字段中没有值的人员。

请使用下图了解日期运算符之间的差异。

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**示例**
>
>当您处理过去和将来的事件时，日期字段可能会变得棘手。 以下是几个例子。
>
>**以前**
>
>对于您的新促销活动，请使用此操作员仅向一年内未订阅或续订您服务或从未订阅的用户发送电子邮件。
>
>**以后**
>
>如果您希望查看90天后即将续订的客户。 您将使用两个不同的过滤器。 首先使用“In Future After 90 days”，然后使用“In Future 91 Days”。 那就能捕捉到90天后有约的人。

## 字符串字段{#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| 运算符 | 说明 |
|---|---|
| is | 精确匹配（不区分大小写） |
| 不是 | 除精确匹配外的任何内容 |
| 开始 | 字符串匹配的前字母 |
| 不是开始 | 字符串的前字母不匹配 |
| 包含 | 字符串匹配中的所有字母(示例：加利福尼亚，福特，为此 |
| 不包含 | 字符串中没有字母匹配。 （“contains”的反向） |
| 为空 | 没有值的记录(NULL) |
| 不为空 | 具有任意值的记录 |

>[!TIP]
>
>使用正比使用负运算符。 “不是”过滤器必须搜索实例中的整个数据集，这可能非常耗时。 积极的“是”过滤器可以利用更有效的搜索算法。

## 整数字段{#integer-fields}

![](assets/image2014-9-10-17-3a16-3a14.png)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">运算符</th> 
   <th colspan="1" rowspan="1">说明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1">is</td> 
   <td colspan="1" rowspan="1">精确数字匹配（= 0将返回两个具有0 <em>和</em> NULL的潜在客户）</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">不是</td> 
   <td colspan="1" rowspan="1">除了精确数字匹配之外的任何内容</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">之间</td> 
   <td colspan="1" rowspan="1">定义两个值，以查找介于（包括）</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">大于</td> 
   <td colspan="1" rowspan="1">高于指定</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">小于</td> 
   <td colspan="1" rowspan="1">小于指定</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">至少</td> 
   <td colspan="1" rowspan="1">高于指定（含）</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">最多</td> 
   <td colspan="1" rowspan="1">小于指定（包含）</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">为空</td> 
   <td colspan="1" rowspan="1">没有值(NULL) — 零的记录是一个数字，它是<em>不</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">不为空</td> 
   <td colspan="1" rowspan="1">具有ANY值的记录（包括零）</td> 
  </tr> 
 </tbody> 
</table>

如您所见，这些运营商使Marketo语的流利性更加简单！

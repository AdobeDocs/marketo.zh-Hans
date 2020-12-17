---
unique-page-id: 557312
description: 智能列表过滤器操作符术语表- Marketo文档——产品文档
title: 智能列表过滤器操作符术语表
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---


# 智能列表过滤器操作符术语表{#smart-list-filter-operators-glossary}

运算符是[智能列表](http://docs.marketo.com/display/docs/smart+lists+and+static+lists)的一部分，可帮助您获得特定。 它允许您用直接的语言描述过滤器或触发器。 可用运算符对于每种类型的字段都不同。\
下面是一个词汇表，描述每组运算符。

## 日期字段{#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

选择运算符时，右侧将动态更改。

| 运算符 | 右侧 | 说明 |
|---|---|---|
| is | 单日期 | 确切日期匹配 |
| 不是 | 单日期 | 任何日期（指定的日期除外） |
| 介于 | 两个日期字段 | 包括两个指定日期和两个指定日期之间的任何日期 |
| 过去 | 自然语言输入* | 请参阅下图 |
| 以前 | 自然语言输入* | 请参阅下图 |
| 未来 | 自然语言输入* | 请参阅下图 |
| 以后 | 自然语言输入* | 请参阅下图 |
| 在时间帧中 | 预设（上一季度、昨天等） | 在选择列表中定义 |
| 之后 | 单日期 | 指定日期后的所有记录 |
| 之前 | 单日期 | 指定记录之前的所有记录 |
| 在或之后 | 单日期 | 与“之后”相同，但包含 |
| 在或之前 | 单日期 | 与“之前”相同，但包括 |
| 空 | 无 | 所有没有日期的记录 |
| 不为空 | 无 | 具有任何日期的所有记录 |

*自然语言输入很酷。 以下是您可以输入的一些模式：

* 1小时
* 82天
* 3周
* 14个月
* 1年

只要把号码和单位一起输入，就行了！

>[!NOTE]
>
>在过去&#x200B;**中，**&#x200B;包含您创建智能列表的日期（直到时间，而非之后）。

>[!CAUTION]
>
>当您使用日期字段过滤器（如出生日期、SFDC创建日期）创建智能列表并在约束&#x200B;**或**&#x200B;之前使用&#x200B;**，智能列表还将包括那些在该日期字段中没有值的人员。**

请使用下图了解日期运算符之间的差异。

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**示例**
>
>在您处理过去和将来的事件时，日期字段可能变得棘手。 下面是几个例子。
>
>**以前**
>
>对于您的新促销，使用此操作员仅向未订阅或在一年内续订您的服务或从未订阅过的用户发送电子邮件。
>
>**以后**
>
>如果您希望查看90天后即将续订的客户。 您需要使用两个单独的过滤器。 首先使用“90天后在将来”，然后使用“91天后在将来”。 那会捕捉到90天后有约会的人。

## 字符串字段{#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| 运算符 | 说明 |
|---|---|
| is | 精确匹配（不区分大小写） |
| 不是 | 除精确匹配外的任何内容 |
| 开始 | 字符串匹配的前字母 |
| 不是开始 | 字符串的前字母不匹配 |
| 包含 | 字符串匹配中的任何字母(示例：加利福尼亚，福特，为此 |
| 不包含 | 字符串中没有字母匹配。 （“包含”的倒数） |
| 空 | 没有值的记录(NULL) |
| 不为空 | 具有任意值的记录 |

>[!TIP]
>
>使用正运算符而不是负运算符。 “不是”过滤器必须搜索实例中的整个数据集，这可能非常耗时。 积极的“is”过滤器可以利用更有效的搜索算法。

## 整数字段{#integer-fields}

![](assets/image2014-9-10-17-3a16-3a14.png)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">运算符</th> 
   <th colspan="1" rowspan="1"><p>说明</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1">is</td> 
   <td colspan="1" rowspan="1">精确数字匹配（= 0将返回两个具有0 <em>和</em> NULL的潜在客户）</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">不是</td> 
   <td colspan="1" rowspan="1">除数字精确匹配外的任何内容</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">介于</td> 
   <td colspan="1" rowspan="1">定义两个值，以找到介于（包括）</td> 
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
   <td colspan="1" rowspan="1">小于指定（含）</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">空</td> 
   <td colspan="1" rowspan="1">无值(NULL)-零是数字，<em>不</em>为NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">不为空</td> 
   <td colspan="1" rowspan="1">具有ANY值的记录（包括零）</td> 
  </tr> 
 </tbody> 
</table>

正如您所看到的，这些运营商使用流畅的Marketo语言变得很容易！

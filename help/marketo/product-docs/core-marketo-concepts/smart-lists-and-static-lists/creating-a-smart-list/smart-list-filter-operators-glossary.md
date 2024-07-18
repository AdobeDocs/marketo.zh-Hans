---
unique-page-id: 557312
description: 智能列表筛选器运算符术语表 — Marketo文档 — 产品文档
title: 智能列表筛选器运算符术语表
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 11%

---

# 智能列表筛选器运算符术语表 {#smart-list-filter-operators-glossary}

运算符是智能列表的一部分，可帮助您获取特定内容。 它可让您以直截了当的语言描述过滤器或触发器。 每种类型的字段的可用运算符各不相同。

以下是一组术语表，用于描述每组运算符。

## 日期字段 {#date-fields}

![](assets/smart-list-filter-operators-glossary-1.png)

当您选择运算符时，右侧将动态更改。

<table><thead>
  <tr>
    <th>操作员</th>
    <th>右侧</th>
    <th>描述</th>
  </tr></thead>
<tbody>
  <tr>
    <td>是</td>
    <td>单个日期</td>
    <td>完全匹配的日期</td>
  </tr>
  <tr>
    <td>不是</td>
    <td>单个日期</td>
    <td>除指定日期之外的任何日期</td>
  </tr>
  <tr>
    <td>介于两者之间</td>
    <td>两个日期字段</td>
    <td>包含两个指定日期且介于这两个指定日期之间的任何日期</td>
  </tr>
  <tr>
    <td>在过去</td>
    <td>自然语言输入*</td>
    <td>请参阅下图</td>
  </tr>
  <tr>
    <td>在过去的时间之前</td>
    <td>自然语言输入*</td>
    <td>请参阅下图</td>
  </tr>
  <tr>
    <td>在未来</td>
    <td>自然语言输入*</td>
    <td>请参阅下图</td>
  </tr>
  <tr>
    <td>在未来时间之后</td>
    <td>自然语言输入*</td>
    <td>请参阅下图</td>
  </tr>
  <tr>
    <td>在时间范围内</td>
    <td>预设（上一季度、昨天等）</td>
    <td>在选取列表中定义</td>
  </tr>
  <tr>
    <td>晚于</td>
    <td>单个日期</td>
    <td>指定日期之后的所有记录</td>
  </tr>
  <tr>
    <td>早于</td>
    <td>单个日期</td>
    <td>指定记录之前的所有记录</td>
  </tr>
  <tr>
    <td>在或晚于</td>
    <td>单个日期</td>
    <td>与“after”相同，但包含</td>
  </tr>
  <tr>
    <td>在或早于</td>
    <td>单个日期</td>
    <td>与“之前”相同，但相互包含</td>
  </tr>
  <tr>
    <td>为空</td>
    <td>无</td>
    <td>所有没有日期的记录</td>
  </tr>
  <tr>
    <td>不为空</td>
    <td>无</td>
    <td>包含任何日期的所有记录</td>
  </tr>
</tbody></table>

**&#42;**&#x200B;自然语言输入很酷。 以下是您可以输入的一些模式：

* 1小时
* 82天
* 3周
* 14个月
* 1年

只要输入数字和单位就行了！

>[!NOTE]
>
>“在过去”_是_&#x200B;包含您创建智能列表的日期（直到该时间，而不是之后）。

>[!CAUTION]
>
>当您使用日期字段过滤器（例如，出生日期、SFDC创建日期）创建智能列表并使用约束&#x200B;**[!UICONTROL 在]**&#x200B;之前、**[!UICONTROL 在]**&#x200B;之前或之前，或者&#x200B;**[!UICONTROL 在]**&#x200B;之前时，智能列表还将包含该日期字段中无值的人员。

请使用下图了解日期运算符之间的差异。

![](assets/smart-list-filter-operators-glossary-2.png)

>[!NOTE]
>
>**示例**
>
>当您处理过去和未来的事件时，日期字段可能会比较棘手。 下面是一些示例。
>
>**[!UICONTROL 过去早于]**
>
>对于新的促销活动，使用此运算符仅向一年内未订阅或续订您的服务或者从未订阅过的人发送电子邮件。
>
>**[!UICONTROL 未来在]**&#x200B;之后
>
>假设您希望查看在90天内需要续订的客户。 您将使用两个单独的过滤器。 首先使用“未来90天之后”，然后使用“未来91天”。 这样可以捕获从现在起还有90天时间的任何人。

## 字符串字段 {#string-fields}

![](assets/smart-list-filter-operators-glossary-3.png)

<table><thead>
  <tr>
    <th>操作员</th>
    <th>描述</th>
  </tr></thead>
<tbody>
  <tr>
    <td>是</td>
    <td>完全匹配（不区分大小写）</td>
  </tr>
  <tr>
    <td>不是</td>
    <td>除完全匹配项之外的任何内容</td>
  </tr>
  <tr>
    <td>开头为</td>
    <td>字符串匹配的前几个字母</td>
  </tr>
  <tr>
    <td>开头不是</td>
    <td>字符串的第一个字母不匹配</td>
  </tr>
  <tr>
    <td>包含</td>
    <td>字符串中的任何字母匹配（例如：california、fortune、them）</td>
  </tr>
  <tr>
    <td>不包含</td>
    <td>字符串中没有匹配的字母。 （“包含”的反向）</td>
  </tr>
  <tr>
    <td>为空</td>
    <td>没有值(NULL)的记录</td>
  </tr>
  <tr>
    <td>不为空</td>
    <td>具有任意值的记录</td>
  </tr>
</tbody>
</table>

>[!TIP]
>
>使用正运算符与负运算符。 “不是”过滤器必须搜索实例中的整个数据集，这可能非常耗时。 积极的“is”过滤器可以利用更有效的搜索算法。

## 整数字段 {#integer-fields}

![](assets/smart-list-filter-operators-glossary-4.png)

<table><thead>
  <tr>
    <th>操作员</th>
    <th>描述</th>
  </tr></thead>
<tbody>
  <tr>
    <td>是</td>
    <td>完全数字匹配（ = 0将返回具有0和NULL的两个潜在客户）</td>
  </tr>
  <tr>
    <td>不是</td>
    <td>除精确数字匹配之外的任何内容</td>
  </tr>
  <tr>
    <td>介于两者之间</td>
    <td>定义两个值以查找介于两者之间的所有人（包括）</td>
  </tr>
  <tr>
    <td>大于</td>
    <td>高于指定的</td>
  </tr>
  <tr>
    <td>小于</td>
    <td>小于指定的</td>
  </tr>
  <tr>
    <td>至少</td>
    <td>高于指定的（包括）</td>
  </tr>
  <tr>
    <td>最多</td>
    <td>小于指定的（包括）</td>
  </tr>
  <tr>
    <td>为空</td>
    <td>没有值(NULL)的记录 — 零是一个数字，它不是NULL</td>
  </tr>
  <tr>
    <td>不为空</td>
    <td>具有ANY值（包括零）的记录</td>
  </tr>
</tbody>
</table>

如您所见，这些操作员可以轻松地说流利的Marketo语！

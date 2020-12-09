---
unique-page-id: 7514151
description: 归因示例4 - Marketo Docs —— 产品文档
title: 归因示例4
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# 归因示例4 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日 | Michelle下载电子书（内容）-成功
* 4月15日 | John参加（网络研讨会）-成功
* 4月22日 |(Opportunity 1)创建价格为3,000美元
* 4月24日 |(Opportunity 2)创建价格为5,000美元
* 4月25日 | John和Michelle都与Optys **相关**
* 4月29日 | [Opty] 1是闭门币

| 项目名称 | （内容） | （网络研讨会） |
|---|---|---|
|  | （第1项） | （选项2） | （第1项） | （选项2） |
| (MT)已创建选项 | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)管道已创建 | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT)Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT)赢得收入 | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**显示答案**

>[!NOTE]
>
>**说明**
>
>当您拥有多个机会和多个成功项目的人时，您必须将信用分给人和项目。 但是，请注意，机会1和机会2的信用未合并。 每项评估都是独特的信用评估。
>
>当涉及到很多人时，Marketo将自动计算给予信用的机会的分数。

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

>[!MORELIKETHIS]
>
>* [归因示例1](attribution-example-1.md)
>* [归因示例2](attribution-example-2.md)
>* [归因示例3](attribution-example-3.md)


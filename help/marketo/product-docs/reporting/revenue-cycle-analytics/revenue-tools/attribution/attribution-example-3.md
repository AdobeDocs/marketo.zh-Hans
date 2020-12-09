---
unique-page-id: 7514149
description: 归因示例3 - Marketo Docs —— 产品文档
title: 归因示例3
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---


# 归因示例3 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日 | Steve下载（内容）-成功
* 4月22日 | Opportunity的创建价格为3,000美元（Steve和Jason都有角色）
* 4月25日 | Jason参加（网络研讨会）-成功
* 4月30日 |机会是闭门的

| 归因指标 | （内容） | （网络研讨会） |
|---|---|---|
| (MT)已创建选项 | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT)管道已创建 | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT)Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)赢得收入 | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**显示答案**

>[!NOTE]
>
>**说明**
>
>记住归因规则#3。 Jason在项目产生后取得了成功。 因此，网络研讨会不能因创建此机会而得到肯定。 只有奥普蒂赢了。
>
>因此，（内容）对于Opty创建和销售渠道有100%的信用，但对于该Opty赢得的信用只有50%。

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
>* [归因示例4](attribution-example-4.md)


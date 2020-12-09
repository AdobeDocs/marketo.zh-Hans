---
unique-page-id: 7514126
description: 归因示例1 - Marketo Docs —— 产品文档
title: 归因示例1
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---


# 归因示例1 {#attribution-example}

请阅读以下方案，并尝试确定网格中应包含的数字。

* 4月11日 | Fred由（贸易展）收购
* 4月15日 | Margo参加（网络研讨会）-成功
* 4月22日 | Fred与此机会关联（角色）
* 4月22日 |创建的销售机会价格为3,000美元

| 项目名称 | （贸易展） | （网络研讨会） |
|---|---|---|
| (FT)创建的选项 | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT)管道创建 | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT)奥普蒂原 | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT)赢得收入 | `<pre>0</pre>` | `<pre>0</pre>` |

**显示答案**

>[!NOTE]
>
>**说明**
>
>首先，要了解某些类型是COUNTS，而其他类型是CURRENCY。 创建的选项是一个计数，一个整数。 管道是一种货币。 在Marketo中，货币将符合您的管理员区域设置。
>
>Tradeshow获得所有积分的原因是，Margo与机会中的角色无关。 没有角色，没有信用。

>[!NOTE]
>
>**归因规则**
>
>1. 信用被平均分配
>1. 你不能给你比挣得多的学分
>1. 你不能因为过去发生的事而自责


尝试所有示例，您将成为归因专家！

>[!MORELIKETHIS]
>
>* [归因示例2](attribution-example-2.md)
>* [归因示例3](attribution-example-3.md)
>* [归因示例4](attribution-example-4.md)


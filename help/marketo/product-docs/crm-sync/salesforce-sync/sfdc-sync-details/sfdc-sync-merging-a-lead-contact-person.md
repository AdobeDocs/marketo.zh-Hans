---
unique-page-id: 7515133
description: SFDC同步——合并潜在客户／联系人／人员- Marketo文档——产品文档
title: SFDC同步——合并潜在客户／联系人／人员
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# SFDC同步：合并潜在客户／联系人／人员{#sfdc-sync-merging-a-lead-contact-person}

有时最好只是列表规则。 下面介绍：

* 在&#x200B;**Salesforce**&#x200B;中合并两个潜在客户时，正常同步会告知Marketo，并且潜在客户会自动合并为Marketo中的人员。
* 在&#x200B;**Marketo**&#x200B;中合并两个人实际调用的过程与在Salesforce中将他们合并为潜在客户的过程相同。 它仍可自动工作。
* 将&#x200B;**潜在客户（人）合并到联系人**&#x200B;中的方式相同。 最后，双方只有一个联系人。
* 合并时，将对默认得分进行总和。

>[!NOTE]
>
>**示例**
>
>合并3个销售线索（人），每个分数为10，将产生1个销售线索（人），得分为30。

* 冲突字段值从“获胜记录”中获取。 （记录=产生的潜在客户或联系人）
* 如果“失败记录”（即正在消失的记录）有价值，而获胜记录没有价值，我们将保持失败记录。 换句话说，“有些价值胜于没有价值。”
* 所有活动日志项都合并。

>[!NOTE]
>
>**深潜**
>
>深入了解有关[在Marketo](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)中合并人员的更多信息。


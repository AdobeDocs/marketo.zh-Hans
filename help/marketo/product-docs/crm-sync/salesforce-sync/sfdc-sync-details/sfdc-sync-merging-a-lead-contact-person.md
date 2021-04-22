---
unique-page-id: 7515133
description: SFDC同步 — 合并潜在客户/联系人/人员 — Marketo文档 — 产品文档
title: SFDC同步 — 合并潜在客户/联系人/人
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# SFDC同步：合并潜在客户/联系人/人员{#sfdc-sync-merging-a-lead-contact-person}

有时最好只列表规则。 下面介绍：

* 在&#x200B;**Salesforce**&#x200B;中合并两个潜在客户时，正常同步会告知Marketo，这些潜在客户会自动合并为Marketo中的人员。
* 在&#x200B;**Marketo**&#x200B;中合并两个人实际上调用与在Salesforce中作为潜在客户合并它们相同的进程。 它仍然自动工作。
* 将&#x200B;**潜在客户（人员）合并到联系人**&#x200B;中的方式相同。 你最后两边只有一个接触。
* 合并时，将对默认得分进行总和。

>[!NOTE]
>
>合并3个销售线索（人），每个分数为10，将产生1个销售线索（人）的结果，得分为30。

* 冲突字段值取自“入选记录”。 （记录=产生的潜在客户或联系人）
* 如果“失败记录”（即正在消失的记录）有价值，而获胜记录没有价值，我们将保持失败记录。 换句话说， “有些值比没有值好。 ”
* 所有活动日志项都将合并。

>[!NOTE]
>
>有关[合并Marketo中人员的详细信息，请深入了解。](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)

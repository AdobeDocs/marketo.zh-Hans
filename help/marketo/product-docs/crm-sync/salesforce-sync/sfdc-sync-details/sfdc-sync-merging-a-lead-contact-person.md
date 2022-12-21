---
unique-page-id: 7515133
description: SFDC同步 — 合并潜在客户/联系人/人员 — Marketo文档 — 产品文档
title: SFDC同步 — 合并潜在客户/联系人/人员
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# SFDC同步：合并潜在客户/联系人/人员 {#sfdc-sync-merging-a-lead-contact-person}

有时最好只列出规则。 我们开始了：

* 在 **Salesforce**，正常同步会告知Marketo，并且潜在客户会作为Marketo中的人员自动合并。
* 将两个人合并 **Marketo** 实际上会调用与在Salesforce中将它们合并为潜在客户相同的流程。 它仍然自动工作。
* 合并 **潜在（个人）联系人** 工作方式相同。 最后两边只有一个接触。
* 合并时，默认得分会相加。

>[!NOTE]
>
>将3个潜在客户（人员）与每个分数10合并，将产生1个潜在客户（人员）的结果，其分数为30。

* 从“入选记录”中获取冲突的字段值。 （记录=结果潜在客户或联系人）
* 如果“失败记录”（即正在消失的记录）有价值，而获胜记录没有价值，我们将保留失败记录。 换句话说，“某些价值比没有价值好。”
* 所有活动日志项都会合并。

>[!NOTE]
>
>深入了解有关 [合并Marketo人](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).

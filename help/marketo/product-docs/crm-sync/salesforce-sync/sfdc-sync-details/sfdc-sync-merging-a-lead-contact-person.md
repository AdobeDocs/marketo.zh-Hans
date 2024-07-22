---
unique-page-id: 7515133
description: SFDC同步 — 合并潜在客户/联系人/人员 — Marketo文档 — 产品文档
title: SFDC同步 — 合并潜在客户/联系人/人员
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# SFDC同步：合并潜在客户/联系人/人员 {#sfdc-sync-merging-a-lead-contact-person}

有时最好只是列出规则。 接下来是：

* 当您在&#x200B;**Salesforce**&#x200B;中合并两个潜在客户时，普通同步会告知Marketo Engage，并且这些潜在客户会自动作为Marketo中的联系人进行合并。
* 在&#x200B;**Marketo**&#x200B;中合并两个人实际上会调用与在Salesforce中合并他们作为潜在客户相同的流程。 它仍然自动工作。
* 将&#x200B;**潜在客户（人员）合并到联系人**&#x200B;的工作方式相同。 最终两边只有一个接触点。
* 合并时，将汇总默认得分。

>[!NOTE]
>
>如果将3个各自得分为10分的潜在客户（人员）合并，则将得到1个潜在客户（人员）的结果，得分为30。

* 从“入选记录”中获取冲突的字段值。 （记录=产生的潜在客户或联系人）
* 如果“失败记录”（正在消失的记录）有价值，而获胜记录没有价值，我们将保留失败记录。 换句话说，“有价值总比没有价值好。”
* 所有活动日志项都会被合并。

>[!NOTE]
>
>深入了解Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}中有关[合并人员的详细信息。

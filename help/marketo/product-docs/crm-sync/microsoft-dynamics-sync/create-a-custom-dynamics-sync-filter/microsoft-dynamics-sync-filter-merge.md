---
unique-page-id: 10092969
description: Microsoft Dynamics同步筛选器 — 合并 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步筛选器 — 合并
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Microsoft Dynamics同步筛选器：合并 {#microsoft-dynamics-sync-filter-merge}

在Microsoft Dynamics中合并潜在客户时，会使用两种选项类型 — 同步过滤器=是(TRUE)和同步过滤器=否(FALSE)。 合并两个记录时，结果会有所不同，具体取决于哪个记录为True和哪个记录为False。

根据管理员为确定入选者而定义的工作流规则，潜在客户记录会变为true或false。 入选记录的同步过滤器最终决定MS Dynamics记录是否与Marketo同步。

只有当一条记录为真、一条记录为假时，才会变得棘手。

| 如果丢失记录的同步筛选器为： | 并且入选记录的同步过滤器为： | 这是Marketo中的结果 |
|---|---|---|
| 真 | 真 | 入选记录将继续与Marketo同步 |
| 假 | 假 | 获胜记录仍将&#x200B;_非_&#x200B;与Marketo同步 |
| 假 | 真 | 入选记录将与Marketo同步 |
| 真 | 假 | 入选记录将不会与Marketo同步 |

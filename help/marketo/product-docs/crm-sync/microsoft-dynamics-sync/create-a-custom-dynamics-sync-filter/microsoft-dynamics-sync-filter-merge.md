---
unique-page-id: 10092969
description: Microsoft Dynamics同步过滤器 — 合并 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步筛选器 — 合并
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Microsoft Dynamics同步过滤器：合并 {#microsoft-dynamics-sync-filter-merge}

在Microsoft Dynamics中合并潜在客户时，会使用“两个选项”类型 — “同步”筛选器=“是”(TRUE)，“同步”筛选器=“否”(FALSE)。 合并两个记录时，结果会有所不同，具体取决于哪个记录为True和哪个为False。

根据管理员为确定入选者而定义的工作流规则，潜在客户记录将变为true或false。 入选记录的同步筛选器最终决定MS Dynamics记录是否与Marketo同步。

当一条记录是真的，一条是假的时候，它就会变得棘手。

| 如果丢失记录的同步筛选器为： | 且入选记录的同步筛选器为： | 这是在Marketo |
|---|---|---|
| 真 | 真 | 获胜记录将继续与Marketo同步 |
| 假 | 假 | 获胜记录将继续 **not** 与Marketo同步 |
| 假 | 真 | 入选记录将与Marketo同步 |
| 真 | 假 | 入选记录将与Marketo不同步 |

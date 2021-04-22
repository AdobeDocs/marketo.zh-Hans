---
unique-page-id: 10092969
description: Microsoft Dynamics Sync过滤器 — 合并 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步筛选器 — 合并
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Microsoft Dynamics同步筛选器：合并{#microsoft-dynamics-sync-filter-merge}

在Microsoft Dynamics中合并潜在客户时使用“Two Options（两个选项）”类型 — “Sync（同步）”过滤器= “Yes(TRUE)”和“Sync（同步）”过滤器= “No(FALSE)”。 合并两个记录时，结果会有所不同，具体取决于哪个记录为True和哪个为False。

潜在客户记录会根据管理员定义的工作流规则变为true或false以确定入选方。 获胜记录的同步过滤器是最终决定MS Dynamics记录是否与Marketo同步的因素。

当一条记录是真的，一条是假的时候，它变得棘手。

| 如果丢失记录的同步过滤器为： | 而获胜记录的同步筛选器是： | 这是Marketo |
|---|---|---|
| True | True | 获胜记录继续与Marketo同步 |
| False | False | 获胜记录继续&#x200B;**不**&#x200B;与Marketo同步 |
| False | True | 获胜记录将与Marketo同步 |
| True | False | 获胜记录将不与Marketo同步 |

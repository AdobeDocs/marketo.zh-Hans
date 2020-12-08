---
unique-page-id: 10092969
description: Microsoft Dynamics Sync过滤器——合并——营销文档——产品文档
title: Microsoft Dynamics同步筛选器——合并
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Microsoft Dynamics同步筛选器：合并 {#microsoft-dynamics-sync-filter-merge}

在Microsoft Dynamics中合并潜在客户时使用“Two Options（两个选项）”类型——同步筛选器= Yes(TRUE)，同步筛选器= No(FALSE)。 合并两个记录时，结果会有所不同，具体取决于哪个记录为True和哪个为False。

根据管理员定义的工作流规则确定入选方，潜在客户记录将变为真或假。 获胜记录的同步筛选器是最终决定MS Dynamics记录是否与Marketo同步的因素。

当一条记录是真的，一条是假的时候，它变得很棘手。

| 如果丢失记录的同步过滤器为： | 并且获胜记录的同步过滤器为： | 这是Marketo的结果 |
|---|---|---|
| True | True | 获胜记录继续与Marketo同步 |
| False | False | 获胜记录继续与 **Marketo** 不同步 |
| False | True | 获胜记录将与Marketo同步 |
| True | False | 获胜记录将不会与Marketo同步 |


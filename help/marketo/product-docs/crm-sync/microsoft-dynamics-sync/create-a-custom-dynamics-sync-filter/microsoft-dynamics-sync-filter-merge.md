---
unique-page-id: 10092969
description: Microsoft Dynamics同步过滤器 — 合并 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步筛选器 — 合并
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# [!DNL Microsoft] Dynamics同步筛选器：合并 {#microsoft-dynamics-sync-filter-merge}

在[!DNL Microsoft Dynamics]中合并潜在客户使用两种选项类型 — 同步筛选器=是(TRUE)和同步筛选器=否(FALSE)。 合并两个记录时，结果会有所不同，具体取决于哪个记录为True和哪个记录为False。

根据管理员为确定入选者而定义的工作流规则，潜在客户记录会变为true或false。 入选记录的同步过滤器最终确定[!DNL MS Dynamics]记录是否与Marketo同步。

只有当一条记录为真、一条记录为假时，才会变得棘手。

| 如果丢失记录的同步筛选器为： | 并且入选记录的同步过滤器为： | 这是Marketo中的结果 |
|---|---|---|
| [!UICONTROL True] | [!UICONTROL True] | 入选记录将继续与Marketo同步 |
| [!UICONTROL False] | [!UICONTROL False] | 获胜记录仍将&#x200B;**非**&#x200B;与Marketo同步 |
| [!UICONTROL False] | [!UICONTROL True] | 入选记录将与Marketo同步 |
| [!UICONTROL True] | [!UICONTROL False] | 入选记录将不会与Marketo同步 |

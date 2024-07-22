---
unique-page-id: 14352464
description: Salesforce中的报表功能板 — Marketo文档 — 产品文档
title: Salesforce中的报告仪表板
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# Salesforce中的报告仪表板 {#reporting-dashboards-in-salesforce}

了解如何在下方设置仪表板。

## 打开并单击报表 {#open-and-click-report}

1. 选择&#x200B;**任务和事件**&#x200B;记录类型。
1. 根据所需的时间范围和层次结构定义报表参数。
1. 添加过滤器以移除记录到Salesforce的内部电子邮件(例如，公司/帐户不等于Marketo)。
1. 选择&#x200B;**摘要**&#x200B;报告格式。
1. 将“主题”、“已分配”和“Marketo Sales Clicked/Marketo Sales Viewed”字段添加到报表中。
1. 在“字段”窗格中双击&#x200B;**添加公式**。
1. 向公式中添加名称，选择格式中的&#x200B;**百分比**，然后选择&#x200B;**分组1**。
1. 在摘要字段中选择&#x200B;**Marketo Sales Clicked/Marketo Sales Viewed，**&#x200B;和&#x200B;**Sum**。
1. 在公式中添加一个除号，然后在“摘要”字段中选择&#x200B;**记录计数** - _另存为_。

## 模板性能报表 {#template-performance-report}

1. 自定义“打开并单击”报表以包含以下字段 — _另存为_。

## 模板卷报告 {#template-volume-report}

1. 修改模板性能报表，并加入过滤器“Marketo Sales Template not equal to blank”。
1. 删除Marketo Sales点击的字段 — _另存为_。

## 趋势帐户报表 {#trending-accounts-report}

1. 选择具有帐户记录类型的活动。
1. 按如下所示设置报表参数和字段 — _另存为_。

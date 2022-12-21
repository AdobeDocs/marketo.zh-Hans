---
unique-page-id: 14352464
description: Salesforce中的报表功能板 — Marketo文档 — 产品文档
title: Salesforce中的报表功能板
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---

# Salesforce中的报表功能板 {#reporting-dashboards-in-salesforce}

了解如何在下面设置功能板。

## 打开并单击报表 {#open-and-click-report}

1. 选择 **任务和事件** 记录类型。
1. 根据所需的时间范围和层次结构定义报表参数。
1. 添加过滤器以删除记录到Salesforce的内部电子邮件(例如，公司/帐户不等于Marketo)。
1. 选择 **概要** 报表格式。
1. 将“已分配的主体”、“已分配的”和“Marketo销售人员已点击/Marketo销售人员已查看”字段添加到报表中。
1. 双击 **添加公式** 字段窗格中。
1. 在公式中添加名称，选择 **百分比** ，然后选择 **分组1**.
1. 选择 **Marketo已点击销售/Marketo已查看销售，** then **总和** 中。
1. 向公式中添加除号，然后选择 **记录计数** 在“摘要”字段中 —  _另存为_.

## 模板性能报表 {#template-performance-report}

1. 自定义打开并单击报表以包含以下字段 —  _另存为_.

## 模板卷报表 {#template-volume-report}

1. 修改模板性能报表并包含过滤器“Marketo销售模板不等于空白”。
1. 删除“已单击Marketo销售”字段 —  _另存为_.

## 趋势帐户报表 {#trending-accounts-report}

1. 选择“具有帐户的活动”记录类型。
1. 设置报表参数和字段，如下所示 —  _另存为_.

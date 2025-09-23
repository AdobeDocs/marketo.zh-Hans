---
unique-page-id: 14352464
description: Salesforce中的报表功能板 — Marketo文档 — 产品文档
title: Salesforce 中的报告仪表板
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 4%

---

# Salesforce 中的报告仪表板 {#reporting-dashboards-in-salesforce}

了解如何在下方设置仪表板。

## 打开并单击报表 {#open-and-click-report}

1. 选择&#x200B;**[!UICONTROL Tasks and Events]**&#x200B;记录类型。
1. 根据所需的时间范围和层次结构定义报表参数。
1. 添加筛选器以移除记录到[!DNL Salesforce]的内部电子邮件(例如公司/帐户不等于Marketo)。
1. 选择&#x200B;**[!UICONTROL Summary]**&#x200B;报表格式。
1. 将“主题”、“已分配”和“Marketo Sales Clicked/Marketo Sales Viewed”字段添加到报表中。
1. 在“字段”窗格中双击&#x200B;**[!UICONTROL Add Formula]**。
1. 向公式中添加名称，选择格式中的&#x200B;**[!UICONTROL Percent]**，然后选择&#x200B;**[!UICONTROL Grouping 1]**。
1. 在摘要字段中选择&#x200B;**[!UICONTROL Marketo Sales Clicked/Marketo Sales Viewed]**，然后选择&#x200B;**[!UICONTROL Sum]**。
1. 在公式中添加一个除号，然后在“摘要”字段中选择&#x200B;**[!UICONTROL Record Count]**- _另存为_。

## 模板性能报表 {#template-performance-report}

1. 自定义“打开并单击”报表以包含以下字段 — _另存为_。

## 模板卷报告 {#template-volume-report}

1. 修改模板性能报表，并加入过滤器“Marketo Sales Template not equal to blank”。
1. 删除Marketo Sales点击的字段 — _另存为_。

## 趋势帐户报表 {#trending-accounts-report}

1. 选择具有帐户记录类型的活动。
1. 按如下所示设置报表参数和字段 — _另存为_。

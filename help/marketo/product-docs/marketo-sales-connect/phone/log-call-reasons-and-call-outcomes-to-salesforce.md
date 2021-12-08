---
description: 将调用原因和调用结果记录到Salesforce - Marketo文档 — 产品文档
title: 记录调用原因和向Salesforce调用结果
hide: true
hidefromtoc: true
source-git-commit: 1dd4a4f6bfac0b101f85f3776396aeef1a1f7182
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# 记录调用原因和向Salesforce调用结果 {#log-call-reasons-and-call-outcomes-to-salesforce}

如果出于报告或可见性目的要记录调用结果并向Salesforce调用原因，则可以为每个活动创建一个自定义活动字段。 每个字段必须使用特定的API名称。

* 调用结果API名称：mktosales_call_outde
* 调用原因API名称：mktosales_call_reason

要使用这些字段，您首先需要将该字段创建为自定义活动字段。 为了让用户可见，您需要将其添加到任务对象页面布局中。

## 在Salesforce Classic中创建自定义活动字段  {#create-custom-activity-field-in-salesforce-classic}

1. 在Salesforce中，转到“设置”。

PICC

1. 在“快速查找”框中输入“活动”。

PICC

1. 单击 **活动自定义字段**.

PICC

1. 单击 **新建**.

PICC

## 在Salesforce闪电中创建自定义活动字段 {#create-custom-activity-field-in-salesforce-lightning}

1. 在Salesforce中，单击右上方的齿轮图标。

PICC

1. 单击 **设置**.

PICC

1. 单击 **对象管理器**.

PICC

1. 在“快速查找”框中输入活动，然后单击活动标签以打开对象的设置。

PICC

1. 在左侧，单击 **字段和关系**.

PICC

1. 单击 **新建**.

PICC

## 在Salesforce Classic中，将自定义活动字段添加到任务页面布局 {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

步骤

## 在Salesforce闪电中，将自定义活动字段添加到任务页面布局 {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

步骤

>[!MORELIKETHIS]
>
>[在活动历史记录中安装Sales Connect事件字段](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)

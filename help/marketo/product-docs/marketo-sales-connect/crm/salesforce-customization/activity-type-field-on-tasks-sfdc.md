---
unique-page-id: 14352476
description: 活动(SFDC)上的“任务类型”字段- Marketo Docs —— 产品文档
title: 活动上的任务类型字段(SFDC)
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# 活动上的任务类型字段(SFDC) {#activity-type-field-on-tasks-sfdc}

在Sales Connect的帮助下，您可以在Salesforce中将电子邮件和呼叫记录为活动。 在Salesforce中拥有有价值数据的关键部分是让“类型”字段填充正确的值。

>[!NOTE]
>
>通过密送记录电子邮件不会查找任务类型选择列表，而是会自动将类型字段填充为“电子邮件”，因为它们将通过密送地址传送到Salesforce。

## 要求 {#requirements}

* 与Salesforce的连接
* 未在“任务类型”选择列表上选择默认类型值
* 呼叫、回复和电子邮件必须都位于“任务类型”选择列表下（大写事项）
* 否 `Workflows` 或 `Triggers` 对“类型”字段的值执行操作

## 设置 {#setup}

首先检查您是否具有正确的选择列表值。 您需要Salesforce管理员的帮助才能对选择列表进行任何更改。

1. 导航到 [Salesforce.com](http://Salesforce.com) ，然后单击右上角的设置。
1. 单击“自定义”。
1. 单击活动。
1. 单击任务字段。
1. 单击“类型”。
1. 您现在位于任务类型选择列表。 确保未选择“默认”。
1. 确保列出“电子邮件”、“呼叫”和“回复”的“类型”值。

现在，您将开始看到“类型”字段填充已记录电子邮件、呼叫和回复的相应值。 这些值不 **会填充** 在Sales Connect提醒任务中。

>[!NOTE]
>
>如果未将“Reply”视为值，请单击“新建”添加 **它**。 “回复”不是Salesforce中的标准值。

---
unique-page-id: 14352476
description: 任务的活动类型字段(SFDC) - Marketo文档 — 产品文档
title: 任务上的活动类型字段(SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# 任务上的活动类型字段(SFDC) {#activity-type-field-on-tasks-sfdc}

借助Sales Connect ，您可以在Salesforce中将您的电子邮件和呼叫记录为活动。 在Salesforce中有价值的数据的一个关键部分是，让“类型”字段填充正确的值。

>[!NOTE]
>
>通过密件抄送记录电子邮件时，不会查找“任务类型”选取列表，而是会自动将“类型”字段填充为“电子邮件”，因为它们将通过您的密件抄送地址传送到Salesforce。

## 要求 {#requirements}

* 与Salesforce的连接
* 任务类型选择列表中未选择默认类型值
* “呼叫”、“回复”和“电子邮件”必须全部存在于“任务类型”选取列表下（大写问题）
* 没有工作流或触发器对“类型”字段的值执行操作

## 设置 {#setup}

首先检查您是否已设置正确的选取列表值。 您需要Salesforce管理员的帮助才能对选择列表进行任何更改。

1. 导航到[Salesforce.com](https://salesforce.com)，然后单击右上角的“设置”。
1. 单击“自定义”。
1. 单击“活动”。
1. 单击“任务字段”。
1. 单击“类型”。
1. 您现在位于任务类型选择列表。 确保未选择“默认”。
1. 确保为“电子邮件”、“呼叫”和“回复”列出“类型”值。

现在，您已完成，接下来会看到类型字段填充了记录的电子邮件、呼叫和回复的相应值。 Sales Connect提醒任务将&#x200B;_不填充_&#x200B;这些值。

>[!NOTE]
>
>如果您未看到“回复”作为值，请单击&#x200B;**新建**&#x200B;以添加它。 “回复”不是Salesforce中的标准值。

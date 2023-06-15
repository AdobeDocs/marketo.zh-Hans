---
unique-page-id: 14352476
description: 任务中的活动类型字段(SFDC) - Marketo文档 — 产品文档
title: 任务中的活动类型字段(SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
source-git-commit: 46c48172a58cf6bd2e9772ef57510fd7d808adc2
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# 任务中的活动类型字段(SFDC) {#activity-type-field-on-tasks-sfdc}

借助Sales Connect，您可以在Salesforce中将您的电子邮件和呼叫记录为活动。 在Salesforce中有价值的数据的一个关键部分是，让“类型”字段填充正确的值。

>[!NOTE]
>
>通过密件抄送记录电子邮件不会查看“任务类型”选取列表，而是会自动将“类型”字段填充为“电子邮件”，因为它们将通过您的密件抄送地址传送到Salesforce。

## 要求 {#requirements}

* 与Salesforce的连接
* 未在“任务类型”选择列表中选择“默认类型”值
* “呼叫”、“回复”和“电子邮件”必须全部存在于“任务类型”选取列表下（大写问题）
* 没有工作流或触发器对“类型”字段的值执行操作

## 设置 {#setup}

首先检查您是否已设置正确的选取列表值。 您需要Salesforce管理员的帮助才能对选择列表进行任何更改。

1. 导航到 [Salesforce.com](https://salesforce.com) 然后单击右上角的“设置”。
1. 单击“自定义”。
1. 单击“活动”。
1. 单击“任务字段”。
1. 单击“类型”。
1. 您现在位于任务类型选择列表。 确保未选择“默认”。
1. 确保为“电子邮件”、“呼叫”和“回复”列出“类型”值。

现在，设置完此选项后，您将看到类型字段填充了记录的电子邮件、呼叫和回复的相应值。 这些值将 _非_ 在Sales Connect提醒任务中填充。

>[!NOTE]
>
>如果您未看到“回复”作为值，请单击以添加它 **新**. “Reply”不是Salesforce中的标准值。

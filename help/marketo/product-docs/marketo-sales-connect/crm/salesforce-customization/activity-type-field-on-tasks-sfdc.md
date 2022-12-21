---
unique-page-id: 14352476
description: 任务(SFDC)上的活动类型字段 — Marketo文档 — 产品文档
title: 任务(SFDC)上的活动类型字段
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# 任务(SFDC)上的活动类型字段 {#activity-type-field-on-tasks-sfdc}

借助Sales Connect，您可以在Salesforce中将电子邮件和呼叫记录为活动。 在Salesforce中拥有有价值数据的一个关键部分是让Type字段填充正确的值。

>[!NOTE]
>
>通过密件抄送记录电子邮件不会查看任务类型选取列表，而是会自动将类型字段填充为“电子邮件”，因为这些电子邮件将通过密件抄送地址提交到Salesforce。

## 要求 {#requirements}

* 与Salesforce的连接
* 未在“任务类型”选取列表上选择“默认类型”值
* 呼叫、回复和电子邮件必须都位于“任务类型”选取列表下（大小写事项）
* 没有工作流或触发器对类型字段的值执行操作

## 设置 {#setup}

首先检查您是否具有正确的选择列表值。 您需要Salesforce管理员的帮助才能对选择列表进行任何更改。

1. 导航到 [Salesforce.com](https://salesforce.com) ，然后单击右上角的设置。
1. 单击自定义。
1. 单击活动。
1. 单击任务字段。
1. 单击类型。
1. 您现在位于“任务类型选取器”列表。 确保未选择“默认”。
1. 确保列出了“电子邮件”、“呼叫”和“回复”的“类型”值。

现在，您将开始看到“类型”字段，该字段填充已记录电子邮件、调用和回复的相应值。 这些值将 **not** 在Sales Connect提醒任务中填充。

>[!NOTE]
>
>如果未看到“Reply”作为值，请单击 **新建**. “Reply”不是Salesforce中的标准值。

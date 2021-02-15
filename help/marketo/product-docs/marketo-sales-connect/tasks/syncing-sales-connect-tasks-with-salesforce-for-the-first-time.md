---
unique-page-id: 14352541
description: 首次将Sales Connect任务与Salesforce同步 — Marketo Docs — 产品文档
title: 首次将Sales Connect任务与Salesforce同步
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# 首次将Sales Connect任务与Salesforce同步{#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

当您首次打开Sales Connect和Salesforce任务之间的同步时，我们会导入您的Salesforce任务。 我们将&#x200B;**不**&#x200B;推送您在Sales Connect to Salesforce中拥有的任何当前任务。 为了减少混乱和重复，从Sales Connect同步到Salesforce的唯一任务是在&#x200B;*您将Sales Connect与SFDC同步后创建的任务。*

以下是同步Sales Connect和SFDC任务时发生的情况：

- 在任务同步时单击“保存”后，它们会开始同步。 这首先需要一些时间。

- 在过去24小时内更新或创建的任何提醒都将从SFDC导入Sales Connect。 同步基于截止日期，所有这些任务将在后端同步，但在命令中心，您将只看到应于今天和明天的任务。

- 如果之前已打开同步，而您删除了SFDC中的任何任务，则过去15天内已删除的任何内容都将从命令中心删除。

- 只要启用了同步，我们就会在Sales Connect和SFDC之间不断同步任务。

初始同步后，您在Sales Connect中创建、编辑、完成或删除的任何任务都将同步到Salesforce中的任务列表。 而在Salesforce中创建、编辑、完成或删除的任何内容都将在Sales Connect中更新您的任务列表。

要打开此同步，只需选中Web应用程序的[设置页面](https://toutapp.com/login)中的同步框。

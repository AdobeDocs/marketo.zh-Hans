---
unique-page-id: 14352541
description: 首次将销售连接任务与Salesforce同步 — Marketo文档 — 产品文档
title: 首次将销售连接任务与Salesforce同步
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 首次将销售连接任务与Salesforce同步 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

首次打开Sales Connect和Salesforce任务之间的同步时，我们会导入您的Salesforce任务。 我们会 **not** 将您在Sales Connect中拥有的任何当前任务推送到Salesforce。 为了减少混乱和重复项，从Sales Connect到Salesforce中同步的任务只有创建的任务 *after* 将Sales Connect与SFDC同步。

下面是同步Sales Connect和SFDC任务时发生的情况：

- 单击“保存任务”同步后，这些任务即开始同步。 这最初需要一些时间。

- 在过去24小时内更新或创建的任何提醒都将从SFDC提取到Sales Connect。 同步基于到期日期，所有这些任务都将在后端同步，但在命令中心，您将只看到今天和明天到期的任务。

- 如果之前已打开同步，并且您删除了SFDC中的任何任务，则过去15天内删除的任何任务都将从命令中心删除。

- 只要同步处于启用状态，我们就会在Sales Connect和SFDC之间不断同步任务。

初始同步后，您在Sales Connect中创建、编辑、完成或删除的任何任务都将同步到Salesforce中的任务列表。 而在Salesforce中创建、编辑、完成或删除的任何内容都将在Sales Connect中更新您的任务列表。

要打开此同步，只需选中 [“设置”页面](https://toutapp.com/login) 在web应用程序中。

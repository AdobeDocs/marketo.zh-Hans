---
unique-page-id: 14352541
description: 首次将Sales Connect Tasks与Salesforce同步 — Marketo文档 — 产品文档
title: 首次将Sales Connect任务与Salesforce同步
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 首次将Sales Connect任务与Salesforce同步 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

当您首次打开Sales Connect和Salesforce任务之间的同步时，我们会导入您的Salesforce任务。 我们会 **非** 将您在Sales Connect中拥有的任何当前任务推送到到Salesforce。 为了减少杂乱和重复项，从Sales Connect同步到Salesforce中的唯一任务是创建的 *之后* 将Sales Connect与SFDC同步。

以下是同步Sales Connect和SFDC任务时会发生的情况：

- 在同步任务时单击“保存”后，它们就会开始进行同步。 这最初需要一些时间。

- 过去24小时内已更新或创建的任何提醒都将从SFDC拉入Sales Connect。 同步基于到期日期，所有这些任务将在后端进行同步，但在指挥中心，您只能看到今天和明天到期的任务。

- 如果以前启用了同步，并且您删除了SFDC中的任何任务，则过去15天内删除的任何任务都将从命令中心删除。

- 只要启用同步，我们就会不断在Sales Connect和SFDC之间同步任务。

初次同步后，您在Sales Connect中创建、编辑、完成或删除的任何任务都将同步到Salesforce中的任务列表。 在Salesforce中创建、编辑、完成或删除的任何内容都将在Sales Connect中更新您的任务列表。

要开启此同步，只需选中您的页面中的 [“设置”页面](https://toutapp.com/login) 在Web应用程序中。

---
unique-page-id: 14352541
description: 首次将Sales Connect任务与Salesforce同步 — Marketo文档 — 产品文档
title: 首次将 Sales Connect 任务与 Salesforce 同步
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 3%

---

# 首次将[!DNL Sales Connect]任务与[!DNL Salesforce]同步 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

当您首次打开[!DNL Sales Connect]和[!DNL Salesforce]任务之间的同步时，我们会导入您的[!DNL Salesforce]任务。 我们&#x200B;**不会**&#x200B;将您在[!DNL Sales Connect]中拥有的任何当前任务推送到[!DNL Salesforce]。 为了减少待处理内容和重复项，从[!DNL Sales Connect]同步到[!DNL Salesforce]的任务只有在&#x200B;*之后您将*&#x200B;与SFDC同步的[!DNL Sales Connect]创建的任务。

以下是同步[!DNL Sales Connect]和SFDC任务时发生的情况：

- 在同步的任务上单击“保存”后，它们就会开始进行同步。 这最初将需要一些时间。

- 过去24小时内已更新或创建的任何提醒都将从SFDC拉入[!DNL Sales Connect]。 同步基于到期日期，所有这些任务将在后端进行同步，但在命令中心，您只能看到今天和明天到期的任务。

- 如果以前启用了同步，并且您删除了SFDC中的任何任务，则过去15天内删除的任何任务都将从命令中心删除。

- 只要已启用同步，我们就会一直在[!DNL Sales Connect]和SFDC之间同步任务。

初始同步后，您在[!DNL Sales Connect]中创建、编辑、完成或删除的任何任务都将同步到[!DNL Salesforce]中的任务列表。 在[!DNL Salesforce]中创建、编辑、完成或删除的任何内容都将在[!DNL Sales Connect]中更新您的任务列表。

若要启用此同步，只需在Web应用程序的[设置页面](https://toutapp.com/login)中选中同步框即可。

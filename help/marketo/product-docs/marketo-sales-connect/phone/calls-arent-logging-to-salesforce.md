---
unique-page-id: 14352435
description: 调用未登录到Salesforce - Marketo文档 — 产品文档
title: 调用未登录到Salesforce
exl-id: 99528c1a-7398-442b-81d1-9b5908e35e2f
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%

---

# 调用未登录到Salesforce {#calls-arent-logging-to-salesforce}

如果您希望将来自Sales Phone的呼叫自动记录到Salesforce，请确保已实施以下操作。

您需要将Sales Connect帐户通过API连接连接到[Salesforce帐户](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)。

如果您是从[Web应用程序](https://toutapp.com/login)中调用，则需要将一个Salesforce ID保存到该联系人。 [单击此处](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/import-a-salesforce-id-into-sales-connect.md)查看如何确保所有Sales Connect联系人都有一个与其关联的Salesforce ID。

>[!NOTE]
>
>确保您的任务类型选择列表中有“呼叫”，以便在Salesforce中准确而轻松地报告。

完成该操作后，您将在Salesforce的Activity History部分看到一个已创建的任务。

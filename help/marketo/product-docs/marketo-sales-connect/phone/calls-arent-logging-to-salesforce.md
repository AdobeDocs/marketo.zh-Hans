---
unique-page-id: 14352435
description: 调用未登录到Salesforce - Marketo文档 — 产品文档
title: 通话未记录到 Salesforce
exl-id: 99528c1a-7398-442b-81d1-9b5908e35e2f
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 4%

---

# 呼叫未记录到[!DNL Salesforce] {#calls-arent-logging-to-salesforce}

如果您希望将来自销售电话的呼叫自动记录到[!DNL Salesforce]，请确保已实施以下操作。

您需要通过API连接将您的[!DNL Sales Connect]帐户连接到您的[[!DNL Salesforce] 帐户](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)。

如果您是从[Web应用程序](https://toutapp.com/login)调用，则需要将一个[!DNL Salesforce] ID保存到该联系人。 [单击此处](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/import-a-salesforce-id-into-sales-connect.md)查看如何确保所有[!DNL Sales Connect]联系人都有一个与其关联的[!DNL Salesforce] ID。

>[!NOTE]
>
>确保您的任务类型选择列表中有“呼叫”，以便在[!DNL Salesforce]中准确而轻松地报告。

完成此操作后，您将在[!DNL Salesforce]的Activity History部分看到已创建的任务。

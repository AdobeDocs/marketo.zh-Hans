---
unique-page-id: 1147082
description: 删除人员 — Marketo文档 — 产品文档
title: 删除人员
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# 删除人员 {#delete-person}

错误的人有时会进入您的数据库。 可以使用“删除人员”流程步骤删除这些人员。

![](assets/delete-person-1.png)

>[!CAUTION]
>
>在删除人员时，也将删除其所有历史RCE数据。 无法撤消此操作。

1. 当您在流程步骤中拖动时，它也会自动设置为从您的CRM中删除。

   ![](assets/delete-person-2.png)

1. 您可以从Marketo Engage中删除，但不能从CRM中删除，如下所示：

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>从CRM _中删除此人仅适用于[!DNL Salesforce]_。 如果您从Marketo中删除人员并选择将他们保留在[!DNL Salesforce]中，则当他们的[!DNL Salesforce]记录更新时，将在Marketo中重新创建他们。

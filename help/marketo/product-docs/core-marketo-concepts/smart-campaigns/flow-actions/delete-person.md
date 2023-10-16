---
unique-page-id: 1147082
description: 删除人员 — Marketo文档 — 产品文档
title: 删除人员
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 1%

---

# 删除人员 {#delete-person}

错误的人有时会进入您的数据库。 可以使用“删除人员”流程步骤删除这些人员。

## 概述 {#overview}

在Smart Campaign中使用流程步骤。

![](assets/one-4.png)

>[!CAUTION]
>
>在删除人员时，也将删除其所有历史RCE数据。 无法撤消此操作。

## 使用情况 {#usage}

当您在流程步骤中拖动时，它也会自动设置为从CRM中删除。

![](assets/two-4.png)

您可以从Marketo Engage中删除，但不能从CRM中删除，如下所示：

![](assets/three-3.png)

>[!NOTE]
>
>从您的CRM中删除人员 _仅适用于[!DNL Salesforce]_. 如果您从Marketo中删除人员并选择将其保留在 [!DNL Salesforce]，则它们将在Marketo中重新创建，如果 [!DNL Salesforce] 记录会随时更新。

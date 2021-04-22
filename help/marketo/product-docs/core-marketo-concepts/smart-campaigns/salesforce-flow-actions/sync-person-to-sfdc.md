---
unique-page-id: 1147027
description: 将人员同步到SFDC - Marketo Docs — 产品文档
title: 将人员同步到SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---

# 将人员同步到SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>仅在与Salesforce集成时可用。

## 概述{#overview}

此流步骤将将Marketo创建的人员作为潜在客户插入您的Salesforce CRM。

![](assets/sync-person-to-sfdc.png)

## 用法{#usage}

1. 默认情况下，此流步骤将根据Salesforce自动分配规则分配给潜在客户所有者。

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce要求人员填写公司和姓氏字段。 否则，它将拒绝潜在客户记录。

1. 您可以将特定Salesforce用户或潜在客户队列设置为潜在客户所有者。

   ![](assets/sync-person-to-sfdc-2.png)

   使用此流步骤时，该人员将立即同步为Salesforce潜在客户，无需等待定期同步。

   >[!CAUTION]
   >
   >Salesforce不允许将“联系人”分配到潜在客户队列。 在这种情况下，Marketo将在Salesforce中创建一个重复“潜在客户”。

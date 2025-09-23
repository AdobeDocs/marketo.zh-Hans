---
unique-page-id: 1147027
description: 将人员同步到SFDC - Marketo文档 — 产品文档
title: 将人员同步到 SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 6%

---

# 将人员同步到 SFDC {#sync-person-to-sfdc}

此流程步骤将把由Marketo创建的人作为潜在客户插入到您的Salesforce CRM。

>[!NOTE]
>
>仅在与[!DNL Salesforce]集成时可用。

1. 默认情况下，此流程步骤将根据Salesforce自动分配规则分配给销售线索责任人。

   ![](assets/sync-person-to-sfdc-1.png)

   >[!TIP]
   >
   >[!DNL Salesforce]要求人员填写公司和姓氏字段。 否则，它将拒绝潜在客户记录。

1. 您可以将特定的[!DNL Salesforce]用户或潜在客户队列设置为潜在客户所有者。

   ![](assets/sync-person-to-sfdc-2.png)

   使用此流程步骤时，人员将立即同步为[!DNL Salesforce]潜在客户，而无需等待常规同步。

   >[!CAUTION]
   >
   >[!DNL Salesforce]不允许将“联系人”分配给潜在客户队列。 在这种情况下，Marketo将在[!DNL Salesforce]中创建重复的“Lead”。

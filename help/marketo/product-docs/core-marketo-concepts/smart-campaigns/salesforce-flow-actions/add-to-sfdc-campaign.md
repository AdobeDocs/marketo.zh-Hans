---
unique-page-id: 1147034
description: 添加到SFDC活动- Marketo Docs —— 产品文档
title: 添加到SFDC活动
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# 添加到SFDC活动{#add-to-sfdc-campaign}

>[!NOTE]
>
>仅当与Salesforce集成时可用。

## 概述{#overview}

此流步骤可用于Marketo活动，或作为单个流步骤将人员添加为Salesforce活动中的潜在客户。 如果Salesforce中尚不存在该潜在客户，它将自动同步并添加到具有指定状态的活动。

![](assets/image2014-9-22-15-3a43-3a36.png)

## 用法{#usage}

1. 查找并选择要将潜在客户添加到的Salesforce活动。

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >如果您在活动列表中看不到Salesforce活动:
   >
   >    
   >    
   >    1. 确保[活动同步已启用](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)。
   >    1. 确认您的[Marketo Sync User](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)是Salesforce中的[Marketing User](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)。


   >[!TIP]
   >
   >您可以使用Salesforce活动[我的令牌](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)简化项目克隆。

1. 选择要在添加潜在客户时分配给潜在客户的Salesforce活动成员状态。

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >如果某人已经是Salesforce活动的潜在客户成员，则将跳过他们，并且不会更新他们的状态。 您可以改用[更改SFDC活动](change-status-in-sfdc-campaign.md)中的状态。


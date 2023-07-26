---
unique-page-id: 1147034
description: 添加到SFDC Campaign - Marketo文档 — 产品文档
title: 添加到SFDC Campaign
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# 添加到SFDC Campaign {#add-to-sfdc-campaign}

>[!NOTE]
>
>仅在与Salesforce集成时可用。

## 概述 {#overview}

此流程步骤可以在Marketo营销活动中使用，也可以作为单个流程步骤在Salesforce营销活动中添加人员作为潜在客户。 如果Salesforce中尚不存在潜在客户，则它会自动同步到具有指定状态的营销策划中，并将其添加到营销策划中。

![](assets/image2014-9-22-15-3a43-3a36.png)

## 使用情况 {#usage}

1. 查找并选择要为其添加潜在客户的Salesforce营销活动。

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >如果在Campaign列表中看不到Salesforce营销活动：
   >
   >  1. 确保 [campaign同步已启用](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >  1. 确认您的 [Marketo同步用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 是 [营销用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) 在Salesforce中。

   >[!TIP]
   >
   >您可以使用Salesforce营销活动 [我的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) 使程序克隆更容易。

1. 选择添加潜在客户时要分配给这些潜在客户的Salesforce营销活动成员状态。

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >如果人员已经是Salesforce营销活动的主要成员，则将跳过这些人员并且不会更新其状态。 您可以使用 [在SFDC营销活动中更改其状态](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md) 而是。

---
unique-page-id: 1147034
description: 添加到SFDC Campaign - Marketo文档 — 产品文档
title: 添加到SFDC Campaign
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# 添加到SFDC Campaign {#add-to-sfdc-campaign}

此流程步骤可以在Marketo Engage营销活动中使用，也可以作为单个流程步骤在Salesforce营销活动中添加人员作为潜在客户。 如果Salesforce中尚不存在该商机，则它会自动同步到并添加到具有指定状态的营销活动中。

>[!NOTE]
>
>仅在与[!DNL Salesforce]集成时可用。

![](assets/add-to-sfdc-campaign-1.png)

## 使用情况 {#usage}

1. 查找并选择要为其添加潜在客户的[!DNL Salesforce]营销活动。

   ![](assets/add-to-sfdc-campaign-2.png)

   >[!TIP]
   >
   >如果在营销活动列表中看不到Salesforce营销活动：
   >
   >  1. 确保已启用[营销活动同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}。
   >  1. 确认您的[Marketo同步用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}是Salesforce中的[营销用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}。

   >[!TIP]
   >
   >您可以使用Salesforce campaign [我的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}简化程序克隆过程。

1. 选择要在添加潜在客户时分配给潜在客户的[!DNL Salesforce]营销活动成员状态。

   ![](assets/add-to-sfdc-campaign-3.png)

   >[!CAUTION]
   >
   >如果人员已经是Salesforce营销活动的牵头成员，则将跳过这些人员并且不会更新其状态。 您可以改用[在SFDC营销活动中更改其状态](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}。

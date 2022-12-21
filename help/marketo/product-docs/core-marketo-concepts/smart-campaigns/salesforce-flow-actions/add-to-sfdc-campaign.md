---
unique-page-id: 1147034
description: 添加到SFDC Campaign - Marketo文档 — 产品文档
title: 添加到SFDC营销活动
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# 添加到SFDC营销活动 {#add-to-sfdc-campaign}

>[!NOTE]
>
>仅在与Salesforce集成时可用。

## 概述 {#overview}

此流程步骤可在Marketo促销活动中使用，或用作单一流程步骤，将人员添加为Salesforce促销活动中的潜在客户。 如果Salesforce中尚不存在该潜在客户，则该潜在客户将自动同步并添加到具有指定状态的营销活动。

![](assets/image2014-9-22-15-3a43-3a36.png)

## 使用情况 {#usage}

1. 查找并选择要将潜在客户添加到的Salesforce营销活动。

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >如果在促销活动列表中看不到Salesforce促销活动，请执行以下操作：
   >
   >  1. 确保 [营销活动同步已启用](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >  1. 确认 [Marketo同步用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 是 [营销用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) 在Salesforce中。


   >[!TIP]
   >
   >您可以使用Salesforce促销活动 [我的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) 使程序克隆更容易。

1. 选择要在添加潜在客户时分配给其的Salesforce促销活动成员状态。

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >如果人员已经是Salesforce营销活动的主要成员，则将跳过该人员，且不会更新其状态。 您可以使用 [在SFDC营销活动中更改其状态](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md) 中。

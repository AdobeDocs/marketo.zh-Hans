---
unique-page-id: 2953469
description: SFDC同步 — 活动同步 — Marketo文档 — 产品文档
title: SFDC同步 — 活动同步
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# SFDC同步：活动同步{#sfdc-sync-campaign-sync}

Marketo项目可以与Salesforce活动同步。 以下是工作原理的概述。

## 为什么我应将Marketo项目与Salesforce活动同步？{#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* 使用Marketo项目的强大功能。
* 使成员及其状态在Marketo项目和Salesforce活动之间保持同步。
* 利用Marketo和Salesforce中的报告功能。

## Marketo项目和Salesforce活动如何同步？{#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

在Marketo中，您可以选择在项目和Salesforce活动之间创建一对一映射。

![](assets/image2015-7-8-9-3a43-3a8.png)

Marketo中的&#x200B;**[渠道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)**&#x200B;和&#x200B;**[期间成本](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)**&#x200B;与Salesforce同步，作为&#x200B;**活动类型**&#x200B;和&#x200B;**实际成本**。 此同步是从Marketo到Salesforce的&#x200B;**单向**。

Marketo **项目成员**&#x200B;及其&#x200B;**[进度状态](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)**&#x200B;与&#x200B;**Salesforce活动成员**&#x200B;和&#x200B;**活动成员状态**&#x200B;保持同步。 这是&#x200B;**双向同步**，因此在Marketo或Salesforce中所做的任何更改都会反映在这两个系统中。

>[!NOTE]
>
>如果Marketo项目中有Salesforce中不存在的成员，则Marketo会将这些成员创建为Salesforce中的潜在客户。

## 触发器/过滤器与活动相关？{#what-are-the-triggers-filters-related-to-campaigns}

触发器：

* 添加到SFDC活动
* 已从SFDC活动中删除
* 状态在SFDC活动中更改

过滤器:

* SFDC活动成员

## 是否可以将Marketo People添加到我的SFDC活动?{#can-i-add-marketo-people-to-my-sfdc-campaign}

是，请使用[添加到SFDC活动流操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md)。 如果此人员在Salesforce中不存在，Marketo将在Salesforce中创建此人员，然后将其添加到活动。

## 是否可以使用Marketo从SFDC活动中删除成员？{#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

是，请使用[从SFDC活动流动操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md)删除。

## 我是否可以使用Marketo更改活动成员状态？{#can-i-change-campaign-member-status-using-marketo}

是，请使用SFDC活动流操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md)中的[更改状态。

## 为什么我看不到任何Salesforce活动?{#why-cant-i-see-any-of-my-salesforce-campaigns}

以下是您可以检查的内容：

1. 确保[活动同步已启用](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)。
1. 确认您的[Marketo同步用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)是Salesforce中的[营销用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)。

>[!NOTE]
>
>如果您的Salesforce活动和映射的Marketo项目具有不兼容的项目状态，您可能会收到错误消息。 我们建议您[在同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)之前匹配项目状态。

>[!MORELIKETHIS]
>
>* [将SFDC活动与项目同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [了解项目会员资格](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [启用/禁用活动同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [使Marketo Sync用户成为营销用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)


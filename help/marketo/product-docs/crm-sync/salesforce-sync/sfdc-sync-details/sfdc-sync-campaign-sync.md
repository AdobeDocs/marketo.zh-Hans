---
unique-page-id: 2953469
description: SFDC同步 — 促销活动同步 — Marketo文档 — 产品文档
title: SFDC同步 — Campaign同步
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
source-git-commit: 8781c6cf2e64543809fe697e75ae6884969a4e40
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# SFDC同步：营销活动同步 {#sfdc-sync-campaign-sync}

Marketo项目可以与Salesforce促销活动同步。 以下是工作原理的概述。

## 为何应将Marketo项目与Salesforce促销活动同步？ {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* 使用Marketo计划的强大功能。
* 使成员及其状态在Marketo项目和Salesforce营销活动之间保持同步。
* 在Marketo和Salesforce中点按报表功能。

## Marketo计划与Salesforce促销活动如何同步？ {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

在Marketo中，您可以选择在项目和Salesforce营销活动之间创建一对一映射。

![](assets/image2015-7-8-9-3a43-3a8.png)

Marketo中的&#x200B;**[channel](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)**&#x200B;和&#x200B;**[期间成本](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)**&#x200B;与Salesforce同步，作为&#x200B;**促销活动类型**&#x200B;和&#x200B;**实际成本**。 此同步是从Marketo到Salesforce的&#x200B;**单向**&#x200B;同步。

Marketo **项目成员**&#x200B;及其&#x200B;**[进度状态](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)**&#x200B;与&#x200B;**Salesforce促销活动成员**&#x200B;和&#x200B;**促销活动成员状态**&#x200B;保持同步。 这是&#x200B;**双向同步**，因此在Marketo或Salesforce中所做的任何更改都会反映在这两个系统中。

>[!NOTE]
>
>如果Marketo计划中的成员在Salesforce中不存在，则Marketo会在Salesforce中创建这些成员作为潜在客户。

## 哪些触发器/过滤器与营销活动相关？ {#what-are-the-triggers-filters-related-to-campaigns}

触发器：

* 已添加到SFDC营销活动
* 从SFDC Campaign中删除
* 在SFDC Campaign中状态已更改

过滤器：

* SFDC营销活动成员

## 我可以将Marketo People添加到我的SFDC营销活动吗？ {#can-i-add-marketo-people-to-my-sfdc-campaign}

是，请使用[添加到SFDC促销活动流操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md)。 如果此人员不存在于Salesforce中，则Marketo将在Salesforce中创建该人员，然后将其添加到营销活动中。

## 我能否使用Marketo从SFDC营销活动中删除成员？ {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

是，使用[从SFDC Campaign流程操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md)删除。

## 我能否使用Marketo更改营销活动成员状态？ {#can-i-change-campaign-member-status-using-marketo}

是，请使用[在SFDC促销活动流操作中更改状态](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md)。

## 为什么看不到我的任何Salesforce营销活动？ {#why-cant-i-see-any-of-my-salesforce-campaigns}

您可以检查以下内容：

1. 确保[促销活动同步已启用](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)。
1. 确认您的[Marketo同步用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)是Salesforce中的[营销用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)。

>[!NOTE]
>
>如果您的Salesforce营销活动和映射的Marketo项目具有不兼容的项目状态，则可能会收到错误消息。 我们建议您[在同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)之前匹配程序状态。

>[!MORELIKETHIS]
>
>* [将SFDC营销活动与项目同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [了解计划会员资格](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [启用/禁用营销活动同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [将Marketo同步用户设为营销用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)


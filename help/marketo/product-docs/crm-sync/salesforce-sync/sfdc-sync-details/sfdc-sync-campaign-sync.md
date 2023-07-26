---
unique-page-id: 2953469
description: SFDC同步 — Campaign同步 — Marketo文档 — 产品文档
title: SFDC同步 — Campaign同步
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# SFDC同步： Campaign同步 {#sfdc-sync-campaign-sync}

Marketo项目可以与Salesforce Campaigns同步。 下面是其工作原理的概述。

## 为何要将Marketo项目与Salesforce促销活动同步？ {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* 使用Marketo程序的强大功能。
* 在Marketo项目和Salesforce营销活动之间保持成员及其状态同步。
* 点按Marketo和Salesforce中的报表功能。

## Marketo项目和Salesforce营销活动如何同步？ {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

在Marketo中，您可以选择在项目和Salesforce营销策划之间创建一对一映射。

![](assets/image2015-7-8-9-3a43-3a8.png)

此 **[渠道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** 和 **[期间成本](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** 在Marketo中，同步到Salesforce作为 **营销活动类型** 和 **实际成本**. 此同步为 **单向**，从Marketo到Salesforce。

Marketo **计划成员** 和他们的 **[进度状态](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** 将保持与 **Salesforce营销活动成员** 和 **营销活动成员状态**. 这是 **双向同步**，因此在Marketo或Salesforce中所做的任何更改都会反映在这两个系统中。

>[!NOTE]
>
>如果Marketo程序中有成员在Salesforce中不存在，则Marketo会创建这些人员作为Salesforce中的潜在客户。

## 与活动相关的触发器/过滤器有哪些？ {#what-are-the-triggers-filters-related-to-campaigns}

触发器：

* 已添加到SFDC Campaign
* 已从SFDC Campaign中删除
* SFDC Campaign中的状态已更改

过滤器:

* SFDC营销活动成员

## 能否将Marketo人员添加到我的SFDC营销活动？ {#can-i-add-marketo-people-to-my-sfdc-campaign}

是，使用 [添加到SFDC营销活动流程操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). 如果此人员在Salesforce中不存在，则Marketo将在Salesforce中创建它，然后将他/她添加到营销活动中。

## 我是否可以使用Marketo从SFDC营销活动中删除成员？ {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

是，使用 [从SFDC Campaign流程操作中删除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md).

## 我可以使用Marketo更改营销活动成员状态吗？ {#can-i-change-campaign-member-status-using-marketo}

是，使用 [在SFDC Campaign流程操作中更改状态](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).

## 为什么我看不到任何Salesforce营销活动？ {#why-cant-i-see-any-of-my-salesforce-campaigns}

您可以检查以下内容：

1. 确保 [campaign同步已启用](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. 确认您的 [Marketo同步用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 是 [营销用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) 在Salesforce中。

>[!NOTE]
>
>如果您的Salesforce营销活动和映射的Marketo项目的项目状态不兼容，您可能会收到一条错误消息。 我们建议您 [匹配同步前的程序状态](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [将SFDC Campaign与程序同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [了解计划成员资格](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [启用/禁用Campaign同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [将Marketo同步用户设为营销用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

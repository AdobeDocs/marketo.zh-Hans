---
unique-page-id: 2953467
description: SFDC同步 — Opportunity同步 — Marketo文档 — 产品文档
title: SFDC同步 — 机会同步
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# SFDC同步：机会同步 {#sfdc-sync-opportunity-sync}

## 两个系统之间的机会详细信息如何保持同步？ {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

同步是单向的：从Salesforce到Marketo。 对Salesforce中业务机会的更新将同步到Marketo。

>[!NOTE]
>
>此 [您在Marketo中为Salesforce输入的凭据](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 用于同步数据。 仅包含这些凭据有权访问的数据。

## 我可以启动Opportunity同步吗？ {#can-i-initiate-an-opportunity-sync}

不，你不能。对Salesforce中的任何机会所做的更改将自动同步到Marketo。

## Marketo是否支持在机会金额中使用多种货币？ {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

不支持，Marketo仅支持一种货币。 机会金额将从Salesforce同步，但货币将为 [默认货币](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) 在您的Marketo订阅中。

## Marketo如何关联机会和联系人？ {#how-does-marketo-associate-opportunities-and-contacts}

Marketo使用以下方式关联机会和联系人 [机会联系人角色](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm). 未分配任何联系人角色的机会将同步到Marketo，但不会属于任何人。 例如，人员将不符合具有机会过滤器的条件。

## 我如何才能看到一个人的所有机会？ {#how-can-i-see-all-the-opportunities-of-a-person}

您可以在 **机会信息** 选项卡 [人员详细信息](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) 页面。

## 与机会相关的触发器/过滤器有哪些？ {#what-are-the-triggers-filters-related-to-opportunity}

触发器：

* 已添加到机会
* 已从机会中移除
* 机会已更新

过滤器:

* 具有机会
* Opportunity已更新/Not Opportunity已更新
* 已添加到Opportunity/未添加到Opportunity
* 已从Opportunity中删除/未从Opportunity中删除
* 总商机金额
* 选件数
* 预计总商机收入

>[!TIP]
>
>查看有关筛选器和触发器的限制。 里面有很多很酷的细节。
>
>只需在Salesforce的opportunity对象中创建一个新字段，它就会自动成为约束！

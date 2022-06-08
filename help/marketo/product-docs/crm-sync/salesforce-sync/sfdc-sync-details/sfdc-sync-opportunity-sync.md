---
unique-page-id: 2953467
description: SFDC同步 — 机会同步 — Marketo文档 — 产品文档
title: SFDC同步 — 机会同步
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# SFDC同步：机会同步 {#sfdc-sync-opportunity-sync}

## 如何在两个系统之间保持机会详细信息的同步？ {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

同步是一种方式：从Salesforce到Marketo。 Salesforce中的商机更新将同步到Marketo。

>[!NOTE]
>
>的 [您在Marketo for Salesforce中输入的凭据](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) 用于通过同步数据。 将只包含这些凭据有权访问的数据。

## 我能否启动机会同步？ {#can-i-initiate-an-opportunity-sync}

不行。对Salesforce中任何销售机会的更改将自动同步到Marketo。

## Marketo是否支持Opportunity Amount中的多种货币？ {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

不，Marketo只支持一种货币。 商机金额将从Salesforce同步，但货币将为 [默认货币](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) 在您的Marketo订阅中。

## Marketo如何关联机会和联系人？ {#how-does-marketo-associate-opportunities-and-contacts}

Marketo联系商机和联系人使用 [机会联系角色](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm). 未分配任何联系人角色的机会将同步到Marketo，但不属于任何人。 例如，该人员将不符合Has Opportunity筛选条件。

## 我如何才能看到一个人的所有机会？ {#how-can-i-see-all-the-opportunities-of-a-person}

您可以在 **机会信息** 选项卡 [人员详细信息](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) 页面。

## 哪些触发器/过滤器与业务机会相关？ {#what-are-the-triggers-filters-related-to-opportunity}

触发器：

* 已添加到机会中
* 从商机中删除
* 机会已更新

过滤器:

* 有机会
* Opportunity was Updated/Not Opportunity was Updated
* 已添加到Opportunity/Not已添加到Opportunity
* 已从Opportunity中删除/未从Opportunity中删除
* 产品总额
* 选项数
* 预计总运营收入

>[!TIP]
>
>了解对过滤器和触发器的限制。 里面有很多很酷的细节。
>
>只需在Salesforce中的机会对象中创建一个新字段，它就会自动成为一个限制！

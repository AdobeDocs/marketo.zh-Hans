---
unique-page-id: 2953467
description: SFDC Sync -Opportunity Sync - Marketo Docs — 产品文档
title: SFDC同步 — 机会同步
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# SFDC同步：Opportunity Sync {#sfdc-sync-opportunity-sync}

## 如何使两个系统之间的机会详细信息保持同步？{#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

同步是一种方式：从Salesforce到Marketo。 对Salesforce中业务机会的更新将同步到Marketo。

>[!NOTE]
>
>您在Marketo中为Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)输入的[凭据用于同步数据。 将仅包含这些凭据有权访问的数据。

## 我是否可以启动Opportunity Sync?{#can-i-initiate-an-opportunity-sync}

不行。对Salesforce中任何业务机会的更改将自动同步到Marketo。

## Marketo是否支持Opportunity Amount中的多种货币？{#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

不，Marketo只支持一种货币。 业务机会金额将从Salesforce同步，但币种将是您的Marketo订阅中的[默认货币](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription)。

## Marketo如何关联机会和联系人？{#how-does-marketo-associate-opportunities-and-contacts}

Marketo使用[Opportunity Contact Roles](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm)将Opportunity和Contact关联起来。 未分配任何联系角色的Opportunity将同步到Marketo，但不属于任何人。 例如，此人将不符合Has Opportunity过滤器的资格。

## 我如何看到一个人的所有机会？{#how-can-i-see-all-the-opportunities-of-a-person}

您可以在[人员详细信息](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)页面的&#x200B;**机会信息**&#x200B;选项卡中视图一个机会列表。

## 哪些触发器/过滤器与机会相关？{#what-are-the-triggers-filters-related-to-opportunity}

触发器：

* 已添加到业务机会
* 从机会中删除
* 已更新业务机会

过滤器:

* 有机会
* Opportunity was Updated/Not Opportunity was Updated
* Was Added to Opportunity/Not Bas Added to Opportunity
* 已从Opportunity中删除/未从Opportunity中删除
* 产权总额
* Optys数
* 预期总业务收入

>[!TIP]
>
>了解过滤器和触发器的约束。 里面有很多很酷的细节。
>
>只需在Salesforce中的机会对象中创建一个新字段，它将自动成为一个约束！

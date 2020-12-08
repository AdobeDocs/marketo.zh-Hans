---
unique-page-id: 2953467
description: SFDC Sync - Opportunity Sync - Marketo Docs —— 产品文档
title: SFDC Sync - Opportunity Sync
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# SFDC同步：机会同步 {#sfdc-sync-opportunity-sync}

## 如何在两个系统之间保持机会详细信息同步？ {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

同步是一种方式：从Salesforce到Marketo。 对Salesforce中业务机会的更新将同步到Marketo。

>[!NOTE]
>
>您 [在Marketo中为Salesforce输入的凭据](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) ，用于同步数据。 将仅包含这些凭据有权访问的数据。

## 我是否可以启动Opportunity Sync? {#can-i-initiate-an-opportunity-sync}

不行。对Salesforce中任何业务机会的更改将自动同步到Marketo。

## Marketo是否支持“机会金额”中的多种货币？ {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

不，Marketo仅支持一种货币。 业务机会金额将与Salesforce同步，但币种将是您的营销 [订阅中](https://docs.marketo.com/display/DOCS/Set+Default+Location+Settings+for+a+Subscription#SetDefaultLocationSettingsforaSubscription-SettheDefaultCurrencySettingsforaSubscription) 的默认币种。

## Marketo如何关联机会和联系人？ {#how-does-marketo-associate-opportunities-and-contacts}

Marketo使用Opportunity Contact Roles将Opportunity和 [联系人关联起来](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm)。 未分配任何联系人角色的机会将同步到Marketo，但不属于任何人。 例如，此人将不符合Has Opportunity筛选条件。

## 我如何看到一个人的所有机会？ {#how-can-i-see-all-the-opportunities-of-a-person}

您可以在“人员详细信息”页面的“ **业务机会信息** ”选项卡中 [视图一](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) 个业务机会列表。

## 触发器/过滤器与机会有哪些关系？ {#what-are-the-triggers-filters-related-to-opportunity}

触发器：

* 已添加到机会
* 从销售机会中删除
* 业务机会已更新

过滤器:

* 有机会
* Opportunity was Updated/Not Opportunity was Updated
* 已添加到Opportunity/Not已添加到Opportunity
* 已从Opportunity中删除／未从Opportunity中删除
* 产品总数
* Optys数
* 预计总业务收入

>[!TIP]
>
>了解过滤器和触发器的约束。 里面有很多很酷的细节。
>
>只需在Salesforce中的机会对象中创建一个新字段，它将自动成为一个约束！

Marketo拥有世界上最好的Salesforce同步！
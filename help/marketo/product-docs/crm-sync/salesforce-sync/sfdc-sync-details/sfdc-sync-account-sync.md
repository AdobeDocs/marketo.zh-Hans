---
unique-page-id: 2953459
description: SFDC同步 — 帐户同步 — Marketo文档 — 产品文档
title: SFDC同步 — 帐户同步
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# SFDC同步：帐户同步 {#sfdc-sync-account-sync}

Marketo Engage还会将您的帐户信息与Salesforce同步。 以下是一些您应了解的具体事项！

## 信息以何种方式同步？ {#which-way-does-the-information-sync}

只有一个办法：从SFDC到Marketo。

## 这些更新是如何工作的？ {#how-do-the-updates-work}

如果您在Marketo中更新某个联系人的“帐户”字段，则会在Marketo中更改属于该帐户的所有联系人的值。 它不会同步到SFDC。 但是，下次在SFDC中更新该帐户时，更改将覆盖Marketo中的所有帐户信息。

## 联系人是否可以属于多个帐户？  {#can-a-contact-belong-to-multiple-accounts}

否. 一个帐户可以有多个联系人，一个联系人只能有一个帐户。

## 我能否从Marketo创建帐户？ {#can-i-create-accounts-from-marketo}

大多没有。 但是，如果您使用 [转换人员](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} 流程步骤，它将创建一个新Contact、一个新Account和一个新Opportunity。

>[!CAUTION]
>
>此流程步骤的用例非常有限。 如果您不确定，则可能不应使用它。

## 在Salesforce中帐户字段的更改是否会导致每个联系人的更改数据值活动日志？  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

大部分，是的。 但是，如果某个帐户拥有超过5,000个联系人，并且该帐户上的某个字段在SFDC中发生更改，我们会同步该更改，但不会记录5,000多个联系人的活动。

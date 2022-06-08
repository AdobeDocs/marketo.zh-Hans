---
unique-page-id: 2953459
description: SFDC同步 — 帐户同步 — Marketo文档 — 产品文档
title: SFDC同步 — 帐户同步
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---

# SFDC同步：帐户同步 {#sfdc-sync-account-sync}

Marketo还会将您的帐户信息与Salesforce同步。 以下是一些您应该了解的具体事项！

## 信息同步的方式是什么？ {#which-way-does-the-information-sync}

只有一种方式：从SFDC到Marketo。

## 如何进行更新？ {#how-do-the-updates-work}

如果您更新Marketo中某个联系人的“帐户”字段，则会更改Marketo中属于该帐户的所有联系人的值。 它不会同步到SFDC。 但是，下次在SFDC中更新该帐户时，更改将覆盖Marketo中的所有帐户信息。

## 联系人是否属于多个帐户？  {#can-a-contact-belong-to-multiple-accounts}

否. 一个帐户可以有多个联系人，一个联系人只能有一个帐户。

## 我可以从Marketo创建帐户吗？ {#can-i-create-accounts-from-marketo}

大多数情况下，不。 但是，如果您使用 [转换人员](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) 流程步骤，将创建新联系人、新帐户和新机会。

>[!CAUTION]
>
>此流程步骤的用例非常有限。 如果你不确定，你可能不该用它。

## Salesforce中帐户字段的更改是否会导致每个联系人的更改数据值活动日志？  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

大多数情况下，是的。 但是，如果一个帐户有5,000个以上的联系人，并且该帐户上的字段在SFDC中发生更改，则我们会同步更改，但不记录5,000个以上联系人的活动。

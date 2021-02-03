---
unique-page-id: 2953459
description: SFDC Sync —— 帐户同步- Marketo Docs —— 产品文档
title: SFDC同步——帐户同步
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# SFDC同步：帐户同步{#sfdc-sync-account-sync}

Marketo还会将您的帐户信息与Salesforce同步。 以下是您应该了解的一些具体内容！

## 信息以哪种方式同步？{#which-way-does-the-information-sync}

只有一种方式：从SFDC到Marketo。

## 这些更新如何工作？{#how-do-the-updates-work}

如果您在Marketo中更新了联系人的“帐户”字段，则会更改Marketo中属于该帐户的所有联系人的值。 它不同步到SFDC。 但是，下次在SFDC中更新该帐户时，更改将覆盖Marketo中的所有帐户信息。

## 联系人是否属于多个帐户？ {#can-a-contact-belong-to-multiple-accounts}

不。 一个帐户可以有多个联系人，一个联系人只能有一个帐户。

## 我可以从Marketo创建帐户吗？{#can-i-create-accounts-from-marketo}

大多数情况下，不。 但是，如果对人员使用[转换人员](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)流程步骤，将创建新的联系人、新的帐户和新的机会。

>[!CAUTION]
>
>此流步骤的用例非常有限。 如果你不确定，你可能不该用它。

## Salesforce中帐户字段的更改是否会为每个联系人生成更改数据值活动日志？ {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

大多数情况下，是的。 但是，如果某个帐户在SFDC中有超过5,000个联系人，并且该帐户上的字段发生了更改，我们会同步该更改，但不会记录5,000个以上联系人的活动。

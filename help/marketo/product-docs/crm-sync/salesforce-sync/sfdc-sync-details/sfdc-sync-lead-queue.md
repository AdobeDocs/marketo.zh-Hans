---
unique-page-id: 7516241
description: 了解如何从Marketo将人员分配给Salesforce潜在客户队列。 使用将人员同步到SFDC或更改责任人流程操作进行商机分配。
title: SFDC同步 — 潜在客户队列
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%

---

# SFDC 同步：潜在客户队列 {#sfdc-sync-lead-queue}

Marketo允许您将人员添加到[[!DNL Salesforce] 潜在客户队列](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm)以帮助进行潜在客户分发。 详情如下。

## 如何在Marketo中为队列分配人员？ {#how-to-assign-a-person-to-a-queue-in-marketo}

您可以使用以下任一流操作将人员分配给[!DNL Salesforce]潜在客户队列：

* [将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>您不能在Marketo中创建或更改队列。

## 如果人员属于队列，则如何存储潜在客户所有者信息？ {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

如果潜在客户属于[!DNL Salesforce]中的队列，则这些销售所有者字段将保留为空，直到将该潜在客户分配给所有者。

* 销售负责人名字
* 销售负责人姓氏
* 销售所有者职务
* 销售负责人电话号码
* 销售负责人电子邮件地址

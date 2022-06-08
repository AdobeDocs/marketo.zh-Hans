---
unique-page-id: 7516241
description: SFDC同步 — 潜在客户队列 — Marketo文档 — 产品文档
title: SFDC同步 — 潜在客户队列
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# SFDC同步：潜在客户队列 {#sfdc-sync-lead-queue}

Marketo允许您将人员添加到 [Salesforce潜在客户队列](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) 以帮助进行潜在客户分发。 细节如下。

## 如何在Marketo中将人员分配到队列？ {#how-to-assign-a-person-to-a-queue-in-marketo}

您可以使用以下任一流程操作将人员分配给Salesforce潜在客户队列：

* [将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>无法在Marketo中创建或更改队列。

## 如果潜在客户属于队列，如何存储潜在客户所有者信息？ {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

如果Salesforce中的队列拥有潜在客户，则这些销售所有者字段将保留为空，直到将该潜在客户分配给所有者为止。

* 销售所有者名字
* 销售所有者姓氏
* 销售所有者标题
* 销售所有者电话号码
* 销售所有者电子邮件地址

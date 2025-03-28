---
unique-page-id: 7516241
description: SFDC同步 — 潜在客户队列 — Marketo文档 — 产品文档
title: SFDC同步 — 潜在客户队列
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%

---

# SFDC同步：潜在客户队列 {#sfdc-sync-lead-queue}

Marketo Engage允许您向[Salesforce潜在客户队列](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm){target="_blank"}添加人员以帮助进行潜在客户分发。 详情如下。

## 如何在Marketo中为队列分配人员？ {#how-to-assign-a-person-to-a-queue-in-marketo}

您可以使用以下任一流操作将人员分配给Salesforce潜在客户队列：

* [将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>您不能在Marketo中创建或更改队列。

## 如果人员属于队列，则如何存储潜在客户所有者信息？ {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

如果Salesforce中的某个队列拥有某个销售线索，则这些销售责任人字段将保留为空，直到将该销售线索分配给责任人。

* 销售负责人名字
* 销售负责人姓氏
* 销售所有者职务
* 销售负责人电话号码
* 销售负责人电子邮件地址

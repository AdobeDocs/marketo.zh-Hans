---
unique-page-id: 7516241
description: SFDC同步——潜在客户队列- Marketo文档——产品文档
title: SFDC同步——潜在客户队列
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# SFDC同步：潜在客户队列 {#sfdc-sync-lead-queue}

Marketo允许您向Salesforce潜在客户队 [列添加人员](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) ，以帮助进行潜在客户分发。 下面是详细信息。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

## 如何在Marketo中将人员分配到队列？ {#how-to-assign-a-person-to-a-queue-in-marketo}

您可以使用以下任一流式操作将人员分配到Salesforce潜在客户队列：

* [将人员同步到SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [更改所有者](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>不能在Marketo中创建或更改队列。

## 如果潜在客户所有者信息属于队列，如何存储该信息？ {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

如果Salesforce中的队列拥有潜在客户，则这些销售所有者字段将保持为空，直到将潜在客户分配给所有者。

* 销售所有者名字
* 销售所有者姓氏
* 销售所有者标题
* 销售所有者电话号码
* 销售所有者电子邮件地址


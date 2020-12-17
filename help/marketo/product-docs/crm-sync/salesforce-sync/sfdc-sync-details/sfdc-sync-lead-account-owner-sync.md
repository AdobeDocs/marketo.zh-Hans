---
unique-page-id: 2953463
description: SFDC Sync —— 潜在客户／帐户所有者同步- Marketo Docs —— 产品文档
title: SFDC同步——潜在客户／帐户所有者同步
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# SFDC同步：潜在客户／帐户所有者同步{#sfdc-sync-lead-account-owner-sync}

这些表在技术上正在Salesforce中同步“用户”表，但我们将其称为“潜在客户／帐户所有者”字段。

## 哪些字段将同步到Marketo?{#which-fields-will-sync-to-marketo}

对于同步到Marketo的每个人，我们还同步以下所有者字段：

* 销售所有者名字
* 销售所有者姓氏
* 销售所有者标题
* 销售所有者电话号码
* 销售所有者电子邮件地址

对于每个联系人，我们会同步上述五个潜在客户所有者字段以及这些帐户所有者字段：

* 帐户所有者名字
* 帐户所有者姓氏
* 帐户所有者电子邮件地址

## 我是否可以更改Marketo中的潜在客户所有者？{#can-i-change-the-lead-owner-in-marketo}

绝对的，只需使用[更改所有者](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)流动操作。

>[!NOTE]
>
>不能使用[使用人员详细信息页面](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)更改所有者信息。

## 我可以如何处理这些数据？{#what-can-i-do-with-this-data}

使用此数据有很多原因，如

* 发送具有销售所有者签名的个性化电子邮件
* 筛选特定销售代表以进行营销甚至分析有效性
* Marketo中的分配（和重新分配）规则
* 在[更改所有者](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)、[将人员同步到SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)和[创建任务](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)流动操作中使用它们

Marketo确实具有出色的Salesforce同步。 没有其他人做得这么好！

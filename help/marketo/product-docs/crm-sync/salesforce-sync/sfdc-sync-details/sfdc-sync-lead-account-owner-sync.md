---
unique-page-id: 2953463
description: SFDC同步 — 潜在客户/帐户所有者同步 — Marketo文档 — 产品文档
title: SFDC同步 — 潜在客户/帐户所有者同步
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# SFDC同步：潜在客户/帐户所有者同步 {#sfdc-sync-lead-account-owner-sync}

从技术上讲，这些字段正在同步Salesforce中的“用户”表，但是我们将它称为“潜在客户/帐户所有者”字段。

## 哪些字段将同步到Marketo？ {#which-fields-will-sync-to-marketo}

对于同步到Marketo的每个人，我们还会同步以下所有者字段：

* 销售所有者名字
* 销售所有者姓氏
* 销售所有者职务
* 销售负责人电话号码
* 销售负责人电子邮件地址

对于每个联系人，我们同步了以上五个潜在客户所有者字段以及以下帐户所有者字段：

* 帐户所有者名字
* 帐户所有者姓氏
* 帐户所有者电子邮件地址

## 我能否在Marketo中更改潜在客户所有者？ {#can-i-change-the-lead-owner-in-marketo}

当然，只要使用 [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md) flow操作。

>[!NOTE]
>
>不能使用更改所有者信息 [使用人员详细信息页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## 我能用这些数据做些什么？ {#what-can-i-do-with-this-data}

使用此数据的理由很多，例如

* 发送包含销售所有者签名的个性化电子邮件
* 筛选特定的销售代表以进行营销甚至分析效果
* Marketo中的分配（和重新分配）规则
* 在中使用 [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)， [将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)、和 [创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) 流操作

Marketo确实拥有出色的Salesforce同步功能。 没人能做得这么好！

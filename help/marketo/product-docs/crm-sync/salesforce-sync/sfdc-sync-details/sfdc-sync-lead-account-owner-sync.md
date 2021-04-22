---
unique-page-id: 2953463
description: SFDC同步 — 潜在客户/帐户所有者同步 — Marketo文档 — 产品文档
title: SFDC同步 — 潜在客户/帐户所有者同步
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# SFDC同步：潜在客户/帐户所有者同步{#sfdc-sync-lead-account-owner-sync}

这些表在技术上正在Salesforce中同步“用户”表，但我们将其称为潜在客户/帐户所有者字段。

## 哪些字段将同步到Marketo?{#which-fields-will-sync-to-marketo}

对于同步到Marketo的每个人，我们还同步以下所有者字段：

* 销售所有者名字
* 销售所有者姓氏
* 销售所有者标题
* 销售所有者电话号码
* 销售所有者电子邮件地址

对于每个联系人，我们会同步上述五个潜在客户所有者字段以及这些帐户所有者字段：

* 帐户所有者名
* 帐户所有者姓氏
* 帐户所有者电子邮件地址

## 我可以更改Marketo中的潜在客户所有者吗？{#can-i-change-the-lead-owner-in-marketo}

绝对，只需使用[更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)流动操作即可。

>[!NOTE]
>
>您不能使用[使用人员详细信息页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)更改所有者信息。

## 我可以使用这些数据做什么？{#what-can-i-do-with-this-data}

使用此数据有很多原因，例如

* 发送具有销售所有者签名的个性化电子邮件
* 针对特定销售代表进行筛选，以进行营销甚至分析有效性
* Marketo中的分配（和重新分配）规则
* 在[更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)、[将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)和[创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)流动操作中使用它们

Marketo绝对能实现绝佳的Salesforce同步。 没有其他人这么做！

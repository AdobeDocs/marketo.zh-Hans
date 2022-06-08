---
unique-page-id: 2953463
description: SFDC同步 — 潜在客户/帐户所有者同步 — Marketo文档 — 产品文档
title: SFDC同步 — 潜在客户/帐户所有者同步
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# SFDC同步：潜在客户/帐户所有者同步 {#sfdc-sync-lead-account-owner-sync}

从技术上讲，它们正在Salesforce中同步“用户”表，但我们将将其称为“潜在客户/帐户所有者”字段。

## 哪些字段将同步到Marketo? {#which-fields-will-sync-to-marketo}

对于同步到Marketo的每个人员，我们还会同步以下所有者字段：

* 销售所有者名字
* 销售所有者姓氏
* 销售所有者标题
* 销售所有者电话号码
* 销售所有者电子邮件地址

对于每个联系人，我们会同步上述五个潜在客户所有者字段以及这些帐户所有者字段：

* 帐户所有者名字
* 帐户所有者姓氏
* 帐户所有者电子邮件地址

## 我可以更换Marketo的主管吗？ {#can-i-change-the-lead-owner-in-marketo}

当然，只需使用 [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md) 流量操作。

>[!NOTE]
>
>您不能使用 [使用“人员详细信息”页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## 我可以使用此数据执行哪些操作？ {#what-can-i-do-with-this-data}

使用此数据有很多理由，例如

* 向销售所有者发送带有签名的个性化电子邮件
* 过滤特定销售代表以进行营销，甚至分析其有效性
* Marketo中的分配（和重新分配）规则
* 在 [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)和 [创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) 流量操作

Marketo的Salesforce同步功能非常棒。 没有人做得这么好！

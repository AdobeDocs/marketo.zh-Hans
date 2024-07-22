---
unique-page-id: 2953463
description: SFDC同步 — 潜在客户/帐户所有者同步 — Marketo文档 — 产品文档
title: SFDC同步 — 潜在客户/帐户所有者同步
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# SFDC同步：潜在客户/帐户所有者同步 {#sfdc-sync-lead-account-owner-sync}

这些字段在技术上同步了Salesforce中的“用户”表，但我们会将其称为“潜在客户/帐户所有者”字段。

## 哪些字段将同步到Marketo Engage？ {#which-fields-will-sync-to-marketo-engage}

对于已同步到Marketo的每个人员，我们还同步了以下所有者字段：

* 销售负责人名字
* 销售负责人姓氏
* 销售所有者职务
* 销售负责人电话号码
* 销售负责人电子邮件地址

对于每个联系人，我们将同步以上五个潜在客户所有者字段以及这些帐户所有者字段：

* 帐户所有者名字
* 帐户所有者姓氏
* 帐户所有者电子邮件地址

## 我可以更改Marketo中的潜在客户所有者吗？ {#can-i-change-the-lead-owner-in-marketo}

当然，只需使用[更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}流程操作即可。

>[!NOTE]
>
>您不能使用[使用人员详细信息页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}更改所有者信息。

## 我可以如何处理此数据？ {#what-can-i-do-with-this-data}

使用此数据的原因很多，例如

* 发送包含销售负责人签名的个性化电子邮件
* 筛选特定的销售代表，以进行营销甚至分析效果
* Marketo中的分配（和重新分配）规则
* 在[更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}、[将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}和[创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}流程操作中使用它们

Marketo拥有出色的Salesforce同步功能。 没有人能做得这么好！

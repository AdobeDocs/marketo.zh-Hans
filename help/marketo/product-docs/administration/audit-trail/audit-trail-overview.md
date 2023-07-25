---
unique-page-id: 11377945
description: 审核记录概述 — Marketo文档 — 产品文档
title: 审核记录概述
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# 审核记录概述 {#audit-trail-overview}

审核记录使您能够获取在Marketo实例中所做的更改的完整历史记录（六个月）。

>[!NOTE]
>
>审核记录数据历史记录从2016年9月14日开始。

![](assets/audit-trail-overview-1.png)

## 什么是审核记录 {#what-is-audit-trail}

审核记录可实时捕获在Marketo订阅中发生的操作和事件的全面列表。 它提供了一种自助式方式，用于访问长达六个月的数据历史，帮助回答以下问题：

此资源或设置发生了什么情况，谁最后更新了它？

用户X最近做了什么？

谁正在登录我们的帐户？

## 我们审核的内容 {#what-we-audit}

Marketo将审核 [创建、编辑和删除](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) 操作：

* Design Studio资产
* 所有Marketo程序
* 智能营销活动
* 列表（智能/静态）
* 用户（管理员）
* 角色和权限（管理员）
* 工作区和分区（管理员）
* 用户登录历史记录

>[!NOTE]
>
>Marketo是 _非_ 审核目前在Web Personalization、Predictive Content或Sales Insight中所做的更改。

## 审核记录组件 {#audit-trail-components}

审核记录包括三个组件。

**1) [资产审核记录](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

请参阅对特定资产执行的活动。

**2) [管理员审核记录](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

监视基于用户的详细信息。

**3) [用户登录历史记录](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

查看谁登录了您的订阅以及登录时间。 还包括失败的登录尝试。

>[!TIP]
>
>您可以使用审核记录审核的次数太多，请务必利用 [正在筛选](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)！

## 导出数据 {#exporting-data}

您只能在实例中查看30天的数据。 要获得（最多）6个月的价值，请使用导出选项。

![](assets/two.png)

>[!NOTE]
>
>**条件**
>
>**未知：** In [!DNL Webhook]，您可能会看到用户名以及列为“未知”的电子邮件。 当您在CRM中更改选择列表值时，会发生这种情况。 这些值显示在Marketo表单和登陆页中。 在CRM端执行此更新将自动草稿引用表单的登陆页面。 In [!DNL Webhook]中，我们将捕获登陆页面已草稿，但用户的名称和电子邮件将显示为“未知”，因为我们无法从CRM端捕获用户信息。

>[!MORELIKETHIS]
>
>[启用审核记录](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)

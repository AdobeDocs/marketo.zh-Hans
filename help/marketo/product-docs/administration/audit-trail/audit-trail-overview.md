---
unique-page-id: 11377945
description: 审核记录概述 — Marketo文档 — 产品文档
title: 审核跟踪概述
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# 审核跟踪概述 {#audit-trail-overview}

通过审核记录，您能够获取在Marketo实例中所做更改的完整历史记录（6个月后）。

>[!NOTE]
>
>审核跟踪数据历史可追溯到2016年9月14日。

![](assets/audit-trail-overview-1.png)

## 什么是审核跟踪 {#what-is-audit-trail}

审核记录可实时捕获在Marketo订阅内发生的操作和事件的完整列表。 它包括一种访问六个月数据历史的自助方式，可帮助回答以下问题：

此资产或设置发生了什么情况，上次更新时是谁？

用户X最近进行了哪些操作？

谁正在登录我们的帐户？

## 我们审核的内容 {#what-we-audit}

Marketo将审核 [创建、编辑和删除](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) 用于的操作：

* 设计Studio资产
* 所有Marketo计划
* 智能营销活动
* 列表（智能/静态）
* 用户（管理员）
* 角色和权限（管理员）
* 工作区和分区（管理员）
* 用户登录历史记录

>[!NOTE]
>
>Marketo _not_ 审核当前在Web个性化、预测内容或销售分析中所做的更改。

## 审核跟踪组件 {#audit-trail-components}

审核记录包含三个组件。

**1) [资产审核跟踪](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

请参阅对特定资产完成的活动。

**2) [管理员审核跟踪](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

监控基于用户的详细信息。

**3) [用户登录历史记录](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

了解谁正在登录您的订阅以及登录时间。 还包括失败的登录尝试。

>[!TIP]
>
>您可以使用审核记录审核的内容非常多，请务必利用 [筛选](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)!

## 导出数据 {#exporting-data}

您在实例中只能查看30天的数据。 要获得（最多）六个月的价值，请使用导出选项。

![](assets/two.png)

>[!NOTE]
>
>**条件**
>
>**未知：** 在审核跟踪中，您可能会看到用户名和电子邮件列为“未知”。 当您在CRM中更改选取列表值时，会发生这种情况。 这些值显示在Marketo表单和登陆页面中。 在CRM端执行此更新后，将自动起草引用表单的登陆页面。 在审核跟踪中，我们将捕获登陆页面已起草，但用户名称和电子邮件将显示为“未知”，因为我们无法从CRM端捕获用户信息。

>[!MORELIKETHIS]
>
>[启用审核跟踪](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)

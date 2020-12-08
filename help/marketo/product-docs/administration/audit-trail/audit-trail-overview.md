---
unique-page-id: 11377945
description: 审计线索概述- Marketo Docs —— 产品文档
title: 审计线索概述
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# 审计线索概述 {#audit-trail-overview}

审核跟踪使您能够获得在Marketo实例中所做更改的完整历史记录（6个月）。

>[!NOTE]
>
>审计线索数据历史从2016年9月14日开始。

![](assets/one.png)

## 什么是审核跟踪 {#what-is-audit-trail}

审核跟踪可实时捕获市场订阅中发生的操作和事件的全面列表。 它包括一种自助方式，可访问为期6个月的数据历史，以帮助回答以下问题：

此资产或设置发生了什么情况，谁上次更新了它？

X用户进行了哪些操作？

谁正在登录我们的帐户？

## 我们审计的内容 {#what-we-audit}

Marketo将审核以下 [项的创建、编辑](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail) 和删除操作：

* Design Studio资源
* 所有营销项目
* 智能活动
* 列表（智能／静态）
* 用户（管理员）
* 角色和权限（管理员）
* 工作区和分区（管理员）
* 用户登录历史记录

>[!NOTE]
>
>Marketo目前 **不** 会审核在Web Personalization、Predictive Content或Sales Insight中所做的更改。

## 审核跟踪组件 {#audit-trail-components}

审核跟踪包括三个组件。

**1)资 [产审核跟踪](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AssetAuditTrail)**

查看对特定资产的活动。

**2)管 [理审计线索](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AdminAuditTrail)**

监视基于用户的详细信息。

**3)用 [户登录历史](http://docs.marketo.com/display/DOCS/User+Login+History)**

查看哪些人登录了您的订阅，以及登录时间。 还包括失败的登录尝试。

>[!TIP]
>
>您可以使用审核跟踪进行审核，请务必利用筛选 [](http://docs.marketo.com/display/DOCS/Filtering+in+Audit+Trail)!

## 导出数据 {#exporting-data}

您只能视图实例中价值30天的数据。 要获得（最多）六个月的价值，请使用导出选项。

![](assets/two.png)

>[!NOTE]
>
>**定义**
>
>**未知：** 在审核跟踪中，您可能会看到用户的姓名和电子邮件列为“未知”。 当您在CRM中更改选择列表值时，会发生这种情况。 这些值显示在Marketo表单和登陆页中。 在CRM端执行此更新将自动起草引用表单的登陆页。 在审核跟踪中，我们将捕获登陆页已起草，但用户的姓名和电子邮件将显示为“未知”，因为我们无法从CRM端捕获用户信息。

>[!NOTE]
>
>**相关文章**
>
>* [启用审核跟踪](enable-audit-trail.md)

>




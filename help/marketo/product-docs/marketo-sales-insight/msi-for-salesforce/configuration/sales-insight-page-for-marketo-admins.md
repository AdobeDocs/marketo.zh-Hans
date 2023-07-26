---
unique-page-id: 42762409
description: 面向Marketo管理员的销售分析页面 — Marketo文档 — 产品文档
title: 面向Marketo管理员的Sales Insight页面
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# 面向Marketo管理员的Sales Insight页面 {#sales-insight-page-for-marketo-admins}

Marketo管理员在Sales Insight中具有某些权限。 了解以下内容。

## Soap API配置 {#soap-api-configuration}

这些凭据用于将您的Salesforce帐户连接到Marketo实例，以便在Salesforce中使用MSI。

![](assets/one-1.png)

## Rest API配置 {#rest-api-configuration}

这些凭据用于将您的Salesforce帐户连接到Marketo实例，以便在Salesforce中使用MSI分析功能板。

![](assets/two-1.png)

## 人员得分设置 {#person-score-settings}

* **星级**：星级表示与其他商机相比的总商机分数。
* **火焰**：火焰表示紧迫性 — 商机分数最近发生了多大变化。

默认情况下， Marketo Sales Insight使用“商机得分”字段计算星星和火焰。 但是，如果您想选择其他字段，请执行以下操作：

1. 在 **管理员** Marketo区域，单击 **销售分析**.

   ![](assets/four.png)

1. 在潜在客户评分设置下，单击 **编辑**.

   ![](assets/five.png)

1. 选择要用于星号的字段。

   ![](assets/six.png)

1. 选择要用于火焰的字段。

   ![](assets/seven.png)

1. 单击 **保存**. 重新计算销售分析将需要一些时间。 您可以稍后查看CRM以查看星星和火焰。

   ![](assets/eight.png)

   >[!TIP]
   >
   >如果您还没有自定义得分字段，请采用以下方法 [创建它们](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## 设置 {#settings}

![](assets/nine.png)

**取消订阅设置：**

您可以从以下取消订阅设置中选择无模板、标准电子邮件和操作电子邮件

* 遵循取消订阅设置
* 当收件人超过1人时，遵守取消订阅设置
* 当收件人超过5人时遵循取消订阅设置
* 忽略取消订阅设置

**启用锁定模板的功能：**

启用此功能后，MSI用户在从Salesforce发送电子邮件时将无法编辑模板

**启用RSS源：**

启用后，MSI用户可以在RSS馈送中查看其潜在客户馈送（除了Salesforce中的潜在客户馈送之外）。 只有在禁用“令牌过期”功能后，RSS馈送才能正常工作。

**令牌过期：**

可在功能管理器中控制令牌过期时间。 要启用/禁用此功能，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support). 启用后，所有Marketo令牌将在10分钟内过期。 禁用后，Marketo令牌将不会过期。

在启用令牌过期之前生成的令牌将不会具有可供验证的过期时间，因此即使当前启用了功能，它们也不会过期。

在启用令牌过期后生成的令牌的过期时间将为10分钟，因此即使在该功能被禁用后，它们仍将在10分钟后过期。

令牌行为将基于其生成时间（令牌过期功能已启用/禁用时，而不是其当前功能状态）。

---
unique-page-id: 42762409
description: 面向Marketo管理员的销售分析页面 — Marketo文档 — 产品文档
title: 面向Marketo管理员的“销售分析”页面
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# 面向Marketo管理员的“销售分析”页面 {#sales-insight-page-for-marketo-admins}

Marketo管理员在Sales Insight中具有某些权限。 了解以下内容。

## Soap API配置 {#soap-api-configuration}

这些凭据用于将您的Salesforce帐户连接到Marketo实例，以便在Salesforce中使用MSI。

![](assets/one-1.png)

## Rest API配置 {#rest-api-configuration}

这些凭据用于将您的Salesforce帐户连接到Marketo实例，以便在Salesforce中使用MSI Insights仪表板。

![](assets/two-1.png)

## 人员得分设置 {#person-score-settings}

* **星**：星星表示与其他潜在客户相比的潜在客户总分数。
* **火焰**：火焰代表紧迫性 — 商机分数最近发生了多大的变化。

默认情况下，Marketo Sales Insight使用“商机得分”字段计算星星和火焰。 但是，如果您想选择其他字段，请按照以下步骤操作：

1. 在 **管理员** Marketo区域，单击 **销售分析**.

   ![](assets/four.png)

1. 在“潜在客户评分设置”下，单击 **编辑**.

   ![](assets/five.png)

1. 选择要用于星星的字段。

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
* 当收件人超过5人时，遵守取消订阅设置
* 忽略取消订阅设置

**启用锁定模板的功能：**

启用后，MSI用户将无法在Salesforce发送电子邮件时编辑模板

**启用RSS馈送：**

启用后，MSI用户可以在RSS馈送中查看其潜在客户馈送（除了Salesforce中的潜在客户馈送之外）。 RSS馈送仅在“令牌过期”功能被禁用时才能正常工作。

**令牌过期：**

令牌过期在功能管理器中进行控制。 要启用/禁用此功能，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support). 启用后，所有Marketo令牌将在10分钟内过期。 禁用后，Marketo令牌将不会过期。

在启用令牌过期之前生成的令牌将不会具有要验证的有效期，因此即使当前启用了此功能，它们也不会过期。

启用令牌过期后生成的令牌的过期时间将为10分钟，因此即使禁用该功能，它们也仍将在10分钟后过期。

令牌行为将基于其生成时间（在启用/禁用令牌过期功能时，而不是其当前功能状态）。

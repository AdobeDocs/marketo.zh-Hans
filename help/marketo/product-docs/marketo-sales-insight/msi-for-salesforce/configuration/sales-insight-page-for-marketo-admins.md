---
unique-page-id: 42762409
description: 面向Marketo管理员的销售分析页面 — Marketo文档 — 产品文档
title: 面向Marketo管理员的Sales Insight页面
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
source-git-commit: 5812f447fbe22bee13060afae8408de7ca7384e5
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# 面向Marketo管理员的Sales Insight页面 {#sales-insight-page-for-marketo-admins}

Marketo管理员在Sales Insight中具有特定权限。 了解下面的内容。

## Soap API配置 {#soap-api-configuration}

这些凭据用于将Salesforce帐户连接到Marketo实例，以便在Salesforce中使用MSI。

![](assets/one-1.png)

## Rest API配置 {#rest-api-configuration}

这些凭据用于将Salesforce帐户连接到Marketo实例，以便在Salesforce中使用MSI分析功能板。

![](assets/two-1.png)

## 人员得分设置 {#person-score-settings}

* **星**:与其他潜在客户相比，星标表示总商机分数。
* **火焰**:火焰代表着紧迫性 — 最近一个线索的得分发生了多大变化。

默认情况下，Marketo Sales Insight使用“潜在客户分数”字段计算星星和火焰。 但是，如果您想选择不同的字段，请按以下方式操作：

1. 在 **管理员** Marketo区域，单击 **销售分析**.

   ![](assets/four.png)

1. 在“潜在客户评分设置”下，单击 **编辑**.

   ![](assets/five.png)

1. 选择要用于星的字段。

   ![](assets/six.png)

1. 选择要用于火焰的字段。

   ![](assets/seven.png)

1. 单击 **保存**. 重新计算销售分析需要一些时间。 您稍后可以检查您的CRM，看到星星和火焰。

   ![](assets/eight.png)

   >[!TIP]
   >
   >如果您还没有自定义得分字段，请参阅以下操作说明 [创建它们](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[星与火](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## 设置 {#settings}

![](assets/nine.png)

**取消订阅设置：**

您可以从以下取消订阅设置中选择无模板、标准电子邮件和操作电子邮件

* 遵循取消订阅设置
* 超过1个收件人时请遵循取消订阅设置
* 超过5个收件人时，请遵循“取消订阅设置”
* 忽略取消订阅设置

**启用锁定模板的功能：**

启用后，MSI用户在从Salesforce发送电子邮件时将无法编辑模板

**启用RSS馈送：**

启用后，MSI用户可以在RSS馈送中查看其潜在客户馈送（除了Salesforce中的潜在客户馈送之外）。 RSS馈送仅在禁用“令牌到期”功能时才能正常工作。

**令牌到期：**

令牌过期在功能管理器中进行控制。 要启用/禁用此功能，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support). 启用后，所有Marketo令牌都会在10分钟内过期。 禁用Marketo令牌后，令牌不会过期。

在启用令牌到期之前生成的令牌没有要针对其进行验证的过期时间，因此即使当前已启用该功能，它们也不会过期。

启用令牌到期后生成的令牌的过期时间将为10分钟，因此即使在禁用该功能后，这些令牌仍会在10分钟内过期。

令牌行为将基于其生成时间（当令牌到期功能处于启用/禁用状态，而不是其当前功能状态）。

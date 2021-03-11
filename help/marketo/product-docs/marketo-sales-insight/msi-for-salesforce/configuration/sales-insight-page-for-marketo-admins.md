---
unique-page-id: 42762409
description: Sales Insight Page for Marketo Admins - Marketo Docs — 产品文档
title: Marketo管理员的销售分析页面
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---


# Marketo管理员{#sales-insight-page-for-marketo-admins}的“销售分析”页

Marketo管理员在Sales Insight中具有特定权限。 了解他们的下面内容。

## Soap API配置{#soap-api-configuration}

为了在Salesforce中使用MSI，这些凭据用于将您的Salesforce帐户连接到您的Marketo实例。

![](assets/one-1.png)

## Rest API配置{#rest-api-configuration}

这些凭据用于将您的Salesforce帐户连接到您的Marketo实例，以便在Salesforce中使用MSI分析仪表板。

![](assets/two-1.png)

您可以选择在SFDC中删除Rest API凭据，并仅使用Soap API。 这将禁用“分析”仪表板

![](assets/three-1.png)

## 人员得分设置{#person-score-settings}

* **星星**:与其他潜在客户相比，星表示潜在客户总分。
* **火焰**:火焰代表着紧迫性 — 最近销售线索的得分发生了多大变化。

默认情况下，Marketo Sales Insight使用“潜在客户分数”字段来计算星形和火焰。 但是，如果您想选择其他领域，请遵循以下方法：

1. 在Marketo的&#x200B;**Admin**&#x200B;区域，单击&#x200B;**Sales Insight**。

   ![](assets/four.png)

1. 在“潜在客户评分设置”下，单击&#x200B;**编辑**。

   ![](assets/five.png)

1. 选择要用于星形的字段。

   ![](assets/six.png)

1. 选择要用于火焰的字段。

   ![](assets/seven.png)

1. 单击&#x200B;**保存**。 重新计算销售洞察需要一些时间。 您可以稍后检查您的CRM，看到星星和火焰。

   ![](assets/eight.png)

   >[!TIP]
   >
   >如果您还没有自定义得分字段，下面介绍如何[创建它们](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)。

   >[!MORELIKETHIS]
   >
   >[《星与火焰》](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## 设置{#settings}

![](assets/nine.png)

**取消订阅设置：**

您可以从以下取消订阅设置中选择“无模板”、“标准电子邮件和运营电子邮件”

* 遵守取消订阅设置
* 当超过1个收件人时，请遵守取消订阅设置
* 超过5个收件人时，请遵守取消订阅设置
* 忽略取消订阅设置

**启用锁定模板的功能：**

启用后，MSI用户将无法在从Salesforce发送电子邮件时编辑模板

**启用RSS源：**

启用后，MSI用户可以在RSS源中视图其潜在客户源（Salesforce中的潜在客户源除外）。 RSS源仅在禁用“令牌到期”功能时才能正常工作。

**令牌到期：**

令牌过期在功能管理器中控制。 要启用/禁用此功能，请联系[Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support)。 启用后，所有Marketo令牌将在10分钟内过期。 禁用后，Marketo令牌将不会过期。

在启用令牌过期之前生成的令牌将没有要验证的过期时间，因此即使当前已启用该功能，它们也不会过期。

启用令牌过期后生成的令牌的过期时间为10分钟，因此即使在禁用该功能后，它们仍将在10分钟后过期。

令牌行为将基于其生成时间（当令牌到期功能处于启用/禁用状态，而不是其当前功能状态）。

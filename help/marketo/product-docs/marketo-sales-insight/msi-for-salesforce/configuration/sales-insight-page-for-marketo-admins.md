---
unique-page-id: 42762409
description: 面向Marketo管理员的Insight销售页面 — Marketo文档 — 产品文档
title: 面向 Marketo 管理员的 Sales Insight 页面
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 1%

---

# 面向Marketo管理员的[!DNL Sales Insight]页面 {#sales-insight-page-for-marketo-admins}

Marketo管理员在[!DNL Sales Insight]中具有特定权限。 了解以下内容。

## Soap API配置 {#soap-api-configuration}

这些凭据用于将您的[!DNL Salesforce]帐户连接到Marketo实例，以便在[!DNL Salesforce]中使用MSI。

![](assets/one-1.png)

## Rest API配置 {#rest-api-configuration}

这些凭据用于将您的[!DNL Salesforce]帐户连接到Marketo实例，以便在[!DNL Salesforce]中使用MSI分析仪表板。

![](assets/two-1.png)

## 人员得分设置 {#person-score-settings}

* **[!UICONTROL Stars]**：星代表与其他潜在客户相比的潜在客户总分数。
* **[!UICONTROL Flames]**：火焰代表紧迫性 — 商机分数最近发生了多少变化。

默认情况下，[!DNL Marketo Sales Insight]使用“潜在客户得分”字段计算星星和火焰。 但是，如果您想选择其他字段，请执行以下操作：

1. 在Marketo的&#x200B;**[!UICONTROL Admin]**&#x200B;区域中，单击&#x200B;**[!UICONTROL Sales Insight]**。

   ![](assets/four.png)

1. 在[!UICONTROL Lead Scoring Settings]下，单击&#x200B;**[!UICONTROL Edit]**。

   ![](assets/five.png)

1. 选择要用于星号的字段。

   ![](assets/six.png)

1. 选择要用于火焰的字段。

   ![](assets/seven.png)

1. 单击&#x200B;**[!UICONTROL Save]**。 Sales insight将需要一些时间来重新计算。 您可以稍后查看CRM以查看星星和火焰。

   ![](assets/eight.png)

   >[!TIP]
   >
   >如果您还没有自定义得分字段，下面是如何[创建它们](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)。

   >[!MORELIKETHIS]
   >
   >[星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## 设置 {#settings}

![](assets/nine.png)

**取消订阅设置：**

您可以为[!UICONTROL No Template]、[!UICONTROL Standard Emails]和[!UICONTROL Operational emails]选择以下取消订阅设置

* [!UICONTROL Respect Unsubscribe Setting]
* [!UICONTROL Respect Unsubscribe Settings when more than 1 recipient]
* [!UICONTROL Respect Unsubscribe Settings when more than 5 recipients]
* [!UICONTROL Ignore Unsubscribe Settings]

**启用锁定模板的功能：**

启用后，MSI用户在从[!DNL Salesforce]发送电子邮件时将无法编辑模板

**启用RSS源：**

启用后，MSI用户可以在RSS馈送中查看其潜在客户馈送（除了[!DNL Salesforce]中的潜在客户馈送之外）。 只有在禁用“[!UICONTROL Token Expiration]”功能的情况下，RSS馈送才能正常工作。

**令牌过期：**

可在功能管理器中控制令牌过期时间。 要启用/禁用此功能，请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)。 启用后，所有Marketo令牌将在10分钟内过期。 禁用后，Marketo令牌将不会过期。

在启用令牌过期之前生成的令牌将不会具有可供验证的过期时间，因此即使当前启用了功能，它们也不会过期。

在启用令牌过期后生成的令牌的过期时间将为10分钟，因此即使在该功能被禁用后，它们仍将在10分钟后过期。

令牌行为将基于其生成时间（令牌过期功能已启用/禁用时，而不是其当前功能状态）。

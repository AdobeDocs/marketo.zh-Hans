---
unique-page-id: 42762409
description: Sales Insight Page for Marketo Admins - Marketo Docs —— 产品文档
title: Marketo管理员的销售分析页
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# Marketo管理员的销售分析页面{#sales-insight-page-for-marketo-admins}

Marketo管理员在Sales Insight中具有特定权限。 了解它们的下面内容。

## Soap API配置{#soap-api-configuration}

这些凭据用于将您的Salesforce帐户连接到您的Marketo实例，以便在Salesforce中使用MSI。

![](assets/one-1.png)

## Rest API配置{#rest-api-configuration}

这些凭据用于将您的Salesforce帐户连接到您的Marketo实例，以便在Salesforce中使用MSI洞察仪表板。

![](assets/two-1.png)

您可以选择在SFDC中删除Rest API凭据，并且只使用Soap API。 这将禁用“洞察”仪表板

![](assets/three-1.png)

## 人员得分设置{#person-score-settings}

| **星星：** | 与其他潜在客户相比，星表示潜在客户总分。 |
|---|---|
| **火焰：** | 火焰代表着紧迫性——最近销售线索的得分发生了多大变化。 |

默认情况下，Marketo Sales Insight使用“潜在客户得分”字段计算星形和火焰。 但是，如果您想要选择其他领域，下面介绍如何：

1. 在Marketo的&#x200B;**Admin**&#x200B;区域，单击&#x200B;**Sales Insight**。

   ![](assets/four.png)

1. 在“潜在客户评分设置”下，单击&#x200B;**编辑**。

   ![](assets/five.png)

1. 选择要用于星形的字段。

   ![](assets/six.png)

1. 选择要用于火焰的字段。

   ![](assets/seven.png)

1. 单击&#x200B;**保存**。 重新计算销售洞察需要一些时间。 您可以稍后检查您的CRM以查看星星和火焰。

   ![](assets/eight.png)

   >[!TIP]
   >
   >如果您还没有自定义得分字段，下面介绍如何[创建它们](http://docs.marketo.com/x/3wMk)。

   >[!NOTE]
   >
   >**相关文章**
   >
   >
   >[星与火](http://docs.marketo.com/x/qgU6Ag)

## 设置{#settings}

![](assets/nine.png)

**取消订阅设置：**

您可以从以下取消订阅设置中选择“无模板”、“标准电子邮件”和“运营”电子邮件

* 遵守取消订阅设置
* 超过1个收件人时，请遵守取消订阅设置
* 超过5个收件人时，请遵守取消订阅设置
* 忽略取消订阅设置

**启用锁定模板的功能：**

启用此功能后，MSI用户将无法在从Salesforce发送电子邮件时编辑模板

**启用RSS源：**

启用后，MSI用户可以在RSS源中视图其潜在客户源（除Salesforce中的潜在客户源外）**。**

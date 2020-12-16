---
unique-page-id: 2952678
description: 使用发送警报信息令牌{{SP_Send_Alert_Info}} - Marketo文档——产品文档
title: 使用发送警报信息令牌
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# 使用发送警报信息令牌 {#use-the-send-alert-info-token-sp-send-alert-info}

该 `{{SP_Send_Alert_Info}}` 令牌是为销售团队创建警报电子邮件时使用的特殊令牌。

>[!TIP]
>
>此令牌仅在通过发送警报流步骤发送包含该令牌的电子 [邮件时](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) 按预期工作。 在“发送电子邮件”流程步骤中使用时，它将不起作用。

示例警报：   ![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>注意！ 警报中的URL具有过期日期，因此应确保它们具有支持这些类型邮件的节奏。 过期日期由 [管理员进行配置](../../../../product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md)。

以下信息是以下内容的一部分 `{{SP_Send_Alert_Info}}`:

* 作为指向Marketo中人员详细信息的链接的名和姓
* 指向CRM中人员的链接
* 发送警报的Marketo中的活动名
* 发送警报的时间

>[!NOTE]
>
>只有该人员在CRM系统中（目前Dynamics CRM中不提供），才会显示指向CRM的链接。 Marketo和非Marketo用户均可访问该链接。

## 将SP_Send_Alert_Info令牌添加到电子邮件 {#add-the-sp-send-alert-info-token-to-an-email}

1. 选择电子邮件，然后单击“ **编辑草稿”**。

   ![](assets/one-3.png)

1. 多次-单击要将令牌添加到的可编辑区域。

   ![](assets/two-3.png)

1. 将光标放在您希望标记所在的位置，然后单击“插入 **令牌** ”按钮。

   ![](assets/three-3.png)

1. 查找并选择令牌， **`{{SP_Send_Alert_Info}}`** 然后单击“ **插入”**。

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. 单击 **保存**。

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>**提醒**
>
>不要忘记批准您的电子邮件。

好东西！ 此令牌非常有用，您应将其用于您为销售团队创建的所有警报。
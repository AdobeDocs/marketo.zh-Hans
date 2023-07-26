---
unique-page-id: 2952678
description: 使用发送警报信息令牌 {{SP_Send_Alert_Info}} - Marketo文档 — 产品文档
title: 使用发送警报信息令牌
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 使用发送警报信息令牌 {#use-the-send-alert-info-token-sp-send-alert-info}

此 `{{SP_Send_Alert_Info}}` 令牌是一种特殊令牌，可在为销售团队创建警报电子邮件时使用。

>[!TIP]
>
>仅当使用发送包含该令牌的电子邮件时，此令牌才会按预期工作 [发送警报](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) 流程步骤。 在“发送电子邮件”流程步骤中使用它时，它将不起作用。

示例警报：

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>抬头！ 警报中的URL具有过期日期，因此请确保它们具有支持这些类型消息的频率。 过期日期为 [由管理员配置](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

以下信息包含在 `{{SP_Send_Alert_Info}}`：

* 在Marketo中将名字和姓氏作为人员详细信息的链接
* CRM中人员的链接
* 发送警报的Marketo中的营销活动名称
* 发送警报的时间

>[!NOTE]
>
>仅当人员在CRM系统中（当前在Dynamics CRM中不可用）时，才会显示指向CRM的链接。 Marketo和非Marketo用户均可访问该链接。

## 将SP_Send_Alert_Info令牌添加到电子邮件中 {#add-the-sp-send-alert-info-token-to-an-email}

1. 选择电子邮件并单击 **编辑草稿**.

   ![](assets/one-3.png)

1. 双击要将令牌添加到的可编辑区域。

   ![](assets/two-3.png)

1. 将光标放在您希望令牌的位置，然后单击 **插入令牌** 按钮。

   ![](assets/three-3.png)

1. 查找并选择 **`{{SP_Send_Alert_Info}}`** 令牌并单击 **插入**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. 单击 **保存**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>别忘了批准您的电子邮件。

好东西！ 此令牌非常有用，您应在为销售团队创建的所有警报中使用它。

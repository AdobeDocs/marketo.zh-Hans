---
unique-page-id: 2360360
description: 创建Webhook - Marketo文档 — 产品文档
title: 创建Webhook
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 6f17d79344653d1b2c364753d774998e343c9808
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# 创建Webhook {#create-a-webhook}

使用Web挂接来利用第三方Web服务发送文本消息、扩展人员数据等。

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关详细信息，请联系您的销售代表。

1. 转到 **管理员** 单击 **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. 单击 **新Webhook**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. 命名并配置Webhook。

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >这通常包括将第三方服务凭据作为URL参数输入，或在POST模板中输入。

   * **URL**:输入在对Web服务的请求中使用的URL。 插入令牌，如人员的电子邮件地址(**`{{lead.Email Address}}`**)，在您的请求中，单击 **插入令牌**.

   * **模板**:如果要在POST正文中传输信息，请输入模板。 使用支持HTTPPOST的任何数据格式，包括XML、JSON或SOAP。 要在模板中插入令牌，请单击 **插入令牌**.

   * **请求令牌编码**:如果令牌值包含特殊字符（如与号、“&amp;”），请指示请求的格式(**JSON** 或 **表单/Url**)。

   * **响应类型**:选择您从服务收到的响应格式(**JSON** 或 **XML**)。

   * **请求类型**:选择要使用的HTTP方法(DELETE、GET、PATCH、POST、PUT)

   单击 **创建**.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>在 [Web挂钩](https://developers.marketo.com/documentation/webhooks/) 深潜。

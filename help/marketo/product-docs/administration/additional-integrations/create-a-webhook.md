---
unique-page-id: 2360360
description: 创建Webhook - Marketo Docs —— 产品文档
title: 创建Webhook
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---


# 创建Webhook {#create-a-webhook}

使用webhooks利用第三方Web服务发送文本消息、扩展人员数据等。

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关详细信息，请与销售代表联系。

1. 转至&#x200B;**Admin**&#x200B;并单击&#x200B;**Webhooks**。

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. 单击&#x200B;**新建Webhook**。

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. 命名并配置Webhook。

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >这通常包括以URL参数或POST模板的形式输入您的第三方服务凭据。

   * **URL**:输入用于POST对Web服务的请求的URL。要在您的请求中插入令牌，如人员的电子邮件地址(**`{{lead.Email Address}}`**)，请单击&#x200B;**插入令牌**。

   * **模板**:如果要在POST正文中传输信息，请输入模板。使用支持HTTPPOST的任何数据格式，包括XML、JSON或SOAP。 要在模板中插入令牌，请单击&#x200B;**插入令牌**。

   * **请求令牌编码**:如果令牌值包含特殊字符（如“&amp;”），请指示请求的格式(**** JSON或 **表单/Url**)。

   * **响应类型**:选择您从服务（JSON或XML）收到的&#x200B;**** 响应 **的格式**。

   单击创建。

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>在[webhooks](http://developers.marketo.com/documentation/webhooks/)深入了解更多信息。

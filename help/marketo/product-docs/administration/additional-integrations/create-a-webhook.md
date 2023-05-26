---
unique-page-id: 2360360
description: 创建 [!DNL Webhook] - Marketo文档 — 产品文档
title: 创建 [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 1f10e1fcdbd5cf91481f749236fd37050ade29f8
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---

# 创建 [!DNL Webhook] {#create-a-webhook}

使用 [!DNL Webhooks] 利用第三方Web服务发送短信、扩展人员数据等。

>[!AVAILABILITY]
>
>并非所有客户都已购买此功能。 有关详细信息，请与您的销售代表联系。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/create-a-webhook-1.png)

1. 单击 **[!UICONTROL Webhook]**.

   ![](assets/create-a-webhook-2.png)

1. 单击 **[!UICONTROL 新建Webhook]**.

   ![](assets/create-a-webhook-3.png)

1. 命名并配置您的 [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >这通常包括在URL参数或POST模板中输入您的第三方服务凭据。

   * **[!UICONTROL URL]**：输入在对Web服务的请求中使用的URL。 插入令牌，如人员的电子邮件地址(**`{{lead.Email Address}}`**)，在您的请求中，单击 **[!UICONTROL 插入令牌]**.

   * **[!UICONTROL 模板]**：如果您希望在请求正文中传输信息，请通过有效负载模板输入。 允许用于以下请求类型的模板：POST、DELETE、PATCH或PUT。 您可以使用数据格式，如JSON或XML。 要在模板中插入令牌，请单击 **[!UICONTROL 插入令牌]**.

   * **[!UICONTROL 请求令牌编码]**：如果令牌值包含特殊字符（例如&amp;符号），请指示请求的格式(**JSON** 或 **表单/URL**)。

   * **[!UICONTROL 响应类型]**：选择您从服务收到的响应的格式(**JSON** 或 **XML**)。

   * **[!UICONTROL 请求类型]**：选择要使用的HTTP方法(DELETE、GET、PATCH、POST、PUT)。

1. 单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>了解详情，请参阅 [[!DNL Webhooks]](https://developers.marketo.com/documentation/webhooks/){target="_blank"} 深潜。

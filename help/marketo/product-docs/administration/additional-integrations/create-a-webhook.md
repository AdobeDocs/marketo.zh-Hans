---
unique-page-id: 2360360
description: 在管理员中创建webhook，以调用短信、人员数据等第三方Web服务。
title: 创建 [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
TQID: https://experienceleague.adobe.com/O4xw1wSvFeTJ2xqZn4Eo7JbrUBQQmKcl7mvLkduFXGc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: fc9b09fe-b844-4544-887b-e420c3b82065
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 202
ht-degree: 3%

---

# 创建[!DNL Webhook] {#create-a-webhook}

使用[!DNL Webhooks]利用第三方Web服务发送短信、扩展人员数据等。

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/create-a-webhook-1.png)

1. 单击 **[!UICONTROL Webhooks]**。

   ![](assets/create-a-webhook-2.png)

1. 单击 **[!UICONTROL New Webhook]**。

   ![](assets/create-a-webhook-3.png)

1. 命名并配置您的[!DNL Webhook]。

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >这通常包括在URL参数或POST模板中输入您的第三方服务凭据。

   * **[!UICONTROL URL]**：输入在对Web服务的请求中使用的URL。 要在您的请求中插入令牌，如人员的电子邮件地址(**`{{lead.Email Address}}`**)，请单击&#x200B;**[!UICONTROL Insert Token]**。

   * **[!UICONTROL Template]**：如果要在请求正文中传输信息，请通过有效负荷模板输入。 允许用于以下请求类型的模板：POST、DELETE、PATCH或PUT。 您可以使用数据格式，如JSON或XML。 要在模板中插入令牌，请单击&#x200B;**[!UICONTROL Insert Token]**。

   * **[!UICONTROL Request Token Encoding]**：如果令牌值包含特殊字符（例如&amp;符号），请指示您的请求格式（**JSON**&#x200B;或&#x200B;**表单/URL**）。

   * **[!UICONTROL Response type]**：选择您从服务收到的响应的格式（**JSON**&#x200B;或&#x200B;**XML**）。

   * **[!UICONTROL Request Type]**：选择要使用的HTTP方法(DELETE、GET、PATCH、POST、PUT)。

1. 单击 **[!UICONTROL Create]**。

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>在[[!DNL Webhooks]](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}深入了解中了解详情。

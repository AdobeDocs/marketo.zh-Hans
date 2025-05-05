---
unique-page-id: 2360350
description: 创建用于ReST API的自定义服务 — Marketo文档 — 产品文档
title: 创建用于ReST API的自定义服务
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# 创建用于ReST API的自定义服务 {#create-a-custom-service-for-use-with-rest-api}

如果您要通过ReST API与Marketo集成，则需要创建自定义服务。 具体方法如下。

>[!PREREQUISITES]
>
>* [创建仅API用户角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [创建仅API用户](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>

>[!NOTE]
>
>**需要管理员权限**

>[!TIP]
>
>有关[REST API](https://developer.adobe.com/marketo-apis/)的详细信息，请查看我们的开发人员文档。 如果您需要，我们还有[SOAP API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/soap/soap-api)。

## 创建自定义服务 {#create-custom-service}

1. 转到&#x200B;**[!UICONTROL 管理员]**&#x200B;区域。

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. 单击&#x200B;**启动点**。

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. 选择&#x200B;**[!UICONTROL 新建]**，然后选择&#x200B;**[!UICONTROL 新建服务]**。

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. 输入服务的&#x200B;**[!UICONTROL 显示名称]**。 选择&#x200B;**[!UICONTROL 仅API用户]** [之前创建的](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)。

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >请注意，我们已经对常见网络研讨会服务进行了本机集成。

1. 单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   哦，太好了！ 服务现已创建，让我们继续获取所有凭据以提供访问权限。

## 用于访问API的凭据 {#credentials-for-api-access}

1. 转到&#x200B;**[!UICONTROL 管理员]**&#x200B;区域。

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. 单击&#x200B;**[!UICONTROL 启动点]**。

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. 单击上面创建的自定义[!UICONTROL LaunchPoint]服务的&#x200B;**[!UICONTROL 查看详细信息]**。

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. 单击&#x200B;**[!UICONTROL 获取令牌]**。

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. 向负责建立连接的人提供&#x200B;**[!UICONTROL 客户端ID]**、**[!UICONTROL 客户端密钥]**、**[!UICONTROL 授权用户]**&#x200B;和&#x200B;**[!UICONTROL 令牌]**。

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>不要共享此信息；这是您数据的后门。 保持安全！

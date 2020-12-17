---
unique-page-id: 2360350
description: 创建用于ReST API - Marketo Docs —— 产品文档的自定义服务
title: 创建与ReST API一起使用的自定义服务
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# 创建用于ReST API {#create-a-custom-service-for-use-with-rest-api}的自定义服务

如果要通过ReST API与Marketo集成，您将需要创建自定义服务。 这是方法。

>[!PREREQUISITES]
>
>* [创建仅API用户角色](../../../product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [创建仅API用户](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md)

>



>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>**深潜**
>
>请查看我们的开发人员文档，了解有关[ReST API](http://developers.marketo.com/documentation/rest/)的详细信息。 如果您需要[SOAP API](http://developers.marketo.com/documentation/soap/)，我们还有&lt;a0/>SOAP API&lt;a1/>。

>[!NOTE]
>
>如果您拥有Spark级别的Marketo，则无法创建自定义服务。

## 创建自定义服务{#create-custom-service}

1. 转至&#x200B;**Admin**&#x200B;并单击&#x200B;**LaunchPoint**。

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. 在&#x200B;**新建**&#x200B;下，单击&#x200B;**新建服务**。

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. 输入服务的&#x200B;**显示名称**。 选择“仅API用户&#x200B;****”。[](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md)

   >[!NOTE]
   >
   >**提醒**
   >
   >请注意，我们已经为流行的网络研讨会服务集成了本机功能。

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. 单击&#x200B;**创建**。

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   哦，耶！ 该服务现已创建，我们继续获取要提供访问的所有凭据。

## API访问{#credentials-for-api-access}的凭据

1. 转至&#x200B;**Admin**&#x200B;并单击&#x200B;**LaunchPoint**。

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. 单击&#x200B;**视图详细信息**，查看上面创建的自定义LaunchPoint服务。

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. 单击&#x200B;**获取令牌**。

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. 向负责建立连接的人员提供**客户端Id**、**客户端机密**、**授权用户**&#x200B;和&#x200B;**令牌**。

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>不要共享此信息；这是你数据的后门。 保证安全！


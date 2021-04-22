---
unique-page-id: 2360350
description: 创建与ReST API - Marketo Docs — 产品文档一起使用的自定义服务
title: 创建与ReST API一起使用的自定义服务
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# 创建用于ReST API {#create-a-custom-service-for-use-with-rest-api}的自定义服务

如果要通过ReST API与Marketo集成，您将需要创建自定义服务。 下面介绍如何操作。

>[!PREREQUISITES]
>
>* [创建仅API用户角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [创建仅API用户](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)

>



>[!NOTE]
>
>**需要管理权限**

>[!TIP]
>
>请查阅我们的开发人员文档，了解有关[ReST API](https://developers.marketo.com/documentation/rest/)的详细信息。 如果您需要[SOAP API](https://developers.marketo.com/documentation/soap/)，则我们还有。

>[!NOTE]
>
>如果您的Spark级别为Marketo，则无法创建自定义服务。

## 创建自定义服务{#create-custom-service}

1. 转至&#x200B;**Admin**&#x200B;并单击&#x200B;**LaunchPoint**。

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. 在&#x200B;**新建**&#x200B;下，单击&#x200B;**新建服务**。

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. 输入服务的&#x200B;**显示名称**。 选择&#x200B;**仅API用户** [之前创建的](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)。

   >[!NOTE]
   >
   >请注意，我们已经为流行的网络研讨会服务集成了本机功能。

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. 单击&#x200B;**创建**。

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   哦耶！ 该服务现已创建，让我们继续并获取所有凭据以供访问。

## API访问{#credentials-for-api-access}的凭据

1. 转至&#x200B;**Admin**&#x200B;并单击&#x200B;**LaunchPoint**。

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. 单击&#x200B;**视图详细信息**&#x200B;以获取上述创建的自定义LaunchPoint服务。

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. 单击&#x200B;**获取令牌**。

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. 将&#x200B;**客户端Id**、**客户端机密**、**授权用户**&#x200B;和&#x200B;**令牌**&#x200B;提供给负责建立连接的人。

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>请勿共享此信息；这是数据的后门。 保持安全！

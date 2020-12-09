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


# 创建与ReST API一起使用的自定义服务 {#create-a-custom-service-for-use-with-rest-api}

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
>有关ReST API的详细信息，请查阅我们的 [开发人员文档](http://developers.marketo.com/documentation/rest/)。 如果您需 [要SOAP](http://developers.marketo.com/documentation/soap/) API，我们也有它。

>[!NOTE]
>
>如果您拥有Spark级别的Marketo，则无法创建自定义服务。

## 创建自定义服务 {#create-custom-service}

1. 转到“管 **理员** ”并单 **击LaunchPoint**。

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. 在“ **新建**”下，单 **击“新建服务**”。

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. 输入服 **务的显** 示名称。 选择以 **前创建的仅**[限API用户](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md)。

   >[!NOTE]
   >
   >**提醒**
   >
   >请注意，我们已经为流行的网络研讨会服务集成了本机功能。

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. 单击 **创建**。

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   哦，耶！ 该服务现已创建，我们继续获取要提供访问的所有凭据。

## API访问凭据 {#credentials-for-api-access}

1. 转到“管 **理员** ”并单 **击LaunchPoint**。

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. 单击 **视图** “详细信息”，查看上面创建的自定义LaunchPoint服务。

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. 单击 **获取令牌**。

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. 为负责建立连接的人员提 **供**客**&#x200B;户端 **ID****、 **客户端机密** 、授权用户和令牌。

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>不要共享此信息；这是你数据的后门。 保证安全！


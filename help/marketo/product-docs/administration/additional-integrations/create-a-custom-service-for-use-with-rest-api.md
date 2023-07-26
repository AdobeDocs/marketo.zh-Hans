---
unique-page-id: 2360350
description: 创建用于ReST API的自定义服务 — Marketo文档 — 产品文档
title: 创建用于ReST API的自定义服务
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '213'
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
>有关更多详细信息，请参阅我们的开发人员文档 [重设API](https://developers.marketo.com/documentation/rest/). 我们还有 [SOAP API](https://developers.marketo.com/documentation/soap/) 如果这是你所需要的。

## 创建自定义服务 {#create-custom-service}

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. 单击 **启动点**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. 选择 **[!UICONTROL 新建]** 然后 **[!UICONTROL 新建服务]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. 输入 **[!UICONTROL 显示名称]** 为这项服务。 选择 **[!UICONTROL 仅API用户]** [之前已创建](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >请注意，我们已经对常见网络研讨会服务进行了本机集成。

1. 单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   哦，太好了！ 服务现已创建，让我们继续获取所有凭据以提供访问权限。

## 用于访问API的凭据 {#credentials-for-api-access}

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. 单击 **[!UICONTROL 启动点]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. 单击 **[!UICONTROL 查看详细信息]** 对于自定义 [!UICONTROL 启动点] 服务创建于上面。

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. 单击 **[!UICONTROL 获取令牌]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. 提供 **[!UICONTROL 客户端ID]**， **[!UICONTROL 客户端密码]**， **[!UICONTROL 授权用户]**、和 **[!UICONTROL 令牌]** 负责建立连接的人员。

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>不要共享此信息；这是您数据的后门。 保持安全！

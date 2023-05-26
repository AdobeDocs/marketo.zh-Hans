---
unique-page-id: 15695874
description: '"Connect [!DNL BrightTALK] Marketo - Marketo文档 — 产品文档”'
title: '"Connect [!DNL BrightTALK] 到Marketo”'
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
source-git-commit: 1f10e1fcdbd5cf91481f749236fd37050ade29f8
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 1%

---

# Connect [!DNL BrightTALK] 到Marketo {#connect-brighttalk-to-marketo}

了解如何连接 [!DNL BrightTALK] 渠道到您的Marketo实例。 为此，您必须是两者的管理员。

>[!NOTE]
>
>**需要管理员权限**

## 中的步骤 [!DNL BrightTALK] {#steps-in-brighttalk}

1. 登录 [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"} 并单击 **[!UICONTROL 立即连接]**.
1. 下 [!UICONTROL 高级Marketo连接器]，单击 **[!UICONTROL Connect]**.
1. 您将进入“凭据”屏幕，询问：客户端ID、客户端密钥、身份服务URL和Rest服务URL。 要获取此信息，请登录Marketo。

## Marketo中的步骤 {#steps-in-marketo}

>[!NOTE]
>
>此时，您需要设置 [!DNL API Only User Role] 和 [!DNL API User] 以限制哪些权限 [!DNL BrightTALK] 将在您的Marketo实例中具有。 由于我们已经提供了有关这些步骤的文章，因此我们将为您链接这些文章。

1. 创建 [仅API用户角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}.

1. [创建API用户](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"}，使用 [!DNL BrightTALK] 您在步骤4中创建的API角色。

1. 返回至 **[!UICONTROL 管理员]** 区域。

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. 下 **[!UICONTROL 集成]**，单击 **[!UICONTROL 启动点]**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. 单击 **[!UICONTROL 新]** 下拉菜单并选择 **[!UICONTROL 新服务]**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. 输入 **[!UICONTROL 显示名称]** 你自己选择的。 单击 **[!UICONTROL 服务]** 下拉菜单并选择 **[!UICONTROL 自定义]** (do _非_ 选择 [!DNL BrightTALK])。

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >切记不要选择 [!DNL BrightTALK] 下拉列表中的每个字段。 该字段我们正在删除中，选择该字段可能会导致与您的相关的重大问题 [!DNL Marketo/BrightTALK] 集成。

1. 输入 [!UICONTROL 描述] 你自己选择的。 单击 **[!UICONTROL 仅API用户]** 下拉菜单并选择 [!DNL BrightTALK API User] 您在步骤5中创建的。 单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. 单击 **[!UICONTROL 查看详细信息]** 用于您刚刚创建的自定义服务。

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. 复制（并保存） **[!UICONTROL 客户端ID]** 和 **[!UICONTROL 客户端密码]**. 单击&#x200B;**[!UICONTROL 关闭]**。

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. 下 **[!UICONTROL 集成]**，选择 **[!UICONTROL Web服务]**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. 下 **[!UICONTROL Rest API]**，复制（并保存） **[!UICONTROL 端点]** 和 **[!UICONTROL 身份]**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## 中的其他步骤 [!DNL BrightTALK] {#additional-steps-in-brighttalk}

1. 返回到 [!DNL BrightTALK] 步骤3中的连接器设置屏幕，然后输入您在步骤12和14中保存的凭据。

在凭据进行身份验证后，您已正式连接 [!DNL BrightTALK] Marketo。 下一步是确定 [要同步哪些数据字段](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target="_blank"}.

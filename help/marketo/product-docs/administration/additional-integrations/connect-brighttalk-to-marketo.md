---
unique-page-id: 15695874
description: "将 [!DNL BrightTALK] 连接到Marketo - Marketo文档 — 产品文档"
title: “连接 [!DNL BrightTALK] 到Marketo”
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
feature: Administration, Integrations
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 将[!DNL BrightTALK]连接到Marketo {#connect-brighttalk-to-marketo}

了解如何将您的[!DNL BrightTALK]渠道连接到Marketo实例。 为此，您必须是两者的管理员。

>[!NOTE]
>
>**需要管理员权限**

## [!DNL BrightTALK]中的步骤 {#steps-in-brighttalk}

1. 登录到[business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"}，然后单击&#x200B;**[!UICONTROL 立即连接]**。
1. 在[!UICONTROL 高级Marketo连接器]下，单击&#x200B;**[!UICONTROL 连接]**。
1. 您将进入“凭据”屏幕，询问：客户端ID、客户端密钥、标识服务URL和Rest服务URL。 要获取此信息，请登录Marketo。

## Marketo的步骤 {#steps-in-marketo}

>[!NOTE]
>
>此时，您需要设置[!DNL API Only User Role]和[!DNL API User]，以限制[!DNL BrightTALK]在您的Marketo实例中拥有的权限。 由于我们已经提供了有关这些步骤的文章，因此我们将为您链接这些文章。

1. 创建[仅API用户角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}。

1. [使用您在步骤4中创建的[!DNL BrightTALK] API角色创建API用户](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"}。

1. 返回&#x200B;**[!UICONTROL 管理员]**&#x200B;区域。

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. 在&#x200B;**[!UICONTROL 集成]**&#x200B;下，单击&#x200B;**[!UICONTROL LaunchPoint]**。

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. 单击&#x200B;**[!UICONTROL 新建]**&#x200B;下拉列表并选择&#x200B;**[!UICONTROL 新建服务]**。

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. 输入您选择的&#x200B;**[!UICONTROL 显示名称]**。 单击&#x200B;**[!UICONTROL 服务]**&#x200B;下拉列表并选择&#x200B;**[!UICONTROL 自定义]** （请&#x200B;_不_&#x200B;选择[!DNL BrightTALK]）。

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >切记不要在下拉列表中选择[!DNL BrightTALK]。 该字段我们正在删除中，选择该字段可能会导致您的[!DNL Marketo/BrightTALK]集成存在重大问题。

1. 输入您选择的[!UICONTROL 描述]。 单击&#x200B;**[!UICONTROL 仅API用户]**&#x200B;下拉列表，然后选择您在步骤5中创建的[!DNL BrightTALK API User]。 单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. 单击刚刚创建的自定义服务的&#x200B;**[!UICONTROL 查看详细信息]**。

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. 复制（并保存）客户端ID **[!UICONTROL 和客户端密钥****。]**&#x200B;单击&#x200B;**[!UICONTROL 关闭]**。

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. 在&#x200B;**[!UICONTROL 集成]**&#x200B;下，选择&#x200B;**[!UICONTROL Web服务]**。

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. 在&#x200B;**[!UICONTROL Rest API]**&#x200B;下，复制（并保存）终结点&#x200B;**[!UICONTROL 和**[!UICONTROL &#x200B;标识&#x200B;]**。]**

   ![](assets/connect-brighttalk-to-marketo-9.png)

## [!DNL BrightTALK]中的其他步骤 {#additional-steps-in-brighttalk}

1. 从步骤3返回到[!DNL BrightTALK]连接器设置屏幕，并输入您在步骤12和14中保存的凭据。

凭据通过身份验证后，您已正式将[!DNL BrightTALK]连接到Marketo。 下一步是确定[要同步的数据字段](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target="_blank"}。

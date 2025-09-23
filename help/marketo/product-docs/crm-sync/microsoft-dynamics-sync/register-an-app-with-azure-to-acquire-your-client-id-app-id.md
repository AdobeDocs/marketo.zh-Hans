---
unique-page-id: 12983390
description: 在Azure中注册应用程序以获取客户端ID/应用程序ID - Marketo文档 — 产品文档
title: 在 Azure 上注册应用程序以获取客户端 ID/应用程序 ID
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 8%

---

# 在 Azure 上注册应用程序以获取客户端 ID/应用程序 ID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory将您的本地目录扩展到云中，为具有本地ADFS身份验证的[!DNL MS Dynamics 365] CRM提供支持。

## 注册新应用程序 {#registering-a-new-app}

1. [使用具有管理员权限的帐户登录](https://login.microsoftonline.com/){target="_blank"}到Microsoft Azure管理门户。 您还可以通过展开左侧导航窗格中的&#x200B;**[!UICONTROL Admin]**&#x200B;项并选择&#x200B;**[!UICONTROL Azure AD]**，通过Office 365管理中心访问Microsoft Azure门户。

   >[!CAUTION]
   >
   >您必须在与要注册应用程序的[!DNL Office 365]订阅相同的订阅中使用帐户。

   >[!NOTE]
   >
   >如果你没有Azure帐户，你可以[注册](https://azure.microsoft.com/en-us/free/){target="_blank"}一个。 请参阅Microsoft文档或联系Microsoft代表以获取更多信息。 创建Azure帐户后，可以使用下面列出的过程注册一个或多个应用程序。
   >
   >
   >如果您有Azure帐户，但您的[!DNL Office 365]与[!DNL Microsoft Dynamics 365]的订阅在您的Azure订阅中不可用，请按照[这些说明](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"}关联这两个帐户。

1. 在左侧导航窗格中查找并单击&#x200B;**[!UICONTROL Azure Active Directory]**。

   ![](assets/two.png)

1. 在[!UICONTROL Manage]下，单击&#x200B;**[!UICONTROL App registrations]**。

   ![](assets/three.png)

1. 单击页面顶部的&#x200B;**[!UICONTROL New registration]**。

   ![](assets/four.png)

1. 输入应用程序的名称，选择适用的帐户类型，然后输入重定向URL。 然后单击页面底部的&#x200B;**[!UICONTROL Register]**。

   ![](assets/five.png)

1. 您现在应会在&#x200B;**[!UICONTROL App registrations]**&#x200B;选项卡中看到您的应用程序。

   ![](assets/six.png)

## 配置应用程序权限 {#configuring-app-permissions}

1. 在Active Directory的&#x200B;**[!UICONTROL App registrations]**&#x200B;选项卡下，单击要为其配置权限的应用程序。

   ![](assets/seven.png)

1. 在[!UICONTROL Manage]下，单击&#x200B;**[!UICONTROL API permissions]**。

   ![](assets/eight.png)

1. 单击&#x200B;**[!UICONTROL Add a permission]**&#x200B;按钮。

   ![](assets/nine.png)

1. 选择&#x200B;**[!UICONTROL Dynamics CRM]**。

   ![](assets/ten.png)

1. 选中&#x200B;**[!UICONTROL Access Common Data Service as organization users]**&#x200B;框，然后单击&#x200B;**[!UICONTROL Add permissions].**

   ![](assets/eleven.png)

1. 成功添加权限后，请至少等待10秒。

   ![](assets/twelve.png)

1. 单击&#x200B;**[!UICONTROL Grant admin consent]**&#x200B;按钮。

   ![](assets/thirteen.png)

1. 单击&#x200B;**[!UICONTROL Yes]**&#x200B;确认。

   ![](assets/fourteen.png)

   你完蛋了！

   ![](assets/fifteen.png)

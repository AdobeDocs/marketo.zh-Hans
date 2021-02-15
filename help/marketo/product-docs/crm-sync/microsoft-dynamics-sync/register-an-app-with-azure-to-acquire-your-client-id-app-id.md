---
unique-page-id: 12983390
description: 向Azure注册应用程序以获取您的客户端ID/应用程序ID - Marketo Docs — 产品文档
title: 向Azure注册应用程序以获取您的客户端ID/应用程序ID
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# 向Azure注册应用程序以获取您的客户端ID/应用程序ID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory将您的本地目录扩展到云中，提供对MS Dynamics 365 CRM的支持，并提供本地ADFS身份验证。

## 注册新应用程序{#registering-a-new-app}

1. [使](https://manage.windowsazure.com/) 用具有管理员权限的帐户登录到Microsoft Azure管理门户。您还可以通过Office 365管理中心访问Microsoft Azure门户，方法是展开左侧导航窗格中的&#x200B;**Admin**&#x200B;项并选择&#x200B;**Azure AD**。

   >[!CAUTION]
   >
   >您必须在与要向其注册应用程序的订阅相同的Office 365中使用帐户。

   >[!NOTE]
   >
   >如果您没有Azure帐户，则可以[注册](https://azure.microsoft.com/en-us/free/)。 有关详细信息，请参阅Microsoft的文档或联系Microsoft代表。 创建Azure帐户后，您可以使用下面概述的步骤注册一个或多个应用程序。
   >
   >
   >如果您有Azure帐户，但Microsoft Dynamics 365的Office 365订阅在您的Azure订阅中不可用，请按照[这些说明](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription)关联这两个帐户。

1. 在左侧导航窗格中查找并单击&#x200B;**Azure Active Directory**。

   ![](assets/two.png)

1. 在“管理”下，单击&#x200B;**应用程序注册**。

   ![](assets/three.png)

1. 单击页面顶部的&#x200B;**新建注册**。

   ![](assets/four.png)

1. 输入应用程序的名称，选择您的适用帐户类型，然后输入重定向URL。 然后，单击页面底部的&#x200B;**注册**。

   ![](assets/five.png)

1. 您现在应该可以在&#x200B;**应用程序注册**&#x200B;选项卡中看到您的应用程序。

   ![](assets/six.png)

## 配置应用程序权限{#configuring-app-permissions}

1. 在Active Directory的&#x200B;**应用程序注册**&#x200B;选项卡下，单击要配置权限的应用程序。

   ![](assets/seven.png)

1. 在“管理”下，单击&#x200B;**API权限**。

   ![](assets/eight.png)

1. 单击&#x200B;**添加权限**&#x200B;按钮。

   ![](assets/nine.png)

1. 选择&#x200B;**Dynamics CRM**。

   ![](assets/ten.png)

1. 选中&#x200B;**以组织用户身份访问公用数据服务***s**&#x200B;框，然后单击&#x200B;**添加权限。**

   ![](assets/eleven.png)

1. 成功添加权限后，请至少等待10秒。

   ![](assets/twelve.png)

1. 单击&#x200B;**授予管理员同意**&#x200B;按钮。

   ![](assets/thirteen.png)

1. 单击&#x200B;**是**&#x200B;进行确认。

   ![](assets/fourteen.png)

   你完了！

   ![](assets/fifteen.png)


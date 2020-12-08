---
unique-page-id: 12983390
description: 向Azure注册应用程序以获取您的客户端ID/应用程序ID - Marketo Docs —— 产品文档
title: 向Azure注册应用程序以获取您的客户端ID/应用程序ID
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# 向Azure注册应用程序以获取您的客户端ID/应用程序ID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory将您的本地目录扩展到云中，提供对MS Dynamics 365 CRM的支持，并提供内部部署ADFS身份验证。

## 注册新应用程序 {#registering-a-new-app}

1. [使用具有管理](http://manage.windowsazure.com/) 员权限的帐户登录到Microsoft Azure管理门户。 您还可以通过Office 365管理中心访问Microsoft Azure门户，方法是展开左侧导航窗格 **中的** Admin项并选择 **Azure AD**。

   >[!CAUTION]
   >
   >您必须在与要注册应用程序的订阅相同的Office 365中使用帐户。

   >[!NOTE]
   >
   >如果您没有Azure帐户，则可 [注册](https://azure.microsoft.com/en-us/free/) 一个。 请参阅Microsoft的文档或联系您的Microsoft代表以了解更多信息。 创建Azure帐户后，您可以按照下面所述的步骤注册一个或多个应用程序。
   >
   >
   >如果您有Azure帐户，但您的Office 365订阅和Microsoft Dynamics 365在您的Azure订阅中不可用，请按照以 [下说明](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription) ，关联这两个帐户。

1. 在左侧导航窗 **格中查找并** 单击“Azure Active Directory”。

   ![](assets/two.png)

1. 在“管理”下，单击“ **应用程序注册**”。

   ![](assets/three.png)

1. 单击页面顶部的**新建注册**。

   ![](assets/four.png)

1. 输入应用程序的名称，选择适用的帐户类型，然后输入重定向URL。 然后，单 **击页** 面底部的“注册”。

   ![](assets/five.png)

1. 您现在应该会在“应用程序注册”选 **项卡中看到您** 的应用程序。

   ![](assets/six.png)

## 配置应用程序权限 {#configuring-app-permissions}

1. 在Active Directory **的** “应用程序注册”选项卡下，单击要配置权限的应用程序。

   ![](assets/seven.png)

1. 在“管理”下，单 **击“API权限**”。

   ![](assets/eight.png)

1. 单击“ **添加权限** ”按钮。

   ![](assets/nine.png)

1. 选 **择Dynamics CRM**。

   ![](assets/ten.png)

1. 选中以 **组织用户身份访问公用数据服务***s框** ，然后单击添 **加权限。**

   ![](assets/eleven.png)

1. 成功添加权限后，请至少等待10秒。

   ![](assets/twelve.png)

1. 单击“授 **予管理员同意** ”按钮。

   ![](assets/thirteen.png)

1. 单击 **是** ，确认。

   ![](assets/fourteen.png)

   你完了！

   ![](assets/fifteen.png)


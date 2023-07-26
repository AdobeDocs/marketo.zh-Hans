---
unique-page-id: 12983390
description: 在Azure中注册应用程序以获取客户端ID/应用程序ID - Marketo文档 — 产品文档
title: 在Azure中注册应用程序以获取您的客户端ID/应用程序ID
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 在Azure中注册应用程序以获取您的客户端ID/应用程序ID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory将您的本地目录扩展到云中，从而支持具有本地ADFS身份验证的MS Dynamics 365 CRM。

## 注册新应用程序 {#registering-a-new-app}

1. [登录](https://login.microsoftonline.com/){target="_blank"} 使用具有管理员权限的帐户访问Microsoft Azure管理门户。 您还可以通过Office 365管理中心访问Microsoft Azure门户，方法是展开 **管理员** 项，然后选择 **Azure AD**.

   >[!CAUTION]
   >
   >必须在您打算在其中注册应用程序的同一个Office 365订阅中使用帐户。

   >[!NOTE]
   >
   >如果你没有Azure帐户，你可以 [注册](https://azure.microsoft.com/en-us/free/){target="_blank"} 就一个。 请参阅Microsoft文档或联系Microsoft代表以获取更多信息。 创建Azure帐户后，可以使用下面列出的过程注册一个或多个应用程序。
   >
   >
   >如果您拥有Azure帐户，但您的Office 365与Microsoft Dynamics 365的订阅在Azure订阅中不可用，请遵循 [这些说明](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"} 以关联这两个帐户。

1. 查找并单击 **Azure活动目录** 在左侧导航窗格中。

   ![](assets/two.png)

1. 在管理下，单击 **应用程序注册**.

   ![](assets/three.png)

1. 单击 **新注册** 页面顶部的。

   ![](assets/four.png)

1. 输入应用程序的名称，选择适用的帐户类型，然后输入重定向URL。 然后单击 **注册** 在页面底部。

   ![](assets/five.png)

1. 现在，您应会在以下位置看到您的应用程序： **应用程序注册** 选项卡。

   ![](assets/six.png)

## 配置应用程序权限 {#configuring-app-permissions}

1. 在 **应用程序注册** 选项卡，单击要为其配置权限的应用程序。

   ![](assets/seven.png)

1. 在管理下，单击 **API权限**.

   ![](assets/eight.png)

1. 单击 **添加权限** 按钮。

   ![](assets/nine.png)

1. 选择 **Dynamics CRM**.

   ![](assets/ten.png)

1. 查看 **以组织用户的身份访问Common **** Service** 框，然后单击 **添加权限。**

   ![](assets/eleven.png)

1. 成功添加权限后，请至少等待10秒。

   ![](assets/twelve.png)

1. 单击 **授予管理员同意** 按钮。

   ![](assets/thirteen.png)

1. 单击 **是** 以确认。

   ![](assets/fourteen.png)

   你完蛋了！

   ![](assets/fifteen.png)

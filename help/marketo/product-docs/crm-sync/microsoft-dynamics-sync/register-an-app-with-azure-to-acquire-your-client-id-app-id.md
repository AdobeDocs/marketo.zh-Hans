---
unique-page-id: 12983390
description: 在Azure中注册应用程序以获取您的客户端ID/应用程序ID - Marketo文档 — 产品文档
title: 在Azure中注册应用程序以获取您的客户端ID/应用程序ID
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
source-git-commit: 6f15abf1fed69431b3bbe249c908b0f90a56d391
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# 在Azure中注册应用程序以获取您的客户端ID/应用程序ID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory将您的本地目录扩展到云中，为MS Dynamics 365 CRM提供内部部署ADFS身份验证支持。

## 注册新应用程序 {#registering-a-new-app}

1. [登录](https://login.microsoftonline.com/){target=&quot;_blank&quot;}使用具有管理员权限的帐户到Microsoft Azure管理门户。 您还可以通过Office 365管理中心，通过扩展 **管理员** 项目，然后选择 **Azure AD**.

   >[!CAUTION]
   >
   >您必须在同一个Office 365订阅中使用一个帐户，以便您在该订阅中注册应用程序。

   >[!NOTE]
   >
   >如果您没有Azure帐户，则可以 [注册](https://azure.microsoft.com/en-us/free/){target=&quot;_blank&quot;}表示一个。 有关更多信息，请参阅Microsoft的文档或联系您的Microsoft代表。 创建Azure帐户后，可使用下面所述的过程注册一个或多个应用程序。
   >
   >
   >如果您有Azure帐户，但Azure订阅中没有Microsoft Dynamics 365的Office 365订阅，请遵循 [这些说明](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target=&quot;_blank&quot;}关联这两个帐户。

1. 查找并单击 **Azure Active Directory** 中。

   ![](assets/two.png)

1. 在管理下，单击 **应用程序注册**.

   ![](assets/three.png)

1. 单击 **新注册** 的双曲余切值。

   ![](assets/four.png)

1. 输入应用程序的名称，选择适用的帐户类型，然后输入重定向URL。 然后，单击 **注册** 页面底部。

   ![](assets/five.png)

1. 此时，您应会在 **应用程序注册** 选项卡。

   ![](assets/six.png)

## 配置应用程序权限 {#configuring-app-permissions}

1. 在 **应用程序注册** 选项卡中，单击要为其配置权限的应用程序。

   ![](assets/seven.png)

1. 在管理下，单击 **API权限**.

   ![](assets/eight.png)

1. 单击 **添加权限** 按钮。

   ![](assets/nine.png)

1. 选择 **Dynamics CRM**.

   ![](assets/ten.png)

1. 检查 **以组织用户身份访问通用数据服****** 框，然后单击 **添加权限。**

   ![](assets/eleven.png)

1. 成功添加权限后，请至少等待10秒。

   ![](assets/twelve.png)

1. 单击 **授予管理员同意** 按钮。

   ![](assets/thirteen.png)

1. 单击 **是** 确认。

   ![](assets/fourteen.png)

   你完蛋了！

   ![](assets/fifteen.png)

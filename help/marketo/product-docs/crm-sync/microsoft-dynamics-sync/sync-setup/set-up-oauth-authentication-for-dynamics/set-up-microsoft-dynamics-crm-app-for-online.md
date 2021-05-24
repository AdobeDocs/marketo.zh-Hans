---
description: 设置Microsoft Dynamics CRM在线应用程序 — Marketo文档 — 产品文档
title: 设置Microsoft Dynamics CRM联机应用程序
exl-id: ec3123c9-e484-4736-9831-9559cc393bd9
source-git-commit: 4283f1b6936316f3053543e06e7eaee45a7f2436
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 设置Microsoft Dynamics CRM联机应用程序{#set-up-microsoft-dynamics-crm-app-for-online}

## 设置{#set-up}

1. 导航到https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration 。

1. 按所有步骤操作。 在步骤3中，输入相关的应用程序名称(例如，“Marketo集成”)。 在“支持的帐户类型”下，选择“仅此组织目录中的帐户”。

1. 记下应用程序ID(ClientId)。 你以后需要在Marketo进入。

1. 按照[本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/grant-consent-for-client-id-and-app-registration.md)中的步骤授予管理员同意。

1. 通过单击&#x200B;**Certificates &amp; secrets**&#x200B;在管理中心生成客户端密钥。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-1.png)

1. 单击&#x200B;**新客户端密钥**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-2.png)

1. 添加客户端密钥说明，然后单击&#x200B;**Add**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-3.png)

   >[!CAUTION]
   >
   >请务必记下“客户端密钥”值（如下面的屏幕截图所示），因为您以后将需要它。 它只显示一次，您将无法再次检索它。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-4.png)

Marketo使用grant_type资源所有者密码凭据(ROPC)通过OAuth验证到Azure AD。 此方案需要为特定应用程序创建主领域发现策略。 使用此策略，Azure AD会将身份验证请求重定向到联合身份验证服务。 必须在AD Connect中为此启用密码哈希同步。 有关更多信息，请参阅[OAuth with ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)和[为应用程序](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application)设置hrd策略。

可在此处](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20anso%20include%20federated，are%20federated%20to%20Azure%20AD。)找到其他引用[。

完成后，应该将&#x200B;**将Dynamics CRM生成的客户端Id和密钥输入Marketo**。

## 在Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}中输入Dynamics CRM生成的客户端Id和密钥

以下步骤适用于联机版本&#x200B;_和_&#x200B;预配置版本。

1. 在Marketo中，单击&#x200B;**Admin**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-5.png)

1. 单击&#x200B;**Microsoft Dynamics**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-6.png)

1. 单击&#x200B;**禁用同步**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-7.png)

1. 在凭据旁边，单击&#x200B;**编辑**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-8.png)

1. 输入您之前检索到的&#x200B;**客户端Id**&#x200B;和&#x200B;**客户端密钥**，然后按&#x200B;**Save**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-9.png)

1. 单击&#x200B;**验证同步设置**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-10.png)

1. 单击&#x200B;**Next**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-11.png)

1. 您应会看到所有绿色复选标记。 单击&#x200B;**关闭**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-12.png)

   >[!NOTE]
   >
   >如果您在绿色复选标记中看到红色X，请参阅[本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)以获取修复选项。

1. 单击&#x200B;**启用同步**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-13.png)

就这样！

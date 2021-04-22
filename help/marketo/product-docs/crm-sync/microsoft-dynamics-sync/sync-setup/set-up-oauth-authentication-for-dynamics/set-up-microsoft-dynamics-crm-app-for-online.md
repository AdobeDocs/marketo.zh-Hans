---
description: 设置Microsoft Dynamics CRM联机应用程序 — Marketo Docs — 产品文档
title: 设置Microsoft Dynamics CRM联机应用程序
exl-id: ec3123c9-e484-4736-9831-9559cc393bd9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# 设置Microsoft Dynamics CRM联机应用程序{#set-up-microsoft-dynamics-crm-app-for-online}

## 设置Microsoft Dynamics CRM App for Online{#set-up-microsoft-dynamics-crm-app-for-online}

1. 导航到https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration。

1. 按照所有步骤操作。 对于步骤3，输入相关应用程序名称(例如“Marketo集成”)。 在“支持的帐户类型”下，选择“仅在此组织目录中的帐户”。

1. 写下应用程序 ID(ClientId)。 您以后需要在Marketo中输入它。

1. 按照[本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/grant-consent-for-client-id-and-app-registration.md)中的步骤授予管理员同意。

1. 单击&#x200B;**证书和机密**，在管理中心中生成客户端机密。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-1.png)

1. 单击&#x200B;**新建客户端密钥**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-2.png)

1. 添加“Client Secret”（客户端机密）描述，然后单击&#x200B;**Add**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-3.png)

   >[!CAUTION]
   >
   >请务必记下“客户端机密”值（如下面的屏幕截图中所示），因为您以后需要它。 它只显示一次，您将无法再次检索它。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-4.png)

Marketo使用grant_type资源所有者密码凭据(ROPC)验证到OAuth的Azure AD。 此方案需要为特定应用程序创建主领域发现策略。 使用此策略，Azure AD会将身份验证请求重定向到联合身份验证服务。 为此，必须在AD Connect中启用口令哈希同步。 有关详细信息，请参阅[OAuth with ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)和[为应用程序](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application)设置hrd策略。

可在此处找到其他引用[。](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20asso%20includes%20federated，are%20federated%20to%20Azure%20AD。)

完成后，应将&#x200B;**将Dynamics CRM生成的客户端Id和机密输入Marketo**。

## 在Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}中输入Dynamics CRM生成的客户端Id和Secret

以下步骤适用于联机&#x200B;_和_&#x200B;预先版本。

1. 在Marketo中，单击&#x200B;**Admin**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-5.png)

1. 单击&#x200B;**Microsoft Dynamics**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-6.png)

1. 单击&#x200B;**禁用同步**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-7.png)

1. 在凭据旁，单击&#x200B;**编辑**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-8.png)

1. 输入您之前检索到的&#x200B;**客户端ID**&#x200B;和&#x200B;**客户端机密**，然后按&#x200B;**保存**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-9.png)

1. 单击&#x200B;**验证同步设置**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-10.png)

1. 单击&#x200B;**下一步**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-11.png)

1. 您应当看到所有绿色复选标记。 单击&#x200B;**关闭**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-12.png)

   >[!NOTE]
   >
   >如果绿色复选标记中显示红色X，请参阅[本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)以了解修复选项。

1. 单击&#x200B;**启用同步**。

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-13.png)

就这样！

---
description: 为Azure AD Federated设置MSD，并预装AD FS、租户和Microsoft Online -Marketo文档 — 产品文档
title: 为Azure AD Federated设置MSD，并预先安装AD FS、租户和Microsoft Online
exl-id: b6c10048-d27e-4135-beef-232deddc2984
source-git-commit: 91ce0914755b578c896996fae1805022cb11c438
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# 为Azure AD Federated设置MSD，并预先安装AD FS、租户和Microsoft Online {#set-up-msd-for-azure-ad-federated-with-ad-fs-on-prem-tenant-and-microsoft-online}

## 设置Microsoft Dynamics CRM应用程序 {#set-up-microsoft-dynamics-crm-app}

1. 导航到https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration 。

1. 按所有步骤操作。 在步骤3中，输入相关的应用程序名称(例如，“Marketo集成”)。 在“支持的帐户类型”下，选择“仅此组织目录中的帐户”。

1. 记下应用程序ID(ClientId)。 你以后需要在Marketo进入。

1. 按照 [本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. 通过单击 **证书和密钥**.

   ![](assets/set-up-msd-for-azure-ad-federated-1.png)

1. 单击 **新客户端密钥**.

   ![](assets/set-up-msd-for-azure-ad-federated-2.png)

1. 添加客户端密钥说明并单击 **添加**.

   ![](assets/set-up-msd-for-azure-ad-federated-3.png)

   >[!CAUTION]
   >
   >请务必记下“客户端密钥”值（如下面的屏幕截图所示），因为您以后将需要它。 它只显示一次，您将无法再次检索它。

   ![](assets/set-up-msd-for-azure-ad-federated-4.png)

Marketo使用grant_type资源所有者密码凭据(ROPC)通过OAuth验证到Azure AD。 此方案需要为特定应用程序创建主领域发现策略。 使用此策略，Azure AD会将身份验证请求重定向到联合身份验证服务。 必须在AD Connect中为此启用密码哈希同步。 有关详细信息，请参阅 [带有ROPC的OAuth](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 和 [为应用程序设置hrd策略](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

其他参考 [可在此处找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20anso%20include%20federated，are%20federated%20to%20Azure%20AD。).

等你完事了，就该 **在Marketo中输入Dynamics CRM生成的客户端Id和密钥**.

## 在Marketo中输入Dynamics CRM生成的客户端Id和密钥 {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

1. 在Marketo中，单击 **管理员**.

   ![](assets/set-up-msd-for-azure-ad-federated-5.png)

1. 单击 **Microsoft Dynamics**.

   ![](assets/set-up-msd-for-azure-ad-federated-6.png)

1. 单击 **禁用同步**.

   ![](assets/set-up-msd-for-azure-ad-federated-7.png)

1. 在凭据旁边，单击 **编辑**.

   ![](assets/set-up-msd-for-azure-ad-federated-8.png)

1. 输入 **客户端Id** 和 **客户端密钥** 您之前检索过，然后按 **保存**.

   ![](assets/set-up-msd-for-azure-ad-federated-9.png)

1. 单击 **验证同步设置**.

   ![](assets/set-up-msd-for-azure-ad-federated-10.png)

1. 单击 **下一个**.

   ![](assets/set-up-msd-for-azure-ad-federated-11.png)

1. 您应会看到所有绿色复选标记。 单击 **关闭**.

   ![](assets/set-up-msd-for-azure-ad-federated-12.png)

   >[!NOTE]
   >
   >如果您在绿色复选标记中看到红色X，请参阅 [本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) ，以了解修复选项。

1. 单击 **启用同步**.

   ![](assets/set-up-msd-for-azure-ad-federated-13.png)

就这样！

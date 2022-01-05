---
description: 第3步（共4步） — 在MS Dynamics中设置客户端应用程序 — Marketo文档 — 产品文档
title: 第3步（共4步） — 在MS Dynamics上设置客户端应用程序
source-git-commit: 598390517dea96b0503fd9c0cdfd47bd7617b48a
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 步骤3（共4步）：在MS Dynamics上设置客户端应用程序 {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [步骤1（共4步）：安装具有资源所有者密码控制连接的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [步骤2（共4步）：使用资源所有者密码控制连接设置Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)


1. 导航到https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration 。

1. 按所有步骤操作。 在步骤3中，输入相关的应用程序名称(例如，“Marketo集成”)。 在“支持的帐户类型”下，选择“仅此组织目录中的帐户”。

1. 记下应用程序ID(ClientId)。 你以后需要在Marketo进入。

1. 按照 [本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. 通过单击 **证书和密钥**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. 单击 **新客户端密钥**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. 添加客户端密钥说明并单击 **添加**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >请务必记下“客户端密钥”值（如下面的屏幕截图所示），因为您以后将需要它。 它只显示一次，您将无法再次检索它。

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## Azure AD Federated与AD FS本地 {#azure-ad-federated-with-ad-fs-on-prem}

Azure AD到ADFS Onprem的联合需要为特定应用程序创建家庭领域发现策略。 使用此策略，Azure AD会将身份验证请求重定向到联合身份验证服务。 必须在AD Connect中为此启用密码哈希同步。 有关详细信息，请参阅 [带有ROPC的OAuth](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 和 [为应用程序设置hrd策略](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

其他参考 [可在此处找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20anso%20include%20federated，are%20federated%20to%20Azure%20AD。).

## 在继续执行步骤4之前 {#before-proceeding-to-step-4}

* 如果要限制同步的记录数， [设置自定义同步筛选器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 现在。
* 运行 [验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 进程。 它验证初始设置是否正确完成。
* 在Microsoft Dynamics CRM中登录到Marketo同步用户。

>[!MORELIKETHIS]
>
>* [步骤4（共4步）：将Marketo解决方案与资源所有者密码控制连接连接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md)


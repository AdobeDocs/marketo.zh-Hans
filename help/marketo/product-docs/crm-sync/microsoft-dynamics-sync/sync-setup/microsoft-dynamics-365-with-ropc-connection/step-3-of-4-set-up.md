---
description: 第3步（共4步） — 在MS [!DNL Dynamics] 上设置客户端应用程序 — Marketo文档 — 产品文档
title: 第3步（共4步） — 在MS [!DNL Dynamics]上设置客户端应用程序
exl-id: e7897174-3303-4c3b-8832-3e10f34fca96
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# 第3步（共4步）：在MS [!DNL Dynamics]上设置客户端应用程序 {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [第1步（共4步）：安装具有资源所有者密码控制连接的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [第2步（共4步）：使用资源所有者密码控制连接设置Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. 导航到此[Microsoft文章](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}。

1. 执行所有步骤。 对于步骤3，输入相关的应用程序名称（例如“[!DNL Marketo Integration]”）。 在支持的帐户类型下，仅在此组织目录中选择帐户。

1. 写下应用程序ID (ClientId)。 您稍后需要在Marketo中输入。

1. 按照[本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}中的步骤授予管理员同意。

1. 通过单击&#x200B;**[!UICONTROL Certificates & secrets]**&#x200B;在管理中心生成客户端密钥。

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. 单击 **[!UICONTROL New client secret]**。

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. 添加客户端密码描述并单击&#x200B;**[!UICONTROL Add]**。

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >请确保记下客户端密钥值（见下面的屏幕快照），因为您以后会需要它。 它只会显示一次，您将无法再次检索它。

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## [!DNL Azure AD]与[!DNL AD FS On-prem]联合 {#azure-ad-federated-with-ad-fs-on-prem}

将[!DNL Azure]AD联合到[!DNL ADFS Onprem]需要为特定应用程序创建主领域发现策略。 使用此策略，[!DNL Azure] AD会将身份验证请求重定向到联合身份验证服务。 必须在[!DNL AD Connect]中为此启用密码哈希同步。 有关详细信息，请参阅[[!DNL OAuth] 使用 [!DNL ROPC]](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)和[为应用程序设置hrd策略](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application)。

其他引用[可在此处](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&text=此%20report%20also%20include%20federated，为%20federated%20to%20Azure%20AD。){target="_blank"}找到。

## 在继续执行步骤4之前 {#before-proceeding-to-step-4}

* 如果要限制同步记录数，请立即[设置自定义同步筛选器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
* 运行[验证 [!DNL Microsoft Dynamics] 同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)进程。 它验证初始设置是否正确完成。
* 登录到[!DNL Microsoft Dynamics] CRM中的Marketo同步用户。

>[!MORELIKETHIS]
>
>* [第4步（共4步）：连接Marketo解决方案与资源所有者密码控制连接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md){target="_blank"}

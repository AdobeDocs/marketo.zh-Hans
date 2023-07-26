---
unique-page-id: 3571827
description: 第2步（共3步） — 使用服务器到服务器连接设置Marketo解决方案 — Marketo文档 — 产品文档
title: 第2步（共3步） — 设置具有服务器到服务器连接的Marketo解决方案
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
feature: Microsoft Dynamics
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 0%

---

# 第2步（共3步）：设置具有服务器到服务器连接的Marketo解决方案 {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[第1步（共3步）：安装具有服务器到服务器连接的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}

## 在Azure AD中创建客户端应用程序 {#create-client-application-in-azure-ad}

1. 导航到 [此Microsoft文章](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. 执行所有步骤。 对于步骤3，输入相关的应用程序名称(例如“Marketo集成”)。 在支持的帐户类型下，选择 **仅此组织目录中的帐户**.

1. 写下应用程序ID (ClientId)和租户ID。 您稍后需要在Marketo中输入。

1. 按照以下步骤授予管理员同意 [本文内容](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. 通过单击在管理中心生成客户端密钥 **证书和密钥**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. 单击 **新客户端密码** 按钮。

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. 输入客户端密码说明，然后单击 **添加**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>请确保记下客户端密钥值（见下面的屏幕快照），因为您以后会需要它。 它只会显示一次，您将无法再次检索它。

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## 在Microsoft中创建应用程序用户 {#create-application-user-in-microsoft}

1. 执行以下链接中的步骤 [在Microsoft中设置应用程序用户](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation){target="_blank"}.

   >[!IMPORTANT]
   >
   >* 在授予应用程序用户权限时，请确保将其分配给“Marketo同步用户角色”。
   >* 请注意以下位置中应用程序用户的电子邮件地址 [查看详细信息选项](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user){target="_blank"} 在电源平台上。 在Marketo中设置与MS Dynamics的连接时，此电子邮件地址将用作用户名。
   >* 同步用户在CRM中所做的任何更新都将 **非** 已同步回Marketo。

## Azure AD Federated与AD FS内部部署 {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD到ADFS Onprem需要为特定应用程序创建主领域发现策略。 使用此策略时，Azure AD会将身份验证请求重定向到联合身份验证服务。 必须在AD Connect中为此启用密码哈希同步。 有关详细信息，请参阅 [带有ROPC的OAuth](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc){target="_blank"} and [Set an hrd policy for an application](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application){target="_blank"}.

其他引用 [可在此处找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=此%20report%20also%20include%20federated，为%20federated%20to%20Azure%20AD。){target="_blank"}.

## 配置Marketo解决方案 {#configure-marketo-solution}

快到了！ 我们只剩下通知Marketo解决方案所创建的新用户。

1. 返回高级设置部分，然后单击 ![](assets/image2015-5-13-15-3a49-3a19.png) 图标，然后选择 **Marketo配置**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果您没有看到 **Marketo配置** 在“设置”菜单中，刷新页面。 如果这样行不通，请尝试 [发布Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"} 再次登录或注销并重新登录。

1. 单击 **默认**.

   ![](assets/fifteen.png)

1. 单击 **Marketo用户** 字段并选择您创建的同步用户。

   ![](assets/sixteen.png)

1. 单击 ![](assets/image2015-3-13-15-3a10-3a11.png) 图标以保存更改。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 单击 **X** 以关闭屏幕。

   ![](assets/seventeen.png)

1. 单击 ![](assets/image2015-5-13-15-3a49-3a19-1.png) 图标，然后选择 **解决方案**.

   ![](assets/eighteen.png)

1. 单击 **发布所有自定义项** 按钮。

   ![](assets/nineteen.png)

   >[!NOTE]
   >
   >如果您从基本身份验证升级到OAuth，您可以使用 [本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"} 以重新配置您的身份验证。

## 在继续执行步骤3之前 {#before-proceeding-to-step}

* 如果要限制同步的记录数， [设置自定义同步过滤器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} 现在。
* 运行 [验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} 进程。 它验证初始设置是否正确完成。
* 登录到Microsoft Dynamics CRM中的“Marketo同步用户”。

>[!MORELIKETHIS]
>
>* [第3步（共3步）：将Marketo解决方案与服务器到服务器连接连接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md){target="_blank"}
>* [重新配置Dynamics身份验证方法](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"}

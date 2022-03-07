---
unique-page-id: 3571827
description: 步骤2（共3步） — 使用服务器到服务器连接设置Marketo解决方案 — Marketo文档 — 产品文档
title: 步骤2（共3步） — 使用服务器到服务器连接设置Marketo解决方案
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
source-git-commit: 3a52db828a9bbf01b617d6e417d078d11ea30fb7
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# 步骤2（共3步）：通过服务器到服务器连接设置Marketo解决方案 {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[步骤1（共3步）：通过服务器到服务器连接安装Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)

## 在Azure AD中创建客户端应用程序 {#create-client-application-in-azure-ad}

1. 导航到 [本Microsoft文章](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration).

1. 按所有步骤操作。 在步骤3中，输入相关的应用程序名称(例如，“Marketo集成”)。 在支持的帐户类型下，选择 **此组织目录中的帐户**.

1. 记下应用程序ID(ClientId)和租户ID。 你以后需要在Marketo进入。

1. 按照以下步骤授予管理员同意 [在本文中](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. 通过单击 **证书和密钥**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. 单击 **新客户端密钥** 按钮。

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. 输入客户端密钥说明并单击 **添加**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>请务必记下“客户端密钥”值（如下面的屏幕截图所示），因为您以后将需要它。 它只显示一次，您将无法再次检索它。

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## 在Microsoft中创建应用程序用户 {#create-application-user-in-microsoft}

1. 按照以下链接中的步骤操作 [在Microsoft中设置应用程序用户](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation).

   >[!IMPORTANT]
   >
   >* 在为应用程序用户授予权限时，请确保将其分配给“Marketo同步用户角色”。
   >* 从 [查看详细信息选项](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) 在电源平台上。 在Marketo中设置与MS Dynamics的连接时，此电子邮件地址将用作用户名。


## Azure AD Federated与AD FS本地 {#azure-ad-federated-with-ad-fs-on-prem}

Azure AD到ADFS Onprem的联合需要为特定应用程序创建家庭领域发现策略。 使用此策略，Azure AD会将身份验证请求重定向到联合身份验证服务。 必须在AD Connect中为此启用密码哈希同步。 有关详细信息，请参阅 [带有ROPC的OAuth](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 和 [为应用程序设置hrd策略](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

其他参考 [可在此处找到](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20anso%20include%20federated，are%20federated%20to%20Azure%20AD。).

## 配置Marketo解决方案 {#configure-marketo-solution}

快到了！ 我们只剩下一步，就是向Marketo解决方案告知所创建的新用户。

1. 返回至高级设置部分，然后单击 ![](assets/image2015-5-13-15-3a49-3a19.png) 图标，然后选择 **Marketo配置**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >如果你看不到 **Marketo配置** 在“设置”菜单中，刷新页面。 如果那不行，请尝试 [发布Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md) 再次注销，然后重新登录。

1. 单击 **默认**.

   ![](assets/fifteen.png)

1. 单击 **Marketo用户** 字段，然后选择您创建的同步用户。

   ![](assets/sixteen.png)

1. 单击 ![](assets/image2015-3-13-15-3a10-3a11.png) 图标来保存更改。

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. 单击 **X** 中，单击以关闭屏幕。

   ![](assets/seventeen.png)

1. 单击 ![](assets/image2015-5-13-15-3a49-3a19-1.png) 图标，然后选择 **解决方案**.

   ![](assets/eighteen.png)

1. 单击 **发布所有自定义设置** 按钮。

   ![](assets/nineteen.png)

   >[!NOTE]
   >
   >如果您从基本身份验证升级到OAuth，则可以使用 [本文](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md) 来重新配置您的身份验证。

## 继续执行步骤3之前 {#before-proceeding-to-step}

* 如果要限制同步的记录数， [设置自定义同步筛选器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 现在。
* 运行 [验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 进程。 它验证初始设置是否正确完成。
* 在Microsoft Dynamics CRM中登录到Marketo同步用户。

>[!MORELIKETHIS]
>
>* [步骤3（共3步）：将Marketo解决方案与服务器连接连接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md)
>* [重新配置Dynamics身份验证方法](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)


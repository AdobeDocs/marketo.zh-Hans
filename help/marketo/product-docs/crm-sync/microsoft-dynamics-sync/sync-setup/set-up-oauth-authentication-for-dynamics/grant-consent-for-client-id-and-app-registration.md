---
description: 客户端ID和应用程序注册的许可 — Marketo Docs — 产品文档
title: 同意客户端ID和应用程序注册
translation-type: tm+mt
source-git-commit: 3a6d9987e214aa8606b9f5abdc780a81355b1001
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---


# 对客户端ID和应用程序注册的许可{#grant-consent-for-client-id-and-app-registration}

## 授予同步用户{#grant-delegated-user-permissions-for-the-sync-user}的委派用户权限

1. 使用简洁的文本项目（Windows用记事本，Mac用文本编辑）创建统一资源标识符(URI)，通过粘贴以下文本并替换client_id、redirect_uri和状态值来进行授权。

   ```
   https://login.microsoftonline.com/common/oauth2/authorize?
   client_id='xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx'
   &response_type='code'
   &redirect_uri='https://www.<ourdomain>.com'
   &response_mode='query'
   &state='SOME_UNIQUE_UID'
   client_id value should be the client_id generated in App Registration process
   redirect_uri value should be same as value entered at the time of App registration-> Redirect URIs
   state value can be any ID (e.g.,12345)
   ```

   <table> 
    <colgroup> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>client_id值</strong></td> 
      <td>应是在应用程序注册过程中生成的client_id</td> 
     </tr> 
     <tr> 
      <td><strong>redirect_uri值</strong></td> 
      <td>应与在应用程序注册&gt;重定向URI时输入的值相同</td> 
     </tr> 
     <tr> 
      <td><strong>状态值</strong></td> 
      <td>可以是任何ID(例如，12345)</td> 
     </tr> 
    </tbody> 
   </table>

   最终的URL应当如下：`https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. 打开在任何浏览器中创建的URI。

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. 以您授予权限的同步用户身份登录。

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >如果您已经以管理员身份在其他选项卡中登录到Azure，则需要使用其他浏览器或Incognito模式以同步用户身份登录。

1. 单击&#x200B;**接受**。

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## 授予所有用户的同意{#grant-consent-for-all-users}

作为管理员，您还可以代表您的租户中的所有用户同意应用程序的授权权限。 管理同意会阻止租户中每个用户显示同意对话框，具有管理员角色的用户可以在Azure门户中完成此操作。 在此处了解哪些管理员角色可以[同意授权。](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference)

1. 在您的Azure门户中，导航到应用程序主页。

1. 在“管理”下，单击&#x200B;**API权限**。

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. 单击&#x200B;**授予管理员同意**（对于租户）按钮。

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. 单击&#x200B;**是**&#x200B;进行确认。

   ![](assets/grant-consent-for-client-id-app-registration-6.png)

>[!MORELIKETHIS]
>
>[为On-prem设置Microsoft Dynamics CRM应用程序](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/set-up-microsoft-dynamics-crm-app-for-on-prem.md)

---
description: 同意客户端Id和应用程序注册 — Marketo文档 — 产品文档
title: 同意客户端ID和应用程序注册
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# 同意客户端ID和应用程序注册 {#grant-consent-for-client-id-and-app-registration}

## 为同步用户授予委派的用户权限 {#grant-delegated-user-permissions-for-the-sync-user}

1. 使用干净文本程序(Windows的记事本、Mac的文本编辑)通过粘贴以下文本并替换client_id、redirect_uri和状态值来创建用于授权的统一资源标识符(URI)。

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
      <td>应为应用程序注册过程中生成的client_id</td> 
     </tr> 
     <tr> 
      <td><strong>redirect_uri值</strong></td> 
      <td>应与应用程序注册&gt;重定向URI时输入的值相同</td> 
     </tr> 
     <tr> 
      <td><strong>状态值</strong></td> 
      <td>可以是任何ID(例如，12345)</td> 
     </tr> 
    </tbody> 
   </table>

   最终URL应如下所示： `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. 在任意浏览器中打开您创建的URI。

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. 以您授予权限的同步用户身份登录。

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >如果您已在其他选项卡中作为管理员登录Azure，则将需要使用其他浏览器或无痕模式以同步用户的身份登录。

1. 单击 **接受**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## 授予所有用户的同意 {#grant-consent-for-all-users}

作为管理员，您还可以代表租户中的所有用户同意应用程序的委托权限。 管理同意阻止租户中的每个用户显示同意对话框，并且可由具有管理员角色的用户在Azure门户中完成。 了解哪些管理员角色可以 [同意在此处委派权限](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference).

1. 在Azure门户中，导航到应用程序主页。

1. 在管理下，单击 **API权限**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. 单击 **授予管理员同意** （适用于租户）按钮。

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. 单击 **是** 以确认。

   ![](assets/grant-consent-for-client-id-app-registration-6.png)


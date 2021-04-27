---
description: 使用OAuth 2.0登录 — Marketo Docs — 产品文档
title: 使用OAuth 2.0登录
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# 使用OAuth 2.0 {#log-in-using-oauth-2-0}登录

Salesforce使用OAuth协议允许应用程序用户安全地访问（使用OAuth 2.0验证应用程序）数据，而不必显示登录凭据。 以下是要执行的步骤，以便将Marketo与Salesforce安全连接并同步。

## 设置已连接的应用程序{#set-up-connected-app}

1. 在Salesforce的设置下，在平台工具中，导航到应用程序、App Manager，然后单击&#x200B;**新建连接的应用程序**。

   ![](assets/setting-up-oauth-2-1.png)

1. 填写详细信息，然后单击&#x200B;**保存**。

   ![](assets/setting-up-oauth-2-2.png)

1. 单击&#x200B;**启用OAuth设置**&#x200B;复选框。 对于回调URL，输入`https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`。 选择所有可用的OAuth作用域，然后单击&#x200B;**添加**。

   ![](assets/setting-up-oauth-2-3.png)

1. 单击&#x200B;**保存**。

   ![](assets/setting-up-oauth-2-4.png)

1. 单击&#x200B;**继续**。

   ![](assets/setting-up-oauth-2-5.png)

1. 复制消费方密钥和消费方密码。

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>保存消费方密钥和消费方密码信息，以供以后在Marketo中使用。

## 设置Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* 必须为Salesforce同步用户启用API访问（如果您是Salesforce Professional Edition用户，则默认情况下该访问不可用 — 请与您的Salesforce帐户主管联系）。
>* Marketo同步用户必须在Salesforce中创建。
>* 对于现有客户，在客户订阅上启用了“启用OAuth for SFDC同步”功能。
>* 弹出窗口阻止程序被禁用。
>* 已创建连接的应用程序，并且我们拥有消费方密钥和消费方密码可供使用。


>[!CAUTION]
>
>单击&#x200B;**同步字段**&#x200B;之前，请务必从同步用户隐藏Marketo中不需要的所有字段。 单击“同步字段”后，用户在SFDC中可以看到的所有字段都将在Marketo中永久创建，并且无法删除。

1. 在“Marketo管理员”部分，单击&#x200B;**CRM**，然后单击&#x200B;**与Salesforce**&#x200B;同步。

   ![](assets/setting-up-oauth-2-7.png)

1. 添加您之前录制的消费方密钥和消费方密码信息，然后单击并&#x200B;**保存**。

   ![](assets/setting-up-oauth-2-8.png)

1. 在Marketo Salesforce同步页面上，单击&#x200B;**使用Salesforce登录**&#x200B;按钮。

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >如果您看到的是用户名/密码/令牌字段，而不是“使用Salesforce登录”按钮，则您的Marketo订阅将启用基本身份验证。 请参阅[设置具有基本身份验证的Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)。 一旦使用一组凭据开始同步，则不会切换Salesforce凭据或订阅。 如果您要使用Oauth 2.0，请联系您的客户成功经理。

1. 将显示带有salesforce登录页面的弹出窗口。 您的“Marketo同步用户”凭据中的密钥并登录。

   ![](assets/setting-up-oauth-2-10.png)

1. 输入您通过电子邮件（由Salesforce发送）收到的验证代码，然后单击&#x200B;**验证**。

   ![](assets/setting-up-oauth-2-11.png)

1. 成功验证后，访问页面将显示请求访问。 单击&#x200B;**允许**。

   ![](assets/setting-up-oauth-2-12.png)

1. 几分钟后，Marketo中将出现一个弹出窗口。 单击&#x200B;**确认凭据**。

   ![](assets/setting-up-oauth-2-13.png)

1. 完成字段同步后，单击&#x200B;**开始Salesforce同步**。

   ![](assets/setting-up-oauth-2-14.png)

1. 单击&#x200B;**开始同步**。

   ![](assets/setting-up-oauth-2-15.png)

您在Marketo和Salesforce之间的同步正在进行中。

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [第1步，共3步：将Marketo字段添加到Salesforce(Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [第2步，共3步：为Marketo创建Salesforce用户(Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [在SalesforceAppExchange中安装Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [在Salesforce Enterprise/Unlimited中配置Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)


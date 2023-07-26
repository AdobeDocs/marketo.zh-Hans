---
description: 使用OAuth 2.0登录 — Marketo文档 — 产品文档
title: 使用OAuth 2.0登录
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 使用OAuth 2.0登录 {#log-in-using-oauth-2-0}

Salesforce使用OAuth协议来允许应用程序用户安全地访问（使用OAuth 2.0对应用程序进行身份验证）数据，而无需泄露登录凭据。 以下是将Marketo安全地连接并与Salesforce同步要执行的步骤。

>[!IMPORTANT]
>
>要使用OAuth连接Marketo和Salesforce，请通过私人（无痕化）浏览器登录Marketo，以避免使用错误的用户名连接到Salesforce。

## 设置连接的应用程序 {#set-up-connected-app}

1. 在Salesforce的设置下，在平台工具中，导航到应用程序、应用程序管理器，然后单击 **新连接的应用程序**.

   ![](assets/setting-up-oauth-2-1.png)

1. 填写详细信息并单击 **保存**.

   ![](assets/setting-up-oauth-2-2.png)

1. 单击 **启用OAuth设置** 复选框。 对于回调URL，输入 `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. 选择所有可用的OAuth范围，然后单击 **添加**.

   ![](assets/setting-up-oauth-2-3.png)

1. 单击 **保存**.

   ![](assets/setting-up-oauth-2-4.png)

1. 单击 **继续**.

   ![](assets/setting-up-oauth-2-5.png)

1. 复制使用者密钥和使用者密码。

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>保存使用者密钥和使用者密钥信息，以供将来在Marketo中使用。

## 设置Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* 必须为Salesforce同步用户启用API访问权限（如果您是Salesforce Professional Edition用户，则默认情况下无法访问该权限 — 请联系您的Salesforce帐户管理员）。
>* 必须在Salesforce中创建Marketo同步用户。
>* 对于现有客户，在客户的订阅上启用了“为SFDC同步启用OAuth”功能。
>* 禁用了弹出窗口阻止程序。
>* 已创建连接的应用程序，并且我们具有可供使用的使用者密钥和使用者密钥。

>[!CAUTION]
>
>在单击之前，请确保向同步用户隐藏Marketo中所有不需要的字段 **同步字段**. 单击“同步字段”后，用户在SFDC中可以查看的所有字段都将在Marketo中永久创建，且无法删除。

1. 在Marketo管理部分中，单击 **CRM**，则 **与Salesforce同步**.

   ![](assets/setting-up-oauth-2-7.png)

1. 添加您之前录制的“使用者密钥”和“使用者密钥”信息，然后单击 **保存**.

   ![](assets/setting-up-oauth-2-8.png)

1. 在Marketo Salesforce同步页面上，单击 **使用Salesforce登录** 按钮。

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >如果您看到“用户名/密码/令牌”字段而不是“使用Salesforce登录”按钮，则表示您的Marketo订阅已启用基本身份验证。 请参阅 [使用基本身份验证设置Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md). 使用一组凭据开始同步后，不会切换Salesforce凭据或订阅。 如果您希望使用Oauth 2.0，请联系Adobe客户团队（您的客户经理）。

1. 此时将显示一个包含salesforce登录页面的弹出窗口。 键入“Marketo同步用户”凭据并登录。

   ![](assets/setting-up-oauth-2-10.png)

1. 输入您通过电子邮件收到的验证码（由Salesforce发送），然后单击 **验证**.

   ![](assets/setting-up-oauth-2-11.png)

1. 成功验证后，访问页面将显示请求访问。 单击 **允许**.

   ![](assets/setting-up-oauth-2-12.png)

1. 几分钟后，Marketo中将出现弹出窗口。 单击 **确认凭据**.

   ![](assets/setting-up-oauth-2-13.png)

1. 字段同步完成后，单击 **启动Salesforce同步**.

   ![](assets/setting-up-oauth-2-14.png)

1. 单击 **开始同步**.

   ![](assets/setting-up-oauth-2-15.png)

Marketo与Salesforce之间的同步正在进行中。

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [第1步（共3步）：将Marketo字段添加到Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [第2步（共3步）：创建Marketo的Salesforce用户(Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [在SalesforceAppExchange中安装Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [在Salesforce Enterprise/Unlimited中配置Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

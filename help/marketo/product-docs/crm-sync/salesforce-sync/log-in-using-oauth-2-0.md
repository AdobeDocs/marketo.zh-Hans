---
description: 使用OAuth 2.0登录 — Marketo文档 — 产品文档
title: 使用OAuth 2.0登录
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 使用OAuth 2.0登录 {#log-in-using-oauth-2-0}

Salesforce使用OAuth协议，让应用程序用户能够安全访问（使用OAuth 2.0验证应用程序）数据，而无需显示登录凭据。 以下是要执行的步骤，以安全地连接Marketo并将其与Salesforce同步。

>[!IMPORTANT]
>
>要使用OAuth连接Marketo和Salesforce，请通过私人（隐身）浏览器登录到Marketo，以避免使用错误的用户名连接到Salesforce。

## 设置连接的应用程序 {#set-up-connected-app}

1. 在Salesforce的设置下，在平台工具中，导航到应用程序、应用程序管理器，然后单击 **新的连接应用程序**.

   ![](assets/setting-up-oauth-2-1.png)

1. 填写详细信息并单击 **保存**.

   ![](assets/setting-up-oauth-2-2.png)

1. 单击 **启用OAuth设置** 复选框。 对于回调URL，输入 `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. 选择所有可用的OAuth作用域，然后单击 **添加**.

   ![](assets/setting-up-oauth-2-3.png)

1. 单击 **保存**.

   ![](assets/setting-up-oauth-2-4.png)

1. 单击 **继续**.

   ![](assets/setting-up-oauth-2-5.png)

1. 复制消费者密钥和消费者密钥。

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>保存消费者密钥和消费者密钥信息，以供日后在Marketo中使用。

## 设置Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* 必须为Salesforce同步用户启用API访问（如果您是Salesforce Professional Edition用户，则该访问默认不可用 — 请联系您的Salesforce帐户管理员）。
>* Marketo同步用户必须在Salesforce中创建。
>* 对于现有客户，客户订阅中启用了“为SFDC同步启用OAuth”功能。
>* 弹出窗口阻止程序处于禁用状态。
>* 已创建连接的应用程序，并且我们提供了消费者密钥和消费者密钥以供使用。


>[!CAUTION]
>
>在单击之前，请确保对同步用户隐藏Marketo中不需要的所有字段 **同步字段**. 单击“同步字段”后，用户在SFDC中可以看到的所有字段都将在Marketo中永久创建，并且无法删除。

1. 在Marketo管理员部分中，单击 **CRM**，则 **与Salesforce同步**.

   ![](assets/setting-up-oauth-2-7.png)

1. 添加您之前记录的消费者密钥和消费者密钥信息，然后单击并 **保存**.

   ![](assets/setting-up-oauth-2-8.png)

1. 在Marketo Salesforce同步页面上，单击 **使用Salesforce登录** 按钮。

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >如果您看到“用户名/密码/令牌”字段而没有“使用Salesforce登录”按钮，则您的Marketo订阅将启用基本身份验证。 请参阅 [使用基本身份验证设置Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md). 一旦使用一组凭据开始同步，则不会切换Salesforce凭据或订阅。 如果要使用Oauth 2.0，请联系Adobe客户团队（您的客户经理）。

1. 此时将显示一个带有salesforce登录页面的弹出窗口。 “Marketo同步用户”凭据中的密钥并登录。

   ![](assets/setting-up-oauth-2-10.png)

1. 输入您通过电子邮件（由Salesforce发送）收到的验证代码，然后单击 **验证**.

   ![](assets/setting-up-oauth-2-11.png)

1. 成功验证后，访问页面将显示请求访问。 单击 **允许**.

   ![](assets/setting-up-oauth-2-12.png)

1. 几分钟后，将在Marketo中显示一个弹出窗口。 单击 **确认凭据**.

   ![](assets/setting-up-oauth-2-13.png)

1. 字段同步完成后，单击 **启动Salesforce同步**.

   ![](assets/setting-up-oauth-2-14.png)

1. 单击 **开始同步**.

   ![](assets/setting-up-oauth-2-15.png)

您在Marketo和Salesforce之间的同步正在进行中。

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [步骤1（共3步）：将Marketo字段添加到Salesforce（企业/无限制）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [步骤2（共3步）：为Marketo创建Salesforce用户（企业/无限制）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [在SalesforceAppExchange中安装Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [在Salesforce企业/无限制中配置Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)


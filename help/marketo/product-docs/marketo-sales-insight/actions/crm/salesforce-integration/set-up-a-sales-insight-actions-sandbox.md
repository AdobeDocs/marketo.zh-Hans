---
description: 设置Sales Insight操作沙盒 — Marketo文档 — 产品文档
title: 设置Sales Insight操作沙盒
exl-id: 8bc3a8a6-7fbc-4cbe-99a7-21b066ec4f96
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# 设置Sales Insight操作沙盒 {#set-up-a-sales-insight-actions-sandbox}

>[!NOTE]
>
>Marketo Sales Insight Actions是一个基于Web的应用程序，它通过[Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}与Salesforce用户界面集成。 它有时称为“Marketo Sales”，或简称为“Actions”。

如果您有Marketo沙盒，则可以启用操作实例来与沙盒一起用于测试目的。

在设置操作实例时，您必须决定是将它配置为与Salesforce沙盒一起使用还是与Salesforce生产一起使用。 这是因为Salesforce对每个使用不同的端点，而Actions使用与Salesforce的连接来激活和验证用户。

请按照以下步骤操作，设置操作实例以与您的Salesforce沙盒实例配合使用。

>[!NOTE]
>
>您可以了解有关用户如何[激活其“操作”座位](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-checklist.md){target="_blank"}的详细信息。 您还可以了解用户将如何[使用Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}进行身份验证。 此外，如果您希望用户使用电子邮件和密码进行身份验证，可以在[登录管理设置文章](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}中了解有关此内容的更多信息。

## 请求将操作实例配置为您的Marketo沙盒{#request=an-actions-instance}

除非得到请求，否则不会为Marketo沙盒实例启用销售分析操作。 联系Adobe客户团队（您的客户经理）以提交请求。

## 为Marketo沙盒配置您的操作帐户 {#provision-your-actions-account}

一旦为Marketo沙盒启用了操作，您将需要执行以下步骤来激活新实例。

1. 登录到您的Marketo沙盒实例。

1. 导航到&#x200B;**管理员**。

1. 选择&#x200B;**销售分析**。

1. 选择&#x200B;**操作配置**。

   >[!IMPORTANT]
   >
   >一个电子邮件地址只能用于沙盒实例和生产实例中的一个Actions实例。 如果您是管理员，并且需要跨生产和沙盒访问多个实例，则必须为每个实例使用不同的电子邮件地址。

1. 在配置信息卡中，选择要邀请加入Sales Insight Actions实例的用户。

## 激活您的操作实例 {#activate-your-actions-instance}

需要使用Salesforce生产帐户激活您的操作实例。 激活后，它可以切换到Salesforce沙盒帐户。

1. 找到已发送的邀请。

1. 单击&#x200B;**开始使用**&#x200B;链接。

1. 使用您的Salesforce Production实例激活。

1. 按照提示设置帐户。 有关详细概述，请查看我们的[用户入门文章](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}。

## 准备您的操作实例以与Salesforce沙盒实例兼容 {#prepare-your-actions-instance}

操作要求您首先使用Salesforce生产用户激活新实例。 激活后，您可以使用以下步骤准备实例以使其与Salesforce沙盒兼容。

1. 将登录设置更新为“所有登录方法”，以便您可以根据需要使用用户名和密码登录。 如果首选，可在配置所有内容后将其切换回“仅限Salesforce”。 [请参阅此处](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}以了解如何执行此操作。

1. 断开与Salesforce Production的连接，并连接到Salesforce沙盒。 [查看如何在此连接](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}。 对于步骤3，选择“Sandbox”而不是“Salesforce”。 如果您已经连接，您应该会在Salesforce的“连接和定制”选项卡上看到断开连接的选项。

>[!NOTE]
>
>如果您的Salesforce实例有自定义域，我们建议在连接到Salesforce或登录到Actions之前登录到您的Salesforce实例。

## 请求转换您的操作实例以便与您的Salesforce沙盒兼容 {#request-your-actions-instance-be-converted}

1. 联系[Marketo Engage支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}，请求将新的Sales Insight Actions实例配置为与Salesforce沙盒兼容。

1. 尝试使用toutapp.com/login页面上的“使用Salesforce登录”按钮登录，以测试所有内容均已正确配置。

   ![](assets/set-up-a-sales-insight-actions-sandbox-1.png)

   >[!TIP]
   >
   >如果此时遇到任何问题，您可以请求密码重置，并使用密码重新获得对帐户的访问权限。

现在，您的实例已准备好与您的Salesforce沙盒实例一起使用。 如果要使用Salesforce中的[Salesforce自动登录](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}，可以在[登录管理设置](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}中切换回“仅限Salesforce”。

>[!NOTE]
>
>* [将您的Sales Insight Actions帐户连接到Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}
>* [销售分析操作用户入门指南](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}
>* [从Salesforce自动登录](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}
>* [登录管理设置](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}

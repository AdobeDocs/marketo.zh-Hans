---
description: 登录管理设置 — Marketo文档 — 产品文档
title: 登录管理设置
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# 登录管理设置 {#login-management-settings}

登录管理设置允许管理员在全局级别为Sales Insight Actions的用户设置身份验证首选项。

>[!NOTE]
>
>默认情况下，将为Sales Insight Actions实例选择“仅限Salesforce”选项。 我们建议使用此设置，以便用户可以 [自动登录](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) 来自Salesforce。

## 更新登录管理设置 {#update-login-management-settings}

>[!NOTE]
>
>**需要管理员权限**

更新您的登录管理首选项，请执行以下步骤。

1. 单击齿轮图标并选择 **设置**.

   ![](assets/login-management-settings-1.png)

1. 在管理设置下，单击 **常规**.

   ![](assets/login-management-settings-2.png)

1. 向下滚动到登录管理卡并选择所需的设置（在本例中，我们选择“仅限Salesforce”）。 单击 **保存** 完成时。

   ![](assets/login-management-settings-3.png)

## 仅限Salesforce常见问题解答 {#salesforce-only-faq}

“仅限Salesforce”意味着用户只能进行身份验证以将Sales Insight Actions与Salesforce结合使用。 它是Sales Insight Actions实例的默认选择，之所以推荐，是因为它允许用户无缝进行身份验证，而无需管理用户名和密码。

### 选择“仅限Salesforce”时，我实例的新用户如何激活其帐户？ {#activate-when-salesforce-only-is-selected}

单击 **快速入门** 邀请电子邮件中的按钮，新用户将被发送到帐户激活屏幕，要求他们连接其Salesforce实例以激活其Sales Insight Actions帐户。

![](assets/login-management-settings-4.png)

### 选择“仅限Salesforce”时，允许我的用户使用哪些身份验证方法进行身份验证？ {#what-authentication-methods}

导航到我们的登录屏幕时，用户将首先输入其电子邮件地址。 然后，他们将单击Salesforce一键登录按钮，在该按钮中，他们可以使用登录到的Salesforce帐户进行身份验证。

>[!NOTE]
>
>这仅适用于直接导航到登录屏幕的用户。 从Salesforce访问Actions的用户将登录 [自动登录](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### 当用户从Salesforce访问“操作”功能且选择了“仅限Salesforce”时，如何处理“操作”的用户身份验证？ {#how-is-user-authentication-handled}

当用户单击其中一个操作（“呼叫”、“电子邮件”、“促销活动”、“任务”、“促销活动列表”等）时，我们将使用其SFDC身份验证自动将其登录到其“销售分析操作”帐户。 我们称之为身份验证 [自动登录](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## 所有登录方法常见问题解答 {#all-login-methods-faq}

### 选择“所有登录方法”后，新用户如何激活其帐户？ {#activate-when-all-login-methods-is-selected}

邀请新用户访问实例时，他们将收到一封帐户激活电子邮件。 他们将单击显示“开始”的按钮，然后进入要求他们创建和确认密码的页面。 创建此之后，将激活其帐户，并通过载入工作流引导他们。

![](assets/login-management-settings-6.png)

### 选择“所有登录方法”后，我的实例的用户可以使用哪些登录？ {#what-are-users-allowed-to-log-in-with-all-login}

使用我们的登录页面时，用户将首先输入其电子邮件地址。 然后，他们将被发送到一个页面，该页面为他们提供了所有登录选项（用户名/密码、SFDC、Gmail、SSO），以便进行身份验证。

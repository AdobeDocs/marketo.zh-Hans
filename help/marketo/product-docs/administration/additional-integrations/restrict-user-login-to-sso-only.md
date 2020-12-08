---
unique-page-id: 2360358
description: 仅限用户登录到SSO - Marketo Docs —— 产品文档
title: 仅限用户登录到SSO
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# 仅限用户登录到SSO {#restrict-user-login-to-sso-only}

如果您使用 [SSO](add-single-sign-on-to-a-portal.md) ，并且希望确保用户无法绕过SSO安全，请按照以下说明操作。

>[!NOTE]
>
>**需要管理员权限**

1. 转到“管理员”并单击“登录设置”。

![](assets/image2014-9-24-14-3a44-3a40.png)

1. 单击“编辑安全设置”。

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. 展开高级设置，选中“需要SSO”，然后单击“保存”。

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!TIP]
>
>如果选 **择Require SSO**，则可以在设置角色时选中Byass [Single Sign-On(绕过单](../../../product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) 一登录)选项，从此限制中排除用户角色 **** 。 这将允许用户正常登录。 例如，管理员用户可能仍需要通过登录屏幕登录到Marketo。

>[!CAUTION]
>
>当新用户被邀请时，他们会收到邀请电子邮件。 但是，如 **果选择** “需要SSO”，则他们将不会收到这些电子邮件，除非他们被分配到设置为“跳过单 **一登录”的角色**。

就这样！ 现在，所有用户（具有绕过单一登录权限的用户除外）将仅限使用SSO登录。
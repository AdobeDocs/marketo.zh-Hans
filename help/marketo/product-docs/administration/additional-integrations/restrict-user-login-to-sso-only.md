---
unique-page-id: 2360358
description: 仅限用户登录SSO - Marketo文档 — 产品文档
title: 仅限用户登录SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# 仅限用户登录SSO {#restrict-user-login-to-sso-only}

如果您是 [使用SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) 并且要确保用户无法绕过SSO安全，请按照以下说明操作。

>[!IMPORTANT]
>
>本文不适用于 [已启用Adobe IMS](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Marketo订阅。

>[!NOTE]
>
>**需要管理员权限**

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. 单击 **[!UICONTROL 登录设置]s**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. 单击 **[!UICONTROL 编辑安全设置]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. 展开 **[!UICONTROL 高级]** 设置，检查 **[!UICONTROL 需要SSO]**，然后单击 **[!UICONTROL 保存]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>最佳做法是邀请用户并接受邀请。 _晚于_ 邀请被接受，管理员随后应将其设置为&quot;[!UICONTROL 需要SSO].”

>[!TIP]
>
>如果您选择 **[!UICONTROL 需要SSO]**，您可以排除 [用户角色](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) 通过检查 **[!UICONTROL 绕过单点登录]** 选项。 这将允许用户正常登录。 例如，管理员用户可能仍需要通过登录屏幕登录Marketo。

>[!CAUTION]
>
>邀请新用户时，他们将收到邀请电子邮件。 但是，如果 **[!UICONTROL 需要SSO]** 选中时，用户不会收到这些电子邮件，除非将其分配给设置为的角色 **[!UICONTROL 绕过单点登录]**.

就是这样！ 现在，所有用户（有权绕过单点登录的用户除外）都将被限制为仅使用SSO登录。

>[!MORELIKETHIS]
>
>* [将单点登录添加到门户](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [使用通用ID进行订阅登录](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [使用通用ID将Marketo用户邀请到两个实例](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

---
unique-page-id: 2360358
description: 限制用户仅登录SSO - Marketo Docs — 产品文档
title: 限制用户仅登录SSO
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---


# 限制用户仅登录SSO {#restrict-user-login-to-sso-only}

如果您[使用SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)，并且希望确保用户无法绕过SSO安全，请按照以下说明操作。

>[!NOTE]
>
>**需要管理权限**

1. 转至&#x200B;**Admin**&#x200B;并单击&#x200B;**登录设置**。

   ![](assets/image2014-9-24-14-3a44-3a40.png)

1. 单击&#x200B;**编辑安全设置**。

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. 展开“高级设置”，选中“**需要SSO**”，然后单击“**保存**”。

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!NOTE]
>
>最佳实践是邀请用户并接受邀请。 _接_ 受邀请后，管理员应将其设置为“需要SSO”。

>[!TIP]
>
>如果选择&#x200B;**要求SSO**，则可以在设置角色时选中&#x200B;**绕过单点登录**&#x200B;选项，从此限制中排除[用户角色](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md)。 这将允许用户正常登录。 例如，管理员用户可能仍需要通过登录屏幕登录Marketo。

>[!CAUTION]
>
>当新用户被邀请时，他们会收到邀请电子邮件。 但是，如果选择了&#x200B;**要求SSO**，则他们将不会收到这些电子邮件，除非他们被分配到设置为&#x200B;**绕过单点登录**&#x200B;的角色。

就这样！ 现在，所有用户（具有绕过单一登录权限的用户除外）将仅限使用SSO登录。

>[!MORELIKETHIS]
>
>* [将单一登录添加到门户](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [使用通用ID进行订阅登录](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [邀请Marketo用户使用具有通用ID的两个实例](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)


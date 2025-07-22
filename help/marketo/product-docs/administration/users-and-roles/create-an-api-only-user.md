---
unique-page-id: 2360207
description: 创建仅API用户 — Marketo文档 — 产品文档
title: 创建仅API用户
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
feature: Users and Roles
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 2%

---

# 创建仅API用户 {#create-an-api-only-user}

如果您要通过[REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}与Marketo集成，则需要创建一个“仅限API用户”。 具体方法如下。

>[!IMPORTANT]
>
>如果您在已登记到Adobe Identity的订阅中创建“仅限API用户”，则您的步骤不同，可从此处[找到](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}。

>[!PREREQUISITES]
>
>[创建仅API用户角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**需要管理员权限**

1. 转到&#x200B;**[!UICONTROL Admin]**&#x200B;区域。

   ![](assets/create-an-api-only-user-1.png)

1. 单击 **[!UICONTROL Users & Roles]**。

   ![](assets/create-an-api-only-user-2.png)

1. 单击 **[!UICONTROL Invite New User]**。

   ![](assets/create-an-api-only-user-3.png)

1. 为仅API用户输入电子邮件、名字和姓氏。 单击 **[!UICONTROL Next]**。

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >添加可选的[!UICONTROL Reason]或[!UICONTROL Access Expiration]日期。 访问过期日期对于短期员工来说是方便的。

1. 选择&#x200B;**[!UICONTROL API Only]**&#x200B;角色并选中&#x200B;**[!UICONTROL API Only]**&#x200B;复选框。 单击 **[!UICONTROL Next]**。

   ![](assets/create-an-api-only-user-5.png)

1. 单击 **[!UICONTROL Send]**。

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>弹出窗口显示，“不仅API需要邀请”，但这并不表示您做了错事。 这仅仅意味着我们将创建角色，而无需发送邀请电子邮件。

那好吧！ 现在，让我们来创建自定义服务。

>[!MORELIKETHIS]
>
>[创建用于REST API的自定义服务](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}

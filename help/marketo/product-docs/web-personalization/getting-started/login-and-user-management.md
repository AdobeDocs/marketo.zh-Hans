---
unique-page-id: 7513771
description: 登录和用户管理 — Marketo文档 — 产品文档
title: 登录与用户管理
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 3%

---

# 登录与用户管理 {#login-and-user-management}

## 创建[!UICONTROL Web Personalization]用户角色 {#create-a-web-personalization-user-role}

1. 转到&#x200B;**[!UICONTROL Admin]**&#x200B;部分，然后单击&#x200B;**[!UICONTROL Users & Roles]**。

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. 单击 **[!UICONTROL Roles]**。

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >如果Web Personalization (WP)用户角色已存在，请确保已按照步骤4中所示对其进行配置。

1. 单击 **[!UICONTROL New Role]**。

   ![](assets/three-1.png)

1. 输入[!UICONTROL Role Name]并选择[!UICONTROL Permissions]。 单击&#x200B;**[!UICONTROL Create]** （此角色必须[应用于所有工作区](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)）。

   ![](assets/four.png)

   >[!TIP]
   >
   >要授予用户访问“定位”和“Personalization”中所有内容的权限，请务必选中&#x200B;_所有_&#x200B;复选框。

## [!UICONTROL Web Personalization]和预测内容用户权限 {#web-personalization-and-predictive-content-user-permissions}

**[!UICONTROL Targeting and Personalization]**：如果仅选择此权限，则用户具有仅查看权限。

**[!UICONTROL Admin Web Personalization + Predictive]**：用户只能访问Web Personalization和预测内容应用程序的“帐户设置”和“内容设置”。 用户可以在应用程序中查看页面，但没有创建、编辑、删除和启动权限。

**[!UICONTROL Predictive Content Editor]**：用户具有预测内容应用程序的编辑器访问权限。 该权限允许创建、编辑和删除内容片段。 不允许在Web或电子邮件中启用预测性使用内容。

**[!UICONTROL Predictive Content Launcher]**：用户有权访问除“帐户”和“内容设置”之外的所有预测内容功能。 该权限允许创建、编辑和删除以及启用内容片段。

**[!UICONTROL Web Campaign Editor]**：用户具有所有Web Personalization功能的编辑器访问权限，以便创建、编辑和删除但不启动Web营销活动。

**[!UICONTROL Web Campaign Launcher]**：用户有权访问除“帐户”和“内容设置”之外的所有Web Personalization应用程序功能。 该权限允许创建、编辑、删除和启动Web营销活动。

## 将WP角色分配给用户 {#assign-wp-role-to-user}

1. 转到&#x200B;**[!UICONTROL Users]**。

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. 选择要授予WP访问权限的用户，然后单击&#x200B;**[!UICONTROL Edit User]**。

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. 为所有工作区选择WP用户角色。

   ![](assets/seven.png)

1. 新启用的用户下次登录时将在“我的Marketo”中看到&#x200B;**[!UICONTROL Web Personalization]**&#x200B;磁贴。

   ![](assets/eight.png)

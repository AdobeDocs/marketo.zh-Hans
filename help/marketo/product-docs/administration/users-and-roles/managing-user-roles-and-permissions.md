---
unique-page-id: 2359909
description: 管理用户角色和权限 — Marketo文档 — 产品文档
title: 管理用户角色和权限
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
source-git-commit: 2d28d4b473815952231356691b1e9310c61a20f1
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 管理用户角色和权限 {#managing-user-roles-and-permissions}

设置、创建和编辑用户角色，并将其分配给用户。 这样，您就可以控制每个Marketo用户有权访问的区域和功能。

例如，营销用户通常需要在整个应用程序中拥有广泛的访问权限，才能创建、修改和部署电子邮件、登陆页面和程序。 另一方面，Web设计人员几乎将所有时间都花在Design Studio中，创建用于电子邮件和登陆页面的资产。 虽然公司领导在Analytics领域广泛使用Marketo的报告，但他们可能不需要自己创建或推动资源或程序。

>[!NOTE]
>
>**需要管理员权限**

Marketo提供了多个内置角色，具有不同的访问级别：

* **管理员**  — 应用程序的所有部分，包括管理员部分
* **标准用户**  — 应用程序的所有部分，管理部分除外
* **营销用户**  — 应用程序的所有部分，管理部分除外
* **Web设计器**  — 仅设计工作室
* **Analytics用户**  — 仅Analytics部分

您无法编辑管理员和标准用户角色，但可以编辑其他角色。 您还可以创建新的自定义角色，以匹配公司中的特定组织结构。

## 具有Adobe身份的Marketo {#marketo-with-adobe-identity}

如果您正在将Marketo与Adobe身份结合使用，则配置文件描述列表 [可在此处找到](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md#profile-levels).

## 将角色分配给用户 {#assign-roles-to-a-user}

在以下情况下，您可以将角色分配给用户： [首次创建用户](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) 或 [编辑现有用户](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/managing-user-roles-and-permissions-1.png)

1. 单击 **[!UICONTROL 用户和角色]**.

   ![](assets/managing-user-roles-and-permissions-2.png)

1. 从列表中，选择要编辑的用户并单击 **[!UICONTROL 编辑用户]**.

   ![](assets/managing-user-roles-and-permissions-3.png)

1. 下 **[!UICONTROL 角色]**，根据所需的权限，选择要分配给用户的角色，然后单击 **[!UICONTROL 保存]**.

   ![](assets/managing-user-roles-and-permissions-4.png)

   >[!NOTE]
   >
   >要了解每个角色，请参阅 [角色权限描述](/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md).

## 创建新角色 {#create-a-new-role}

有时，贵组织有员工担任非常特定的角色，这些角色需要自定义权限组合。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/managing-user-roles-and-permissions-5.png)

1. 单击 **[!UICONTROL 用户和角色]**.

   ![](assets/managing-user-roles-and-permissions-6.png)

1. 单击 **[!UICONTROL 角色]** 选项卡。

   ![](assets/managing-user-roles-and-permissions-7.png)

1. 单击 **[!UICONTROL 新建角色]**.

   ![](assets/managing-user-roles-and-permissions-8.png)

1. 输入 **[!UICONTROL 角色名称]**， a **[!UICONTROL 描述]** （可选），然后选择此角色中的用户所需的权限。

   ![](assets/managing-user-roles-and-permissions-9.png)

## 编辑角色 {#edit-a-role}

如果需要更改与现有角色关联的权限，可以编辑该角色。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/managing-user-roles-and-permissions-10.png)

1. 单击 **[!UICONTROL 用户和角色]**.

   ![](assets/managing-user-roles-and-permissions-11.png)

1. 单击 **[!UICONTROL 角色]** 选项卡。

   ![](assets/managing-user-roles-and-permissions-12.png)

1. 从列表中，选择要修改的角色，然后单击 **[!UICONTROL 编辑角色]**.

   ![](assets/managing-user-roles-and-permissions-13.png)

1. 更改 **[!UICONTROL 角色名称]** 和 **[!UICONTROL 描述]** （如有必要），然后更改关联的选择 **[!UICONTROL 权限]**.

   ![](assets/managing-user-roles-and-permissions-14.png)

   >[!NOTE]
   >
   >拥有您编辑的角色的用户将在注销并重新登录后收到修改后的权限。

## 删除角色 {#delete-a-role}

如果某个角色变得不必要，您可以将其删除。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/managing-user-roles-and-permissions-15.png)

1. 单击 **[!UICONTROL 用户和角色]**.

   ![](assets/managing-user-roles-and-permissions-16.png)

1. 单击 **[!UICONTROL 角色]** 选项卡。

   ![](assets/managing-user-roles-and-permissions-17.png)

1. 从列表中选择要删除的角色，然后单击 **[!UICONTROL 删除角色]**.

   ![](assets/managing-user-roles-and-permissions-18.png)

1. 单击 **[!UICONTROL 删除]** 以确认。

   ![](assets/managing-user-roles-and-permissions-19.png)

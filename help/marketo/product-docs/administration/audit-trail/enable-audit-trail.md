---
unique-page-id: 11382122
description: 启用审核跟踪 — Marketo文档 — 产品文档
title: 启用审核记录
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
feature: Audit Trail
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# 启用审核记录 {#enable-audit-trail}

审核记录对所有客户都可用，并受两个管理员权限控制。

>[!NOTE]
>
>默认情况下，所有系统管理员角色都启用这两个权限。

## 为角色启用审核跟踪 {#enable-audit-trail-for-a-role}

1. 单击 **[!UICONTROL 管理员]**.

   ![](assets/enable-audit-trail-1.png)

1. 选择 **[!UICONTROL 用户和角色]** 并单击 **[!UICONTROL 角色]**.

   ![](assets/enable-audit-trail-2.png)

1. 选择要为其启用审计追踪的角色，然后单击 **[!UICONTROL 编辑角色]**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >您还可以选择在此创建新角色并授予其审核记录访问权限。

1. 展开 **[!UICONTROL 访问管理员]** 许可。 选择 **[!UICONTROL 访问审核记录]** 和/或 **[!UICONTROL 访问登录历史记录]**，具体取决于您的需求。 单击 **[!UICONTROL 保存]**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**条件**
   >
   >**[!UICONTROL 访问审核记录]**：允许用户同时访问两者 [!UICONTROL 资产审核记录] 和 [!UICONTROL 管理员审核记录].
   >
   >**[!UICONTROL 访问登录历史记录]**：授予用户访问 [用户登录历史记录](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## 将审核跟踪角色分配给用户 {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[创建](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) 或 [启用](#enable-audit-trail) 现有的角色，为其授予审核记录权限。

1. 在 **[!UICONTROL 用户和角色]**，单击 **[!UICONTROL 用户]**.

   ![](assets/enable-audit-trail-5.png)

1. 选择要为其授予审计追踪访问权限的用户，然后单击 **[!UICONTROL 编辑用户]**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >创建新用户时此过程也适用。

1. 选择您创建的审计线索角色。 在此示例中，我们创建了“审核记录 — 资产和管理员”以及“审核记录 — 包含登录历史记录”。

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >如果已启用工作区，请确保选中角色的复选框，该复选框将选择所有工作区。 取消选择单个工作区将隐藏审核跟踪。 这意味着您将看到每个工作区的审核记录数据。 在以下情况下，您可以选择隐藏工作区 [筛选](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. 单击 **[!UICONTROL 保存]**.

   ![](assets/enable-audit-trail-8.png)

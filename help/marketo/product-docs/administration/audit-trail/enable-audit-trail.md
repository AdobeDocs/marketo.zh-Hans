---
unique-page-id: 11382122
description: 启用审核跟踪 — Marketo文档 — 产品文档
title: 启用审核跟踪
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
source-git-commit: 73d41904ca74ae265648c3ed91805be7c4d24fe0
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# 启用审核跟踪 {#enable-audit-trail}

审核跟踪可供所有客户使用，并由两个管理员权限控制。

>[!NOTE]
>
>默认情况下，所有系统管理员角色都启用了这两个权限。

## 为角色启用审核跟踪 {#enable-audit-trail-for-a-role}

1. 单击 **管理员**.

   ![](assets/enable-audit-trail-1.png)

1. 选择 **用户和角色** 单击 **角色**.

   ![](assets/enable-audit-trail-2.png)

1. 选择要为其启用审核跟踪的角色，然后单击 **编辑角色**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >您还可以选择在此处创建新角色并授予其“审核记录”访问权限。

1. 展开 **访问管理员** 权限。 选择 **访问审核记录** 和/或 **访问登录历史记录**，具体取决于您的需求。 单击 **保存**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**条件**
   >
   >**访问审核跟踪：** 允许用户同时访问资产审核跟踪和管理员审核跟踪。
   >
   >**访问登录历史记录：** 授予用户访问 [用户登录历史记录](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## 将审核记录角色分配给用户 {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[创建](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) 或 [启用](#enable-audit-trail) 现有角色，授予其“审核记录”权限。

1. 在 **用户和角色**，单击 **用户**.

   ![](assets/enable-audit-trail-5.png)

1. 选择要授予审核记录访问权限的用户，然后单击 **编辑用户**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >创建新用户时，此过程也适用。

1. 选择您创建的“审核记录”角色。 在此示例中，我们创建了“审核跟踪 — 资产和管理员”和“审核跟踪 — 具有登录历史记录”。

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >如果已启用工作区，请确保选中角色的复选框，此复选框将选择所有工作区。 取消选择单个工作区将隐藏审核跟踪。 这意味着您将看到每个工作区的审核记录数据。 在 [过滤](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. 单击 **保存**.

   ![](assets/enable-audit-trail-8.png)

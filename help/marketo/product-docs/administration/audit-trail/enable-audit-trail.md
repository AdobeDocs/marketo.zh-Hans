---
unique-page-id: 11382122
description: 启用审核跟踪- Marketo Docs —— 产品文档
title: 启用审核跟踪
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# 启用审核跟踪 {#enable-audit-trail}

审核跟踪对所有客户可用，并受两个管理权限控制。

>[!NOTE]
>
>默认情况下，所有系统管理员角色都启用了这两个权限。

## 为角色启用审核跟踪 {#enable-audit-trail-for-a-role}

1. 单击 **管理**。

   ![](assets/one-2.png)

1. 选择“ **用户和角色** ”，然后 **单击“角色**”。

   ![](assets/two-2.png)

1. 选择要为其启用审核跟踪的角色，然后单击“编 **辑角色”**。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >您还可以选择在此处创建新角色并授予其“审核跟踪”访问权限。

1. 展开“访 **问管理** ”权限。 根据 **您的需要** ，选择“访 **问审核跟踪”和／或“访**&#x200B;问登录历史记录”。 单击 **保存**。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >**定义**
   >
   >
   >**访问审核跟踪：** 允许用户同时访问资产审核跟踪和管理员审核跟踪。
   >
   >
   >**访问登录历史记录：** 允许用户访问用 [户登录历史](user-login-history.md)。

## 为用户分配审核跟踪角色 {#assign-audit-trail-role-to-a-user}

>[!NOTE]
>
>**先决条件**
>
>[创建](http://docs.marketo.com/display/DOCS/Create,+Delete,+Edit+and+Change+a+User+Role#Create,Delete,EditandChangeaUserRole-CreateaRole) 或启 [用现有](#Enable) 角色，为其授予“审核跟踪”权限。

1. 在“ **用户和角色**”中，单 **击“用户**”。

   ![](assets/five-1.png)

1. 选择要授予审核跟踪访问权限的用户，然后单击“编 **辑用户”**。

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >创建新用户时也会应用此过程。

1. 选择您创建的审核跟踪角色。 在此示例中，我们创建了“审核跟踪——资产和管理员”和“审核跟踪——登录历史记录”。

   ![](assets/seven-1.png)

   >[!CAUTION]
   >
   >如果已启用工作区，请确保选中角色的复选框，该复选框将选择所有工作区。 取消选择单个工作区将隐藏审核跟踪。 这意味着您将看到每个工作区的审核跟踪数据。 筛选时，您确实可以选择隐藏工 [作区](http://docs.marketo.com/display/DOCS/Filtering+in+Audit+Trail)。

1. 单击 **保存**。

   ![](assets/eight-1.png)


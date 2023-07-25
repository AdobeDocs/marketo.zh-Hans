---
unique-page-id: 7513771
description: 登录和用户管理 — Marketo文档 — 产品文档
title: 登录和用户管理
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# 登录和用户管理 {#login-and-user-management}

## 创建Web个性化用户角色 {#create-a-web-personalization-user-role}

1. 转到 **管理员** 部分，然后单击 **用户和角色**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. 单击 **角色**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >如果Web个性化(WP)用户角色已存在，请确保已按照步骤4中所示对其进行配置。

1. 单击 **新建角色**.

   ![](assets/three-1.png)

1. 输入角色名称并选择权限。 单击 **创建** (此角色必须 [应用于所有工作区](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md))。

   ![](assets/four.png)

   >[!TIP]
   >
   >要授予用户访问“定位”和“个性化”中所有内容的权限，请务必选择 _所有_ 复选框。

## Web个性化和预测内容用户权限 {#web-personalization-and-predictive-content-user-permissions}

**定位和个性化**：用户具有仅查看权限（如果仅选择此权限）。

**管理Web个性化+预测**：用户只能访问Web个性化和预测内容应用程序的“帐户设置”和“内容设置”。 用户可以查看应用程序中的页面，但没有创建、编辑、删除和启动权限。

**预测内容编辑器**：用户具有预测内容应用程序的编辑器访问权限。 该权限允许创建、编辑和删除内容片段。 不允许在Web或电子邮件上启用预测性使用内容。

**预测内容启动器**：用户有权访问所有预测内容功能，但帐户和内容设置除外。 该权限允许创建、编辑和删除以及启用内容片段。

**Web营销活动编辑器**：用户具有所有Web个性化功能的编辑访问权限，这些功能可用于创建、编辑和删除但不启动Web营销活动。

**Web营销活动启动器**：用户有权访问所有Web个性化应用程序功能，但帐户和内容设置除外。 该权限允许创建、编辑、删除和启动Web营销活动。

## 将WP角色分配给用户 {#assign-wp-role-to-user}

1. 转到 **用户**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. 选择要向其授予WP访问权限的用户，然后单击 **编辑用户**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. 为所有工作区选择WP用户角色。

   ![](assets/seven.png)

1. 新启用的用户将看到 **Web个性化** Marketo图块。

   ![](assets/eight.png)

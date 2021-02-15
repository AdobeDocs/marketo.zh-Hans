---
unique-page-id: 7513771
description: 登录和用户管理 — Marketo Docs — 产品文档
title: 登录和用户管理
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---


# 登录和用户管理{#login-and-user-management}

## 创建Web个性化用户角色{#create-a-web-personalization-user-role}

1. 转到&#x200B;**Admin**&#x200B;部分，然后单击&#x200B;**用户和角色**。

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. 单击&#x200B;**角色**。

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >如果Web个性化(WP)用户角色已存在，请确保已按照步骤4中的说明进行配置。

1. 单击&#x200B;**新建角色**。

   ![](assets/three-1.png)

1. 输入角色名称，然后选择权限。 单击&#x200B;**创建**（此角色必须[应用于所有工作区](https://docs.marketo.com/display/DOCS/Managing+Marketo+Users#ManagingMarketoUsers-CreateUsers)）。

   ![](assets/four.png)

   >[!TIP]
   >
   >要向用户授予访问“定位和个性化”中所有内容的权限，请确保选中&#x200B;*所有*&#x200B;复选框。

## Web个性化和预测内容用户权限{#web-personalization-and-predictive-content-user-permissions}

**定位和个性化**:如果仅选择了此权限，则用户只具有视图权限。

**管理Web个性化+预测**:用户只能访问Web个性化和预测内容应用程序的帐户设置和内容设置。用户可以视图应用程序中的页面，但没有创建、编辑、删除和启动权限。

**预测内容编辑器**:用户具有对“预测内容”应用程序的编辑器访问权限。该权限允许创建、编辑和删除内容片段。 它不允许在Web或电子邮件上启用“预测”内容。

**预测内容启动器**:除“帐户”和“内容设置”外，用户可以访问所有“预测内容”功能。该权限允许创建、编辑、删除和启用内容片段。

**Web活动编辑器**:用户可以访问所有Web个性化功能的编辑器，以创建、编辑和删除Web活动，但不能启动Web个性化。

**Web活动启动器**:用户有权访问除“帐户”和“内容设置”之外的所有Web个性化应用程序功能。该权限允许创建、编辑、删除和启动Web活动。

## 为用户{#assign-wp-role-to-user}分配WP角色

1. 转到&#x200B;**Users**。

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. 选择要授予WP访问权限的用户，然后单击&#x200B;**编辑用户**。

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. 为所有工作区选择WP用户角色。

   ![](assets/seven.png)

1. 新启用的用户在下次登录时将在My Market中看到&#x200B;**Web Personalization**&#x200B;拼贴。

   ![](assets/eight.png)

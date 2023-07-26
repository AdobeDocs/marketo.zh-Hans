---
unique-page-id: 10095429
description: 修复Dynamics验证同步问题 — Marketo文档 — 产品文档
title: 修复Dynamics验证同步问题
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 修复Dynamics验证同步问题 {#fix-dynamics-validation-sync-issues}

## 验证同步工具结果 {#validate-sync-tool-results}

运行Dynamics Validate Sync时，它将生成一个报表。 如果有 ![x](assets/delete.png) 在步骤旁边，请参阅以下选项以识别和修复问题。 然后，重新运行同步验证步骤，直到结果仅显示绿色复选标记。

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL有效 {#url-is-valid}

如果您拥有 ![x](assets/delete.png) 在此处，验证URL是否有效。 请在此处开发人员资源中找到该内容，然后查看组织服务。 URL可能由于多种原因而无效。

1. 登录到Dynamics。 单击设置图标并选择 **高级设置**.

   ![](assets/one.png)

1. 单击设置，然后选择 **自定义**.

   ![](assets/two.png)

1. 单击 **开发人员资源**.

   ![](assets/three.png)

1. 可以在服务端点下找到组织服务URL。

   ![](assets/four.png)

## 用户名和密码有效 {#username-and-password-are-valid}

如果您拥有 ![x](assets/delete.png) 在此处，验证您的Microsoft Dynamics凭据是否有效。 对于Web API S2S身份验证，Marketo中的用户名必须匹配 [电子邮件地址](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) CRM中应用程序用户的个人资料。 对于其他类型，它应该与同步用户的用户名匹配。

## 已将同步用户分配给Marketo同步用户角色 {#sync-user-is-assigned-to-the-marketo-sync-user-role}

如果您拥有 ![x](assets/delete.png) 在此，它可能是以下三个问题之一。

**选项一 — 验证是否已在Microsoft Dynamics中选中Marketo同步用户角色**：

1. 在Dynamics中，单击“设置”图标并选择 **高级设置**.

   ![](assets/one.png)

1. 单击 **设置** 并选择 **安全性**.

   ![](assets/six.png)

1. 单击 **用户。**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. 单击同步用户的链接。

   ![](assets/seven.png)

1. 单击 **管理角色**.

   ![](assets/eight.png)

1. 验证是否已选中Marketo同步用户角色。 如果没有，选中它并单击 **好的。**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**选项二 — 确认授予同意**：

1. 查看 [同意客户端ID和应用程序注册](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) 以确认应用程序同意调用API。

**选项3 — 同步用户**：

1. 验证是否已将同步用户添加到Marketo配置。

## Marketo解决方案安装正确 {#marketo-solution-is-properly-installed}

如果您拥有 ![x](assets/delete.png) 此处，转到Microsoft Dynamics以验证是否安装了Marketo。 请参阅Microsoft Dynamics设置文档中的步骤1。

1. 在Dynamics中，单击“设置”图标并选择 **高级设置**.

   ![](assets/one.png)

1. 单击 **设置** 并选择 **解决方案。**

   ![](assets/eleven.png)

1. 验证是否列出了解决方案。

   ![](assets/twelve.png)

## 解决方案中的所有步骤均已启用 {#all-steps-in-the-solution-are-enabled}

如果您拥有 ![x](assets/delete.png) 在此处，验证是否未停用任何默认步骤。 所有步骤在安装时自动启用，但在自定义过程中可以停用它们。

## 同步用户已分配给Marketo解决方案 {#sync-user-is-assigned-to-the-marketo-solution}

如果您拥有 ![x](assets/delete.png) 在此，确保已在Microsoft Dynamics的Marketo默认页面上分配了同步用户。

1. 在Dynamics中，单击“设置”图标并选择 **高级设置**.

   ![](assets/one.png)

1. 单击 **设置** 并选择 **Marketo配置**.

   ![](assets/thirteen.png)

1. 验证是否已将同步用户指定为默认用户。

   ![](assets/fourteen.png)

## 同步用户匹配用户名和密码 {#sync-user-matches-username-and-password}

如果您拥有 ![x](assets/delete.png) 在此，请确保在Microsoft Dynamics的Marketo配置默认设置步骤的Marketo用户字段中分配正确的同步用户。

>[!MORELIKETHIS]
>
>[验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)

---
unique-page-id: 10095429
description: 修复了Dynamics验证同步问题 — Marketo文档 — 产品文档
title: 修复了Dynamics验证同步问题
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
source-git-commit: b4fafa28d9a38504a29c25700496d8376c4fe47b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 修复了Dynamics验证同步问题 {#fix-dynamics-validation-sync-issues}

## 验证同步工具结果 {#validate-sync-tool-results}

运行Dynamics验证同步时，会生成一个报表。 如果有 ![x](assets/delete.png) 在步骤旁边，请参阅以下选项以识别并修复问题。 然后，重新运行同步验证步骤，直到结果只显示绿色复选标记。

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL有效 {#url-is-valid}

如果您有 ![x](assets/delete.png) 在此，验证URL是否有效。 请在此处的开发人员资源中找到它，然后查看组织服务。 该URL可能由于多种原因而无效。

1. 登录到Dynamics。 单击“设置”图标，然后选择 **高级设置**.

   ![](assets/one.png)

1. 单击设置，然后选择 **自定义**.

   ![](assets/two.png)

1. 单击 **开发人员资源**.

   ![](assets/three.png)

1. 组织服务URL可在服务端点下找到。

   ![](assets/four.png)

## 用户名和密码有效 {#username-and-password-are-valid}

如果您有 ![x](assets/delete.png) 在此，验证您的Microsoft Dynamics用户名和密码是否有效。

## 同步用户被分配给Marketo同步用户角色 {#sync-user-is-assigned-to-the-marketo-sync-user-role}

如果您有 ![x](assets/delete.png) 在这里，这可能是以下两个原因之一。

**选项1 — 验证是否在Microsoft Dynamics中选中Marketo同步用户角色**:

1. 在Dynamics中，单击设置图标，然后选择 **高级设置**.

   ![](assets/one.png)

1. 单击 **设置** 选择 **安全性**.

   ![](assets/six.png)

1. 单击 **用户。**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. 单击同步用户的链接。

   ![](assets/seven.png)

1. 单击 **管理角色**.

   ![](assets/eight.png)

1. 验证是否已选中Marketo同步用户角色。 如果没有，请检查它并单击 **好。**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**选项2 — 确认授予同意**:

1. 查看 [授予客户ID和应用程序注册的同意](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) ，以确认应用程序是否同意调用API。

## Marketo解决方案安装正确 {#marketo-solution-is-properly-installed}

如果您有 ![x](assets/delete.png) 在此，转到Microsoft Dynamics以验证Marketo安装是否存在。 请参阅Microsoft Dynamics设置文档的步骤1。

1. 在Dynamics中，单击设置图标，然后选择 **高级设置**.

   ![](assets/one.png)

1. 单击 **设置** 选择 **解决方案。**

   ![](assets/eleven.png)

1. 验证是否已列出解决方案。

   ![](assets/twelve.png)

## 解决方案中的所有步骤均已启用 {#all-steps-in-the-solution-are-enabled}

如果您有 ![x](assets/delete.png) 在此，请确认未停用任何默认步骤。 所有步骤在安装时自动启用，但可以在自定义过程中停用它们。

## 同步用户已分配给Marketo解决方案 {#sync-user-is-assigned-to-the-marketo-solution}

如果您有 ![x](assets/delete.png) 在此，请确保在Microsoft Dynamics的“Marketo默认”页面上分配了同步用户。

1. 在Dynamics中，单击设置图标，然后选择 **高级设置**.

   ![](assets/one.png)

1. 单击 **设置** 选择 **Marketo配置**.

   ![](assets/thirteen.png)

1. 验证是否将同步用户分配为默认用户。

   ![](assets/fourteen.png)

## 同步用户与用户名和密码匹配 {#sync-user-matches-username-and-password}

如果您有 ![x](assets/delete.png) 在此，请确保在Microsoft Dynamics的Marketo配置默认设置步骤的Marketo用户字段中分配正确的同步用户。

>[!MORELIKETHIS]
>
>[验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)

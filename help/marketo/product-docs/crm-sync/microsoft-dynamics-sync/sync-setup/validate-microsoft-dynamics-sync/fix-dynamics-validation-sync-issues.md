---
unique-page-id: 10095429
description: 修复Dynamics验证同步问题 — Marketo Docs — 产品文档
title: 修复Dynamics验证同步问题
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 修复Dynamics验证同步问题{#fix-dynamics-validation-sync-issues}

## 验证同步工具结果{#validate-sync-tool-results}

运行Dynamics验证同步时，它会生成此报表。 如果步骤旁边有![delete](assets/delete.png)，请参见下面以确定并修复问题。 然后重新运行同步验证步骤，直到结果显示的只有复选标记。

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL有效{#url-is-valid}

如果此处有![delete](assets/delete.png)，请验证URL是否有效。 在开发人员资源中找到它，然后查看组织服务。 URL可能无效，原因有多。

1. 登录到Dynamics。 单击“设置”图标，然后选择&#x200B;**高级设置**。

   ![](assets/one.png)

1. 单击“设置”，然后选择“**自定义**”。

   ![](assets/two.png)

1. 单击&#x200B;**Developer Resources**。

   ![](assets/three.png)

1. 可以在服务端点下找到组织服务URL。

   ![](assets/four.png)

## 用户名和密码有效{#username-and-password-are-valid}

如果此处有![—](assets/delete.png)，请验证您的Microsoft Dynamics用户名和密码是否有效。

## 将同步用户分配给Marketo Sync用户角色{#sync-user-is-assigned-to-the-marketo-sync-user-role}

如果您在此处拥有![—](assets/delete.png)，则需要验证Marketo Sync用户角色是否已在Microsoft Dynamics中选中。 请参阅Microsoft Dynamics安装文档的步骤2。

1. 在Dynamics中，单击“设置”图标，然后选择&#x200B;**高级设置**。

   ![](assets/one.png)

1. 单击&#x200B;**设置**&#x200B;并选择&#x200B;**安全**。

   ![](assets/six.png)

1. 单击&#x200B;**用户。**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. 单击同步用户的链接。

   ![](assets/seven.png)

1. 单击&#x200B;**管理角色**。

   ![](assets/eight.png)

1. 验证是否已选中Marketo同步用户角色。 如果没有，请检查它，然后单击&#x200B;**确定。**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## Marketo解决方案已正确安装{#marketo-solution-is-properly-installed}

如果此处有![—](assets/delete.png)，请转到Microsoft Dynamics，以验证Marketo安装是否存在。 请参阅Microsoft Dynamics设置文档的步骤1。

1. 在Dynamics中，单击“设置”图标，然后选择&#x200B;**高级设置**。

   ![](assets/one.png)

1. 单击&#x200B;**设置**&#x200B;并选择&#x200B;**解决方案。**

   ![](assets/eleven.png)

1. 验证已列出解决方案。

   ![](assets/twelve.png)

## 解决方案中的所有步骤均已启用{#all-steps-in-the-solution-are-enabled}

如果此处有![—](assets/delete.png)，请验证所有默认步骤均未停用。 安装时会自动启用所有步骤，但在自定义过程中可取消激活这些步骤。

## 将同步用户分配给Marketo解决方案{#sync-user-is-assigned-to-the-marketo-solution}

如果此处有![—](assets/delete.png)，请确保在Microsoft Dynamics的“Marketo默认”页上分配了“同步”用户。

1. 在Dynamics中，单击“设置”图标，然后选择&#x200B;**高级设置**。

   ![](assets/one.png)

1. 单击&#x200B;**设置**&#x200B;并选择&#x200B;**Marketo Config**。

   ![](assets/thirteen.png)

1. 验证是否将同步用户分配为默认用户。

   ![](assets/fourteen.png)

## 同步用户与用户名和密码{#sync-user-matches-username-and-password}匹配

如果您在此处拥有![—](assets/delete.png)，请确保在Microsoft Dynamics的Marketo配置默认设置步骤的“Marketo用户”字段中分配正确的同步用户。

>[!MORELIKETHIS]
>
>[验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)

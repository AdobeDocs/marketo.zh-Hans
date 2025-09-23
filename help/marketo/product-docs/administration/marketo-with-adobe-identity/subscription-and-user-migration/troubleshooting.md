---
description: Adobe IMS用户迁移疑难解答指南 — Marketo文档 — 产品文档
title: Adobe IMS用户迁移疑难解答指南
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# Adobe IMS用户迁移疑难解答指南 {#adobe-ims-user-migration-troubleshooting-guide}

在IMS用户迁移过程中，将为每个要迁移的Adobe用户创建一个Marketo Engage用户（除非该用户已存在且电子邮件地址相同）。 有时不会创建它，这可能是由用户在Active Directory中的记录或电子邮件地址问题造成的。

对于执行自迁移的用户，本文列出了您在自迁移控制台的状态字段中可能会看到的每个错误消息。

>[!NOTE]
>
>目录/域相关的错误可以由另一个已设置目录信任或声明了域的org/Admin Console触发。

## 错误消息 {#error-messages}

首先，确定是否需要迁移用户，因为这将影响要遵循的解决步骤。

使用右侧的“在此页面上”部分直接跳转到特定错误。

### Gmail无效字符 {#gmail-invalid-character}

**根本原因**：根据Adobe安全策略，Gmail电子邮件地址中不允许使用字符`.`和`+`。 非Gmail电子邮件地址中允许使用这两个字符。

**分辨率**：

_如果用户需要迁移_ — 电子邮件地址必须在Marketo Engage中更新，以符合Adobe安全策略并进行还原。 Marketo管理员，然后从迁移控制台为此用户重新运行用户迁移。

_如果用户&#x200B;**不**&#x200B;需要迁移_ - Marketo Engage管理员在迁移控制台中跳过该用户。 如果通过迁移或跳过来考虑所有用户，则会显示“迁移完成”按钮。 单击按钮以结束用户迁移过程。

### 用户不在目录中 {#user-not-in-directory}

**根本原因**：用户在Active Directory (AD)中不存在。 对于已启用AD同步且采用SSO的任何组织，只允许通过身份提供程序(IdP)创建用户。 因此，在用户迁移期间无法通过Admin Console添加用户。

**分辨率**：

_如果需要迁移用户_ — 系统管理员必须以适当的权限将该用户添加到Active Directory。 Marketo Engage管理员，然后从迁移控制台为此用户重新运行用户迁移。

_如果用户&#x200B;**不**&#x200B;需要迁移_ - Marketo Engage管理员在迁移控制台中跳过该用户。 如果通过迁移或跳过来考虑所有用户，则会显示“迁移完成”按钮。 单击按钮以结束用户迁移过程。

### 非活动用户 {#inactive-user}

**根本原因**： AD同步已启用，用户的联合帐户存在，但处于非活动/禁用状态。

**分辨率**：

_如果需要迁移用户_ — 系统管理员必须还原用户的状态和适当的权限。 Marketo Engage管理员，然后从迁移控制台为此用户重新运行用户迁移。

_如果用户&#x200B;**不**&#x200B;需要迁移_ - Marketo Engage管理员在迁移控制台中跳过该用户。 如果通过迁移或跳过来考虑所有用户，则会显示“迁移完成”按钮。 单击按钮以结束用户迁移过程。

### 无效域 {#invalid-domain}

**根本原因**：已在Admin Console中启用域强制。 但是，用户电子邮件地址的域不是允许的域之一，或者已在其他组织/Admin Console中声明了该域。

**分辨率**：

_如果用户需要迁移_（并且在迁移组织中启用了域实施） — 必须在Marketo Engage中更新电子邮件地址以符合域实施(DE)策略。 或者，系统管理员可以[将域](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"}移动到另一个域实施(DE)禁用的目录，或者[创建一个不在DE策略下的新目录](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。 Marketo Engage管理员，然后从迁移控制台为此用户重新运行用户迁移。

_如果用户需要迁移_（并且已在其他组织中启用域实施） — 已声明域的组织的系统管理员需要将用户的电子邮件地址添加到异常列表。 Marketo Engage管理员，然后从迁移控制台为此用户重新运行用户迁移。

_如果用户&#x200B;**不**&#x200B;需要迁移_ - Marketo Engage管理员在迁移控制台中跳过该用户。 如果通过迁移或跳过来考虑所有用户，则会显示“迁移完成”按钮。 单击按钮以结束用户迁移过程。

### Type2E失败 {#type2e-failure}

**根本原因**：如果为组织配置了联盟帐户(T3)，并且用户已存在单个帐户(T1)，则任何创建（如果适用）并将仅授权帐户(T2e)链接到联盟帐户的尝试都将失败，错误代码为FAILED_TO_CREATE_TYPE2E_USER。

**分辨率**：

1. 从Adobe组织中删除单个用户。 _请注意：用户将失去对所有产品的访问权限，需要稍后重新授权。 如果这样不好，请联系Adobe支持部门。_
1. 重新运行用户迁移，以便为此用户创建联合用户帐户。
1. 将创建仅授权帐户（如果适用）并将其链接到联合帐户作为其身份验证帐户。

**了解详情**
* [设置标识而不使用单点登录](https://helpx.adobe.com/enterprise/using/set-up-identity.html#:~:text=Set%20up%20identity%20without%20Single%20Sign%2DOn)
* [使用单点登录设置身份](https://helpx.adobe.com/enterprise/using/set-up-identity.html#:~:text=Set%20up%20identity%20with%20Single%20Sign%2DOn)

### Pendo迁移失败 {#pendo-migration-failed}

**根本原因**：用户的联合帐户处于非活动状态/已禁用，或者在Active Directory (AD)中缺失。

**分辨率**：

_如果需要迁移用户_

1. 系统管理员必须恢复用户的帐户状态和权限。

1. 对于具有AD同步的SSO组织：

   * 通过身份提供程序(IdP)创建用户。
   * 同步用户数据与AD。

1. 对于没有SSO/AD同步的组织：

   * 重新创建托管帐户以恢复状态。
   * 组织管理员必须重新分配角色和权限。

1. Marketo Engage管理员会在迁移控制台中重新运行迁移。

1. 如果控制台无法访问，请联系[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support)以重新运行迁移。

_如果用户&#x200B;**不**&#x200B;需要迁移_

* Marketo Engage管理员应在迁移控制台中跳过用户。
* 迁移或跳过所有用户后，单击&#x200B;**[!UICONTROL Migration Complete]**&#x200B;以完成。
* 如果错误仍然存在，请将包含相关详细信息的支持案例提交给[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support)。


### 用户创建失败 {#user-creation-failed}

[请参阅下文](#failed)

### Marketo授权失败 {#marketo-entitlement-failed}

[请参阅下文](#failed)

### 用户数据迁移失败 {#user-data-migration-failed}

[请参阅下文](#failed)

### 产品数据同步失败 {#product-data-sync-failed}

[请参阅下文](#failed)

### Adobe授权失败 {#adobe-entitlement-failed}

[请参阅下文](#failed)

### 用户注销失败 {#user-sign-out-failed}

[请参阅下文](#failed)

### Adobe ID创建失败 {#adobe-id-creation-failed}

[请参阅下文](#failed)

### 失败 {#failed}

**根本原因**：这些错误可能是由后端中的各种原因造成的。

**分辨率**：

提交支持案例，其中包含[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}的相关详细信息。

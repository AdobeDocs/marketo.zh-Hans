---
description: Adobe IMS用户迁移疑难解答指南 — Marketo文档 — 产品文档
title: Adobe IMS用户迁移疑难解答指南
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e95748ed9a26f5454c342c6f6a9c29ec687c7cad
workflow-type: tm+mt
source-wordcount: '877'
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

**根本原因**：在用户迁移期间创建联合用户帐户（用于单点登录）失败，因为与单个用户相同的电子邮件地址已存在Adobe ID。

**分辨率**：

1. 从Adobe组织中删除单个用户。 请注意：用户将失去对所有产品的访问权限，需要稍后重新获得授权。
1. 重新运行用户迁移，以便为此用户创建联合用户帐户。
1. 将用户添加回他们之前有权访问的产品。

### 用户创建失败 {#user-creation-failed}

[请参阅下文](#failed)

### Marketo授权失败 {#marketo-entitlement-failed}

[请参阅下文](#failed)

### Pendo迁移失败 {#pendo-migration-failed}

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

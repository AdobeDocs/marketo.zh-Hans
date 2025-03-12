---
description: Adobe IMS用户迁移疑难解答指南 — Marketo文档 — 产品文档
title: Adobe IMS用户迁移疑难解答指南
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e96bc8676a73694ec60f46bb045f2a6ea5d8069c
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Adobe IMS用户迁移疑难解答指南 {#adobe-ims-user-migration-troubleshooting-guide}

在IMS用户迁移过程中，将为每个要迁移的Adobe用户创建一个Marketo Engage用户（除非该用户已存在且电子邮件地址相同）。 有时不会创建它，这可能是由用户在Active Directory中的记录或电子邮件地址问题造成的。 发生这种情况时，Marketo Engage管理员将在自迁移控制台中的用户迁移状态字段中看到原因。

## 错误消息 {#error-messages}

首先，确定是否需要迁移用户，因为这将影响要遵循的解决步骤。

使用右侧的“在此页面上”部分直接跳转到特定错误。

### 不在目录中 {#not-in-directory}

**根本原因**：用户在Active Directory (AD)中不存在。 对于已启用AD同步且采用SSO的任何组织，只允许通过身份提供程序(IdP)创建用户。 因此，在用户迁移期间无法通过Admin Console添加用户。

**分辨率**：

_如果不需要迁移用户_ - Marketo Engage管理员在迁移控制台中跳过该用户。 如果通过迁移或跳过来考虑所有用户，则会显示“迁移完成”按钮。 单击按钮以结束用户迁移过程。

_如果确实需要迁移用户_ — 系统管理员必须以适当的权限将该用户添加到Active Directory。 Marketo Engage管理员，然后从迁移控制台为此用户重新运行用户迁移。

### Gmail无效字符 {#gmail-invalid-character}

**根本原因**：根据Adobe安全策略，Gmail电子邮件地址中不允许使用字符`.`和`+`。 非Gmail电子邮件地址中允许使用这两个字符。

**分辨率**：

_如果不需要迁移用户_ - Marketo Engage管理员在迁移控制台中跳过该用户。 如果通过迁移或跳过来考虑所有用户，则会显示“迁移完成”按钮。 单击按钮以结束用户迁移过程。

_如果用户确实需要迁移_ — 电子邮件地址必须在Marketo Engage中更新，以符合Adobe的安全策略并进行还原。 Marketo管理员，然后从迁移控制台为此用户重新运行用户迁移。

### 非活动用户 {#inactive-user}

**根本原因**： AD同步已启用，用户的联合帐户存在，但处于非活动/禁用状态。

**分辨率**：

_如果不需要迁移用户_ - Marketo Engage管理员在迁移控制台中跳过该用户。 如果通过迁移或跳过来考虑所有用户，则会显示“迁移完成”按钮。 单击按钮以结束用户迁移过程。

_如果确实需要迁移用户_ — 必须还原用户的状态和适当的权限。 Marketo Engage管理员，然后从迁移控制台为此用户重新运行用户迁移。

### 不在域中 {#not-in-domain}

**根本原因**：已在Admin Console中启用域实施，但用户电子邮件地址的域不是允许的域之一。

**分辨率**：

_如果不需要迁移用户_ - Marketo Engage管理员在迁移控制台中跳过该用户。 如果通过迁移或跳过来考虑所有用户，则会显示“迁移完成”按钮。 单击按钮以结束用户迁移过程。

_如果用户确实需要迁移_ — 电子邮件地址必须在Marketo Engage中更新以符合域实施(DE)策略。 或者，系统管理员可以[将域](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"}移动到另一个域强制执行(DE)禁用的目录，或者[创建一个不在DE策略下的新目录](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。 Marketo Engage管理员，然后从迁移控制台为此用户重新运行用户迁移。

### 创建失败 {#create-failure}

**根本原因**：此错误可能是由后端中的各种原因造成的。

**分辨率**：

提交支持案例，其中包含[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}的相关详细信息。

### Type2e用户失败 {#type2e-user-failure}

**根本原因**：此错误可能是由后端中的各种原因造成的。

**分辨率**：

提交支持案例，其中包含[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}的相关详细信息。

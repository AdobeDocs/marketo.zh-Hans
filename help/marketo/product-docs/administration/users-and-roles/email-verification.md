---
description: 电子邮件验证 — Marketo文档 — 产品文档
title: 电子邮件验证
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# 电子邮件验证 {#email-verification}

Adobe Marketo Engage订阅要求所有非API用户验证其电子邮件地址，包括Marketo Engage管理员。 为未分配管理员角色或分配了“略过SSO”权限的角色的单一登录(SSO)用户启用了电子邮件验证功能后，其订阅将自动进行电子邮件验证。

## 为什么引入此功能 {#why-this-feature-was-introduced}

Marketo Engage正在继续推出电子邮件验证，以便为将客户迁移到Adobe业务平台做准备，包括迁移到AdobeID。 此功能增强了现有Marketo Engage用户帐户的安全性。 要确保Marketo Engage用户与适当的Adobe ID相关联，现有Marketo Engage用户必须验证其电子邮件地址。 Marketo Engage用户必须具有经验证的电子邮件地址才能迁移到Adobe ID。 如果Marketo Engage用户不验证其电子邮件地址，则无法将其迁移到Adobe ID，并且在用户迁移到Marketo订阅完成后，他们将失去对该订阅的访问权限。

## 用户邀请 {#user-invite}

当管理员邀请用户时，该用户在单击邀请链接后将自动验证。 未分配管理员角色的SSO用户将被自动验证。

## 验证电子邮件 {#verification-email}

在为订阅激活电子邮件验证时，或者由管理员/用户触发时，用户将收到以下电子邮件：

![](assets/email-verification-1.png)

>[!NOTE]
>
>要向未验证的用户重新发送验证电子邮件，只需选择用户的记录并单击 **[!UICONTROL 验证电子邮件]** 按钮。

## 更改电子邮件地址 {#changing-an-email-address}

更改用户的电子邮件地址后，该地址将变为未验证状态。 将向他们发送电子邮件，以便他们重新验证。 用户可以通过单击手动重新发送该电子邮件 **[!UICONTROL 重新发送验证]**.

![](assets/email-verification-2.png)

![](assets/email-verification-3.png)

## 用户和角色 {#users-and-roles}

在 **[!UICONTROL 管理员]** > **[!UICONTROL 用户和角色]**，电子邮件状态列显示每个用户的验证状态。

![](assets/email-verification-4.png)

## 多个用户登录ID {#multiple-user-login-ids}

只有一个用户帐户可以与单个电子邮件地址关联。 如果有多个用户帐户与单个电子邮件地址关联，则Marketo Engage需要解决冲突，并显示与该电子邮件地址关联的所有用户登录，以及三个解决选项：

* 使用当前电子邮件作为当前用户登录ID
* 使用新电子邮件作为当前用户登录ID
* 将决策延迟到下次登录

  ![](assets/email-verification-5.png)

>[!NOTE]
>
>用户帐户必须与单个地址关联，但可以通过通用ID在多种订阅中使用用户帐户。

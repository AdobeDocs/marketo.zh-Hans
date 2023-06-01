---
description: 电子邮件验证 — Marketo文档 — 产品文档
title: 电子邮件验证
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: e104a8bd41d61451202ba089512dc688680292ce
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# 电子邮件验证 {#email-verification}

Adobe Marketo Engage订阅要求所有非API用户(包括Marketo Engage管理员)验证其电子邮件地址。 为未分配管理员角色或分配了“略过SSO”权限角色的单点登录(SSO)用户启用电子邮件验证功能后，将自动验证其订阅。

## 用户邀请 {#user-invite}

当管理员邀请用户时，该用户单击邀请链接后将自动进行验证。 未分配管理员角色的SSO用户将被自动验证。

## 验证电子邮件 {#verification-email}

受邀用户将收到以下电子邮件：

![](assets/email-verification-1.png)

>[!NOTE]
>
>要将验证电子邮件重新发送给未验证用户，只需选择其记录并单击 **验证电子邮件** 按钮。

## 更改电子邮件地址 {#changing-an-email-address}

当用户的电子邮件地址发生更改时，它将变为未验证。 将向他们发送电子邮件，以便他们重新验证。 用户可以通过单击手动重新发送该电子邮件 **重新发送验证**.

![](assets/email-verification-2.png)

![](assets/email-verification-3.png)

## 用户和角色 {#users-and-roles}

In **管理员** > **用户和角色**，电子邮件状态列显示每个用户的验证状态。

![](assets/email-verification-4.png)

## 多个用户登录ID {#multiple-user-login-ids}

只有一个用户帐户可以与单个电子邮件地址关联。 如果有多个用户帐户与单个电子邮件地址关联，则Marketo Engage需要解决冲突，并显示与该电子邮件地址关联的所有用户登录，以及三个解决方法选项：

* 使用当前电子邮件作为当前用户登录ID
* 使用新电子邮件作为当前用户登录ID
* 将决策延迟到下次登录

   ![](assets/email-verification-5.png)

>[!NOTE]
>
>虽然用户帐户必须与单个地址关联，但用户帐户可以通过通用ID用于多个订阅。

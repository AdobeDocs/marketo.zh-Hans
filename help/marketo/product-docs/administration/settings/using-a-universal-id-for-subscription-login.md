---
unique-page-id: 10100311
description: 使用通用ID进行订阅登录 — Marketo文档 — 产品文档
title: 使用通用ID进行订阅登录
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
source-git-commit: d5c1c1d0ce2a521898eaa4f6610bf1ce04b4f66b
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# 使用通用ID进行订阅登录 {#using-a-universal-id-for-subscription-login}

通用ID允许您通过一次登录访问多个Marketo订阅，并快速在订阅之间切换。 但是，如果您需要，可以对订阅使用不同的登录方式。

借助通用ID，您仍可以为每个订阅创建支持票证。

使用通用ID（例如，角色、权限和密码策略）的用户接受订阅级别设置。 用户配置文件级别的更改会反映在所有订阅中，例如名字、姓氏和电子邮件地址。

## 设置通用ID {#setting-up-a-universal-id}

所有Marketo订阅均附带可选的通用ID功能。 从每个实例中，Marketo管理员必须通过相同的登录邀请您访问每个不同的订阅。 Marketo无法自动合并您现有的登录。

>[!NOTE]
>
>如果您有多个订阅登录ID，则还可能有多个社区用户档案。 请务必为与您要使用的用户档案关联的通用ID选择ID，该ID适用于您的生产实例，而不是沙盒。

## 登录 {#logging-in}

当您登录以使用通用ID接受第二次订阅的邀请时，您将看到选择加入登录页面。 在此，您必须选中复选框以接受条款和条件。 接受后，您将看到任何后续登录的正常重置页面，而不是此页面。 通过接受条款和条件，您允许Marketo将您的基本配置文件数据（如名字、姓氏和电子邮件地址）分发到托管订阅的不同位置的数据中心。

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>除非订阅管理员删除这些ID，否则您不再使用的ID将保留。 我们建议您保留这些ID，以防万一您有一个分配给自己的私人报表，且该报表只能使用该ID访问。 在这种情况下，将这些专用报表移动到新的通用ID中，然后删除现有ID是合理的。

## 密码 {#passwords}

通过对多个订阅使用通用ID，Marketo自动强制实施最严格的密码策略。 例如，如果某些订阅需要最小密码长度，而其他订阅则不需要，则所有订阅都将强制使用最小长度。

使用适用于多个订阅的通用ID，只有您才能更改密码。

>[!NOTE]
>
>如果当前订阅的密码不符合其受邀参加的第二个订阅的密码策略，Marketo将要求那些希望使用通用ID来重置密码的用户。

## 在订阅之间切换 {#switching-between-subscriptions}

使用通用ID，您可以查看您登录的订阅，并选择您有登录访问权限的其他订阅。 在大多数情况下，您无需注销即可在它们之间进行切换。

![](assets/image2016-11-3-15-3a10-3a16.png)

当您注销并重新登录时，Marketo会自动将您登录到您上次登录的订阅。 然后，您可以根据需要切换到其他订阅。

## 社区用户档案 {#community-profiles}

如果您有多个订阅，则可能有多个社区用户档案。 我们建议您选择与您最活跃的社区用户档案关联的登录。

## 移动平台 {#mobile-platform}

具有通用ID的用户可以从他们上次登录的订阅中查看其关于Marketo时刻和iPad事件签入应用程序的数据。 您无法从移动平台本身更改订阅。

>[!MORELIKETHIS]
>
>* [将单点登录添加到门户](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [限制用户仅登录SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [邀请Marketo用户加入两个具有通用ID的实例](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)


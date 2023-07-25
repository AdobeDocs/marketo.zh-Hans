---
unique-page-id: 10100311
description: 使用通用ID进行订阅登录 — Marketo文档 — 产品文档
title: 使用通用ID进行订阅登录
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
feature: Administration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# 使用通用ID进行订阅登录 {#using-a-universal-id-for-subscription-login}

通用ID允许您通过一次登录访问多个Marketo订阅，并快速在订阅之间切换。 但是，您可以根据需要对订阅使用不同的登录。

使用通用ID，您仍然可以为每个单独订阅创建支持工单。

使用通用ID的用户（例如角色、权限和密码策略）将遵循订阅级别设置。 用户配置文件级别更改会反映在所有订阅中，例如名字、姓氏和电子邮件地址。

## 设置通用ID {#setting-up-a-universal-id}

所有Marketo订阅都附带可选的通用ID功能。 对于每个实例，Marketo管理员必须使用相同的登录名邀请您使用各个订阅。 Marketo无法自动合并您的现有登录。

>[!NOTE]
>
>如果您有多个订阅登录ID，则可能还拥有多个社区配置文件。 请确保为连接到要使用的配置文件的通用ID选择ID，该ID适用于生产实例，而不是沙盒。

## 登录 {#logging-in}

当您使用通用ID登录以接受第二个订阅的邀请时，您将看到选择加入登录页面。 在此，您必须选中复选框以接受条款和条件。 接受后，您将看到任何后续登录的常规重置页面，而不是此页面。 通过接受这些条款和条件，您将允许Marketo将您的基本配置文件数据（如名字、姓氏和电子邮件地址）分发到托管您的订阅的其他位置的数据中心。

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>您不再使用的ID将保留，除非订阅管理员删除它们。 例如，如果您有一个分配给自己的私人报告，且该报告只能使用该ID访问，我们建议您保留这些报告。 在这种情况下，将这些专用报表移动到新的通用ID，然后删除现有ID是合理之举。

## 密码 {#passwords}

通过为多个订阅使用通用ID，Marketo会自动实施最严格的密码策略。 例如，如果某些订阅需要最小密码长度，而其他订阅则不需要，则将对所有订阅强制执行最小长度。

使用多个订阅的通用ID，只有您可以更改密码。

>[!NOTE]
>
>如果当前订阅的密码不符合邀请他们访问的第二个订阅的密码策略，Marketo将要求希望使用通用ID的用户重置密码。

## 在订阅之间切换 {#switching-between-subscriptions}

使用通用ID，您可以查看已登录的订阅，并选择您有权登录的其他订阅。 在大多数情况下，您无需注销再重新登录，即可在它们之间切换。

![](assets/image2016-11-3-15-3a10-3a16.png)

当您注销并重新登录时，Marketo会自动将您登录到上次登录的订阅。 然后，您可以根据需要切换到其他订阅。

## 社区配置文件 {#community-profiles}

如果您有多个订阅，则可能有多个社区用户档案。 我们建议您选择与最活跃的社区用户档案关联的登录名。

## 移动平台 {#mobile-platform}

具有通用ID的用户可以从他们上次登录的订阅的Marketo Ments和iPad事件签入应用程序中查看其数据。 您无法从Mobile平台本身更改订阅。

>[!MORELIKETHIS]
>
>* [将单点登录添加到门户](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [仅限用户登录SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [使用通用ID将Marketo用户邀请到两个实例](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

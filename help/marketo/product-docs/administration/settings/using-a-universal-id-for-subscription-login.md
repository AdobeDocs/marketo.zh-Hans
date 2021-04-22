---
unique-page-id: 10100311
description: 使用通用ID进行订阅登录 — Marketo文档 — 产品文档
title: 使用通用ID进行订阅登录
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 使用通用ID进行订阅登录{#using-a-universal-id-for-subscription-login}

通用ID允许您通过一次登录访问多个Marketo订阅，并在订阅之间快速切换。 但是，如果您愿意，您可以对订阅使用不同的登录名。

借助Universal ID，您仍然可以为每个订阅创建支持票证。

订阅级别设置适用于使用通用ID的用户，例如角色、权限和口令策略。 用户用户档案级别的更改反映在所有订阅中，例如名、姓和电子邮件地址。

## 设置通用ID {#setting-up-a-universal-id}

从每个实例中，Marketo管理员必须邀请您使用相同的登录名访问各个不同订阅。 Marketo无法自动合并您现有的登录名。 启用通用ID后，**您的Marketo实例将在最多30分钟内不可用**。 如果您的用户群更大，则可能会更长一些。

>[!CAUTION]
>
>如果为用户启用了“单个ID”或“通用ID”，则用户的角色和工作区可以在初始设置后&#x200B;**不**&#x200B;进行编辑。

>[!NOTE]
>
>如果您有多个订阅登录ID，则可能还有多个社区用户档案。 请务必为连接到要使用的用户档案的通用ID选择ID，而这是针对生产实例而非沙箱的。

## 登录{#logging-in}

当您登录以使用通用ID接受第二个订阅的邀请时，您将看到选择登录页面。 在此，您必须选中复选框以接受条款和条件。 接受后，您将看到任何后续登录的普通重置页面，而不是此页面。 接受条款和条件后，即允许Marketo将您的基本用户档案数据（如名、姓和电子邮件地址）分发到订阅托管位置不同的数据中心。

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>除非订阅管理员删除您不再使用的ID。 我们建议您保留这些ID，以防您有一个分配给自己的私人报告，只能使用该ID访问。 在这种情况下，将这些私有报表移到新的通用ID，然后删除现有ID是有意义的。

## 密码{#passwords}

借助通用ID，Marketo可以针对多个订阅自动实施最严格的密码策略。 例如，如果某些订阅需要最小密码长度，而其他订阅不需要，则所有将强制使用最小密码长度。

通用ID适用于多个订阅，只有您可以更改密码。

>[!NOTE]
>
>如果当前订阅的密码不符合其所邀请的第二个订阅的密码策略，Marketo将要求希望使用通用ID的用户重置其密码。

## 在订阅{#switching-between-subscriptions}之间切换

使用通用ID，您可以看到您登录的订阅，并选择您有权登录的其他订阅。 在大多数情况下，您无需注销或重新登录即可在它们之间切换。

![](assets/image2016-11-3-15-3a10-3a16.png)

当您注销并重新登录时，Marketo会自动将您登录到您上次登录的订阅。 然后，如有必要，您可以切换到其他订阅。

## 社区用户档案{#community-profiles}

如果您有多个订阅，则可能有多个社区用户档案。 我们建议您选择与您最活跃的社区用户档案关联的登录名。

## 移动平台{#mobile-platform}

具有通用ID的用户可以从上次登录的订阅查看Marketo Moments和iPad事件登记应用程序上的数据。 您无法从移动平台本身更改订阅。

>[!MORELIKETHIS]
>
>* [将单一登录添加到门户](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [限制用户仅登录SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [邀请Marketo用户加入两个具有通用ID的实例](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)


---
description: 了解Marketo订阅和用户迁移到Adobe Admin Console - Marketo文档 — 产品文档
title: 了解Marketo订阅和用户迁移到Adobe Admin Console
hide: true
hidefromtoc: true
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: 234c4548101947a2c5badddeab0532ff727e1f5a
workflow-type: tm+mt
source-wordcount: '1121'
ht-degree: 0%

---

# 了解Marketo订阅和用户迁移到Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe正在改进您管理Adobe Marketo Engage订阅和用户的方式，从而提高您和贵组织的生产效率。 作为此更改的一部分，Adobe正在将您的Marketo Engage订阅和用户迁移到Adobe Admin Console。 这是必需的迁移，不会影响任何营销工作流、内容、集成或资产。

了解如何使用Adobe Admin Console通过管理您整个组织的Adobe权利 [企业和团队管理指南](https://helpx.adobe.com/enterprise/admin-guide.html){target="_blank"}.

## 有什么变化？ {#what-is-changing}

作为迁移的一部分，您的订阅和用户管理将从Marketo应用程序移至Adobe Admin Console。

* **系统管理员将管理Adobe Admin Console上的订阅**. 在一个控制台中查看您的所有Adobe产品。

* **产品管理员将管理用户及其对Adobe Admin Console的访问权限**. 添加和删除所有Adobe订阅的用户。

* **用户将使用Adobe身份登录**. Adobe会将现有用户迁移到Adobe Admin Console。 用户将使用其新的Adobe身份(Adobe ID或AdobeFederated ID(SSO))登录到其Marketo订阅。

* **您管理所有其他功能的方式没有变化** Marketo Engage应用程序本身，包括对功能、用户角色、工作区、功能和行为的管理。


## 迁移历程时间线 {#migration-journey-timeline}

Adobe将首先将Marketo Engage订阅迁移到Adobe Admin Console，然后使用已验证的电子邮件地址迁移所有现有用户。 如果您是系统管理员或Marketo产品管理员，您将收到一封电子邮件，引导您完成迁移历程。 以下是您可以期待的时间表：

### 订阅迁移完成 {#subscription-migration-complete}

迁移到Adobe Admin Console的订阅完成后，系统管理员将收到一封电子邮件。

系统管理员可能需要在用户迁移开始之前完成一些必需步骤，以最大程度地减少对Marketo用户的影响。

* 如果您的Marketo用户当前使用SSO登录，您将需要在Adobe Admin Console上设置SSO，以便您的用户可以继续使用SSO登录。 如果您的Marketo用户当前未使用SSO，但希望在Adobe Admin Console上对其进行设置，则可以在迁移过程中的此时进行设置。

* 如果您已在Adobe Admin Console中管理其他Adobe产品，则Adobe可能会寻求您的同意，以自动将用户迁移到您的现有控制台。 单击电子邮件中的“开始”按钮以导航到同意页面。

用户管理目前没有变化。 Marketo管理员将继续在Marketo管理区域管理用户，并且用户将继续使用其Marketo身份登录，直到其用户迁移完成为止。

### 计划用户迁移 {#schedule-user-migration}

系统管理员完成上一节中所述的先决条件后，Adobe将自动计划提前30天迁移用户，并与Marketo产品管理员沟通以管理用户迁移。

Marketo产品管理员将：

* 提前三十天接收包含计划用户迁移开始日期的电子邮件。

* 获取对位于Marketo管理区域中的Marketo迁移控制台的访问权限，在该控制台中，用户可以更改订阅的迁移日期。

>[!NOTE]
>
>由于迁移的复杂程度，日期更改限制在计划日期后的30天内有效。 如果您需要更晚的日期，请发送电子邮件至marketocares@adobe.com 。

* 查看“我的Marketo”中的横幅，其中显示用户迁移开始日期的倒计时。

* 在用户迁移开始日期的前一天收到提醒电子邮件。

### 准备用户迁移日 {#prepare-users-for-migration-day}

作为Marketo产品管理员，我们建议您确保所有用户都为迁移日期做好准备。

* 在Marketo管理区域检查所有用户的电子邮件验证状态。 鼓励尚未验证电子邮件地址的用户验证其电子邮件地址，并帮助用户解决完成验证过程时遇到的任何挑战

* 为所有用户准备即将迁移到Adobe身份。

>[!NOTE]
>
>在用户迁移时，他们将收到Adobe的电子邮件，通知他们对Marketo登录方式所做的更改。 将邀请用户接受首次使用Adobe身份进行登录的邀请，方法是使用现有Adobe ID登录，或使用同一电子邮件地址设置一个新帐户。

### 迁移日期待完成的任务 {#what-to-expect-on-migration-day}

用户迁移将在Marketo订阅中设置的时区的午夜开始。

**Adobe将首先自动迁移Marketo管理员**. 将Marketo管理员迁移到Adobe身份后，将会在Marketo应用程序中为他们分配Adobe产品管理员角色，以及他们之前具有的任何其他角色。

**如果您的Marketo订阅用户数少于75个**，Adobe将自动迁移其余用户。 此工作流旨在实现最高级别的自动化，以最大程度地减少AdobeMarketo用户的开销。 无需执行任何操作即可执行迁移。

**如果您的Marketo订阅拥有超过75个用户**&#x200B;中，Marketo产品管理员将获得对Marketo迁移控制台的“自助用户迁移”区域的访问权限，该区域位于Marketo管理区域中。 对于在用户迁移过程中需要加强控制的用户，Marketo产品管理员将能够开始批量或一次性选择要迁移的用户。 选择用户后，管理员可以选择“立即迁移”或“计划迁移”以供日后使用，从而让管理员在迁移哪些用户时拥有最大的灵活性和控制能力。

>[!NOTE]
>
>在用户迁移期间，不会失去对产品的访问权限。 如果用户在其迁移期间登录，则在迁移完成后，用户将被注销，并提示用户在几分钟内使用Adobe标识重新登录。

在迁移用户时，他们将会收到Adobe的电子邮件，通知他们登录Marketo的方式发生了更改。 将邀请用户接受首次使用Adobe身份进行登录的邀请，方法是使用现有Adobe ID登录，或使用同一电子邮件地址设置新的Adobe ID。 欲知更多信息，请参阅我们的 [使用Adobe登录的用户](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md) 文章。

## 用户迁移完成 {#user-migration-complete}

迁移所有管理员和用户后，Adobe将通过电子邮件通知所有系统管理员和产品管理员。 此时，该订阅的所有Marketo用户都将使用Adobe身份登录到Marketo，产品管理员将仅在Adobe Admin Console上管理用户。

## 获取支持 {#get-support}

有关您的订阅或用户迁移的其他支持，请发送电子邮件至marketocares@adobe.com。

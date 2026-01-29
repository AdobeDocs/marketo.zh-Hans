---
description: 了解 Marketo 订阅和用户迁移到 Adobe Admin Console — Marketo 文档 — 产品文档
title: 了解 Marketo 订阅和用户迁移到 Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '1571'
ht-degree: 100%

---

# 了解 Marketo 订阅和用户迁移到 Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe 正在改进您管理 Adobe Marketo Engage 订阅和用户的方式，帮助您和您的组织提升工作效率。作为此项改进的一部分，Adobe 正在将您的 Marketo Engage 订阅和用户迁移到 Adobe Admin Console。这是一次必要的迁移，不会影响任何营销工作流程、内容、集成或资源。

>[!TIP]
>
>请参阅[企业和团队管理员指南](https://helpx.adobe.com/cn/enterprise/admin-guide.html){target="_blank"}，了解如何使用 Adobe Admin Console 在整个组织范围内管理您的 Adobe 授权。

## 有哪些变化？ {#what-is-changing}

作为迁移的一部分，您的订阅和用户管理将从 Marketo 应用程序内转移至 Adobe Admin Console。

* **系统管理员将在 Adobe Admin Console 中管理订阅。**&#x200B;在一个控制台中查看所有 Adobe 产品。

* **产品管理员将在 Adobe Admin Console 中管理用户及其访问权限。**&#x200B;可为所有 Adobe 订阅添加或移除用户。Adobe Admin Console 不支持基于用户的访问过期设置。迁移后原本设置了 Marketo Engage 访问过期时间的用户，仍会迁移，并可获得不设过期时间的访问权限。迁移完成后，必须在期望的过期日期当天或之前手动移除这些用户。

* **用户将使用 Adobe Identity 登录。** Adobe 会将现有用户迁移到 Adobe Admin Console。用户将使用新的 Adobe Identity（Adobe ID 或 Adobe Federated ID（SSO））登录其 Marketo 订阅。

* **迁移完成后，URL 将有所不同。** Marketo Engage 将从 experience.adobe.com 迁移至 Adobe Experience Cloud，URL 将采用以下格式：`https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/`（其中 XXX 表示 Munchkin ID，@tenantID 来自您的 Adobe 组织）。您需要与 IT 团队协作，将[本文顶部](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"}列出的所有 Adobe 域名加入允许列表，以避免 Marketo Engage 的访问受到影响。

您的资源 ID 编号将保持不变。而且此前指向 engage-xx.marketo.com 域名下 Marketo Engage 资源的链接和书签&#x200B;_仍将_&#x200B;继续有效。但您必须先登录与该 URL 对应的 Marketo Engage 实例。例如，若要访问 Munchkin ID 为 123-ABC-456 的实例中某个智能营销活动的书签，您需要先登录 Munchkin ID 为 123-ABC-456 的 Marketo Engage 实例。

尽管目前没有相关计划，但未来的开发工作可能会影响此重定向功能。为避免出现意外中断，建议您尽早更新相关书签。

## 哪些内容不会发生变化？ {#what-is-not-changing}

* 在 Marketo Engage 应用程序本身中，**其他所有功能的管理方式均不会发生变化**，包括功能管理、用户角色、工作区、功能以及行为等。本地（仅 API）用户管理仍保留在 Marketo 管理员域中的&#x200B;_用户和角色_&#x200B;选项卡内。

## 迁移流程时间线 {#migration-journey-timeline}

Adobe 将首先把您的 Marketo Engage 订阅迁移到 Adobe Admin Console，然后迁移所有已验证电子邮件地址的现有用户。如果您是系统管理员或 Marketo 产品管理员，您将收到电子邮件，引导您完成整个迁移流程。以下是您可以预期的迁移时间线：

![](assets/understanding-marketo-subscription-and-user-migration-1.png){width="800" zoomable="yes"}

### 订阅迁移完成 {#subscription-migration-complete}

当订阅迁移到 Adobe Admin Console 完成后，System Admin 将收到一封通知电子邮件。

在用户迁移开始之前，系统管理员可能需要完成一些必要步骤，以尽量减少对 Marketo 用户的影响：

* 如果您的 Marketo 用户当前使用 SSO 登录，则需要在 Adobe Admin Console 中配置 SSO，以确保用户仍可通过 SSO 登录。如果您的 Marketo 用户目前尚未使用 SSO，但您希望在 Adobe Admin Console 中启用 SSO，也可以在迁移流程的此阶段进行配置。

* 如果您已在 Adobe Admin Console 中管理其他 Adobe 产品，Adobe 可能会征求您的同意，将用户自动迁移到现有控制台。请点击电子邮件中的 “Get Started” 按钮，前往同意页面。

在此阶段，用户管理方式不会发生变化。尽管 Marketo 产品已显示在 Admin Console 中，但在用户迁移完成之前，Marketo 管理员仍需在 Marketo 管理区域中管理用户，用户也将继续使用其 Marketo 身份登录。在此期间，在用户迁移开始之前，无法在 Admin Console 中管理 Marketo 产品。这也包括与该订阅关联的 Dynamic Chat 实例。

>[!NOTE]
>
>如果您目前尚未使用 SSO，但正在考虑实施，建议在用户迁移开始之前完成配置。如果您希望实施单点登录（SSO），且您的订阅已接入 Adobe Identity 但尚未在 Adobe 组织中实施 SSO，请向 [Marketo 支持](https://nation.marketo.com/){target="_blank"}提交工单，并将主题注明为“在 Admin Console 中管理 Marketo，并实施单点登录（SSO）”。

### 计划用户迁移 {#schedule-user-migration}

在您的系统管理员完成上一节中列出的前提条件后，Adobe 将自动在 30 天后为您安排用户迁移，并与 Marketo 产品管理员沟通以推进用户迁移相关事宜。

Marketo 产品管理员将：

* 在用户迁移开始日期前 30 天收到一封电子邮件，告知其已安排的用户迁移开始时间。

* 获得对 Marketo Migration Console（位于 Marketo 管理员区域内）的访问权限，并可在其中选择更改订阅的迁移日期。

>[!NOTE]
>
>由于迁移过程较为复杂，迁移日期的更改最多只能延后不超过原定日期的 30 天。如果需要更晚的迁移日期，请发送电子邮件至 `marketocares@marketo.com`。

* 在 My Marketo 中看到一个横幅，显示距离用户迁移开始日期的倒计时。

* 在用户迁移开始日期的前一天收到一封提醒电子邮件。

### 为迁移日做好用户准备 {#prepare-users-for-migration-day}

作为 Marketo 产品管理员，建议您确保所有用户都已为迁移日做好准备。

* 在 Marketo 管理员区域中检查所有用户的[电子邮件验证](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"}状态。鼓励尚未完成电子邮件验证的用户尽快完成验证，并协助用户解决验证过程中遇到的任何问题。

* 在您的电子邮件收件箱中搜索包含“已锁定”的用户通知。建议已被锁定的用户在迁移日前重置其密码，以重新获得对 Marketo Engage 的访问权限。

* 为即将迁移至 Adobe Identity 提前做好所有用户的准备工作。

>[!IMPORTANT]
>
>如果 Marketo Engage 用户在用户迁移时尚未完成电子邮件验证，或其帐户处于锁定状态，该用户将不会被迁移至 Adobe ID，并将在该订阅的迁移完成后失去对 Marketo 的访问权限。如需恢复访问权限，Marketo 产品管理员需要将该用户作为新用户重新添加。

### 迁移当天须知 {#what-to-expect-on-migration-day}

所有使用美国时区的 Marketo 订阅，将在迁移开始日期的太平洋标准时间（PST）午夜开始迁移。所有其他订阅的用户迁移，将在其订阅所指定时区的午夜开始。

**Adobe 将首先自动迁移 Marketo 管理员（具有标准管理员角色的用户）**。当 Marketo 管理员以 Admin Console 产品管理员角色迁移至 Adobe Identity 后，他们将在 Marketo 应用程序中分配获得 Adobe 产品管理员角色，同时保留其之前拥有的所有其他角色。

**如果您的 Marketo 订阅在 Marketo 和/或 Adobe 组织中未启用 SSO**，Adobe 将自动迁移其余所有用户。该流程旨在实现高度自动化，从而最大限度地减少 Adobe Marketo 用户的运维负担。您无需执行任何操作即可完成迁移。

**如果您的 Marketo 订阅在 Marketo 和/或 Adobe 组织中启用了 SSO**，Marketo 管理员将获得对 Marketo 迁移控制台中“自助式用户迁移”区域的访问权限，该控制台位于 Marketo 管理员区域内。对于在用户迁移过程中需要更高控制度的情况，Marketo 管理员可以选择分批迁移用户，或一次性迁移全部用户。在选定用户后，管理员可以选择“立即迁移”或“计划在稍后日期迁移”，从而对迁移哪些用户以及迁移时间实现最大程度的灵活控制。

>[!NOTE]
>
>在用户迁移期间，不会影响对产品的访问。如果用户在其帐户迁移过程中仍处于登录状态，该用户将会自动登出，并在迁移完成后的几分钟内收到提示使用 Adobe Identity 重新登录。用户必须点击成功完成用户迁移后发送的授权电子邮件中的链接，以接受邀请。

在用户完成迁移后，他们将收到一封来自 Adobe 的电子邮件，通知其 Marketo 登录方式已发生变更。用户&#x200B;**必须**&#x200B;在首次使用 Adobe Identity 登录时接受邀请，可选择使用现有的 Adobe ID 登录，或使用相同的电子邮件地址创建新的 Adobe ID。

更多信息请参阅[迁移至 Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}、[使用 Adobe 进行用户登录](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}以及 [Adobe Identity Management 常见问题](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}。

## 用户迁移完成 {#user-migration-complete}

当所有管理员和用户均完成迁移后，Adobe 将通过电子邮件通知所有系统管理员和产品管理员。此时，该订阅下的所有 Marketo 用户都将使用 Adobe Identity 登录 Marketo，产品管理员仅可在 Adobe Admin Console 中管理用户。

## 获取支持 {#get-support}

如需获取有关订阅或用户迁移的进一步支持，请发送电子邮件至 `marketocares@marketo.com`。

>[!MORELIKETHIS]
>
>* [迁移至 Adobe Identity 概述](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [使用 Adobe ID 进行用户登录](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [Adobe Identity Management 常见问题解答](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
>* [迁移至 Adobe Identity Management 教程](https://experienceleague.adobe.com/zh-hans/docs/marketo-learn/tutorials/fundamentals/migrating-to-adobe-identity-management){target="_blank"}

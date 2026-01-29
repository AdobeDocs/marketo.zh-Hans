---
description: Adobe Identity Management 常见问题解答 — Marketo 文档 — 产品文档
title: Adobe Identity Management 常见问题解答
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 95ed91736b7276dd7a5b9e09958c1f09832ae719
workflow-type: ht
source-wordcount: '1579'
ht-degree: 100%

---

# Adobe Identity Management 常见问题解答 {#adobe-identity-management-faq}

**什么是 Adobe Identity？**

Adobe Identity Management System 由三个组件组成。

* [!DNL Adobe Identity Service]：负责最终用户的身份验证与校验，包括联合身份以及运行时单点登录（SSO）。

* Adobe Admin Console：Admin Console 为您在整个组织范围内管理 Adobe 授权提供统一入口。它支持用户管理、云服务管理、桌面许可证授权、联合身份配置，并提供数据防泄露（DLP）安全功能。

* Adobe 用户管理 API（UMAPI）：允许组织通过 API 在 Adobe Admin Console 中管理企业用户及其授权。

**现有的 Marketo Engage 订阅何时会集成到 IMS？**

现有的 Marketo Engage 订阅目前会在发生任何销售事件时迁移到 Adobe IMS，包括续约、重新签约和/或合同补充协议等情形。自 2024 年 10 月起，也支持在非销售事件场景下进行迁移。

**迁移后，Marketo Engage 的 URL 会保持不变吗？**

不会。迁移后，URL 将呈现为以下格式：`https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/`（其中 XXX 表示 Munchkin ID，@tenantID 来自您的 Adobe 组织）。

**我们是否需要为 URL 的更改提前做些什么准备？**

是的。迁移完成后，Marketo Engage 将从原先的 experience.adobe.com 迁移到 Adobe Experience Cloud 提供服务。您需要与 IT 团队协作，将[本文顶部](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"}列出的所有 Adobe 域名加入允许列表，以避免 Marketo Engage 的访问受到影响。

此前指向 engage-xx.marketo.com 域名下 Marketo Engage 资源的链接和书签&#x200B;_仍将_&#x200B;继续有效。但您必须先登录与该 URL 对应的 Marketo Engage 实例。例如，若要访问 Munchkin ID 为 123-ABC-456 的实例中某个智能营销活动的书签，您需要先登录 Munchkin ID 为 123-ABC-456 的 Marketo Engage 实例。

尽管目前没有相关计划，但未来的开发工作可能会影响此重定向功能。为避免出现意外中断，建议您尽早更新相关书签。

**这是否支持 SSO？**

是的。与 Adobe IMS 的集成支持通用 ID 用户和 SSO。SSO 现由 Adobe IMS 统一驱动，并在 Adobe Admin Console 中以组织级别进行配置。不过，与 Adobe 的 SP 发起型支持相比，Marketo Engage 的 IdP 发起型支持存在一些差异（[了解更多](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}）。如果您在迁移至 Admin Console 后需要了解有关 SSO 差异的帮助，请联系 [Adobe 客户关怀团队](https://helpx.adobe.com/cn/contact.html){target="_blank"}。

**Adobe 产品管理员与 Marketo Engage 管理员有什么区别？**

* Adobe 产品管理员是 Marketo 平台中的一个新角色。
* 添加为 Adobe Admin Console 中产品管理员的用户，将获得 Adobe 产品管理员角色。
* Adobe 产品管理员是只读角色，无法在 Marketo Engage 中进行编辑或删除。
* Adobe 产品管理员拥有与标准 Marketo 管理员相同的权限与特权。
* Marketo Engage 管理员仍然是一个管理员角色，并在 Marketo Engage 中直接授予用户。
* 只有拥有 Marketo 默认管理员角色的用户，才会在 Admin Console 中分配成为 Marketo 产品管理员。

**用户管理 API 的客户端支持是否有变化？**

是的。已接入 Adobe IMS 的用户将无法继续使用所有现有的 Marketo 用户管理 API。在用户邀请、更新和删除等操作中，应改用 Adobe 的 [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"}。在角色管理方面，仍然使用 Marketo 用户管理 API。除此之外，Marketo REST API 的客户端支持不再有其他变化。

**如果已集成 IMS，应联系谁获取支持？**

* 用户迁移前：可在 [Marketing Nation 社区](https://nation.marketo.com/t5/support/ct-p/Support)提交支持工单，或发送电子邮件至 `customercare@marketo.com`

* 用户迁移后：可在 [Marketing Nation 社区](https://nation.marketo.com/t5/support/ct-p/Support)提交支持工单，或发送电子邮件至 `customercare@marketo.com`

* 支持迁移完成后：产品支持管理员可通过 Experience League 支持门户提交工单。

如果您拥有 Ultimate Success 服务，则可使用 Admin Console 迁移的白手套服务。如需协助，请联系 Adobe 客户团队（您的客户经理）。

**如果我使用 Adobe Identity 访问其他 Adobe 应用程序，是否也可以用来访问 Marketo？**

即使您已在使用其他 Adobe 产品，在订阅迁移到 IMS 之前，仍无法使用 Adobe Identity 访问 Marketo。

**Marketo 中（工作区内）的用户角色是否在 Adobe Admin Console 中管理？**

不是。用户角色管理（工作区内）仍在 Marketo Engage 中完成。

**我是 IMS 集成订阅中的 Marketo 管理员，但无法访问 Admin Console。如何获取访问权限？**

任何拥有您组织 Admin Console 访问权限的 Adobe 系统管理员或产品管理员，都可以为您授予访问权限。如果不确定组织内谁拥有控制台管理员权限，请联系 [Adobe 客户关怀团队](https://helpx.adobe.com/cn/contact.html){target="_blank"}。

**管理员如何向 Marketo [!DNL Sales Connect] 添加用户？**

尽管 Admin Console 中会显示 [!DNL Sales Connect] 的产品卡片，但不应通过 Admin Console 添加或管理用户。管理员可通过以下链接在 Marketo [!DNL Sales Connect] 中管理用户：[https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}。

**我可以在哪里进一步了解 Adobe Admin Console？**

[https://helpx.adobe.com/cn/enterprise/admin-guide.html](https://helpx.adobe.com/cn/enterprise/admin-guide.html){target="_blank"}。

**我是否仍需前往 Marketo 的“管理员”区域来修改用户帐户？**

不需要，您需要前往 [account.adobe.com](https://account.adobe.com){target="_blank"}。

**这与 Marketo 的通用 ID 如何配合使用？**

已接入 Adobe Identity 的用户，可通过产品内的订阅切换器无缝访问所有已启用 IMS 的订阅。

**这是否支持 SSO？**

是的。Marketo 与 Adobe IMS 的集成支持通用 ID 用户和 SSO。SSO 现由 Adobe IMS 统一驱动，并在 Adobe Admin Console 中以组织级别进行配置。[在此处了解详情](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

**我已经接入 Adobe Identity，现在想要实施 SSO。我该怎么办？**

如果您希望实施单点登录（SSO），且您的订阅已接入 Adobe Identity 但尚未在 Adobe 组织中实施 SSO，请向 [Marketo 支持](https://nation.marketo.com/){target="_blank"}提交工单，并将主题注明为“在 Admin Console 中管理 Marketo，并实施单点登录（SSO）”。

**设备授权是如何运作的？**

Adobe IMS 目前不支持类似 Marketo 设备授权的功能。

**是否仍可以使用“邀请用户对话框中的登录名”功能，使用户登录名不同于其电子邮件地址？**

不可以。当订阅启用 IMS 后，用户邀请流程将不再生效，因此该功能也不再可用。Adobe Identity 要求以用户的电子邮件地址作为其身份标识。

**在 Adobe IMS 中，是否可以选择使用 Adobe ID、Enterprise ID 或 Federated ID？**

可以，您可以自行决定组织所支持的身份类型。更多信息请参阅：[身份概述](https://helpx.adobe.com/cn/enterprise/using/identity.html)以及[设置身份](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

**Adobe Admin Console 支持哪些产品卡片？**

支持的产品卡片包括：Marketo Engage、Marketo Measure、Marketo Dynamic Chat、Marketo Sales Connect，以及 Marketo Sales Insight Actions。

**如果在迁移到 Adobe Identity 后，我的用户登录名与电子邮件地址不一致，会发生什么情况？**

当前 Marketo Engage 用户如果其登录名与电子邮件地址不同，在迁移到 Adobe Identity 后将无法再使用该登录凭据登录。Adobe Identity 始终使用用户的电子邮件地址进行身份验证。您可以在 [account.adobe.com](https://account.adobe.com){target="_blank"} 更新 Adobe Identity 的电子邮件地址。

**如果我的订阅使用了 IP 限制设置，Adobe Identity 迁移后会发生什么？**

您当前的 IP 限制将在 2026 年第一季度之前继续生效（适用于在迁移前已启用该设置的订阅）。这些限制同样适用于 Adobe ID 用户，因此您的访问控制将继续按预期工作。

自 2026 年第一季度起，旧版 IP 限制将会弃用。此后，基于 IP 的访问控制将完全在 Adobe Admin Console（AAC）中进行管理。为确保访问安全，您需要在 AAC 中配置 IP 限制。更多信息请参阅这篇 [Marketing Nation 博客帖子](https://nation.marketo.com/t5/product-blogs/updated-important-update-ip-restrictions-feature-transition/ba-p/358420){target="_blank"}。

**如果在 Adobe Identity 迁移后，我有一些用户的角色启用了“绕过单点登录”选项，会发生什么？**

Adobe Admin Console 默认包含一个 Business ID 目录。在 Adobe 组织中，凡是不在 Federated ID 目录已声明域名范围内的用户，都会分配到此目录，并使用 Adobe ID 身份类型。这些用户无需通过单点登录（SSO）即可访问 Marketo Engage，并且许可证的所有权仍归公司所有，而非个人。

**我有多个订阅，但并非全部启用单点登录。完成 Adobe Identity 迁移后会怎样？**

当订阅加入 Adobe Identity 后，单点登录（SSO）会在 Adobe 组织级别进行设置。这意味着，SSO 会应用于 Adobe 组织中的所有产品实例。配置 SSO 后，它会对该 Adobe 组织内的所有 Marketo 实例生效。此前，Marketo 支持在实例级别配置此设置。但 Adobe Identity Management System 不支持这种实例级别的配置方式。

**完成 Adobe Identity 迁移后，我们目前用于 Marketo Engage 的 CNAME、SPF 或 DKIM 是否需要做任何更改？**

不需要，这些配置不会受到影响。

**如何防止会话超时？**

在[高级设置](https://helpx.adobe.com/cn/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}中，您可以自定义所需的最大会话时长（需要系统管理员权限）。建议在产品迁移完成后、用户迁移开始前配置此设置。

**我现在必须先进入 Experience Cloud 才能访问 Marketo Engage。有没有办法简化这个流程？**

可以。您可以将点击 Marketo Engage 实例入口页面上的&#x200B;**启动**&#x200B;按钮后打开的链接保存为浏览器书签，今后即可直接通过该书签访问，从而跳过该入口页面。

![](assets/faq-1.png)

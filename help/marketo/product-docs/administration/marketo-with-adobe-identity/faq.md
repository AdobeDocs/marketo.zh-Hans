---
description: AdobeIdentity Management常见问题解答 — Marketo文档 — 产品文档
title: AdobeIdentity Management常见问题解答
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 094a11f9544e0dba75167de229d78e8ff50cf6e8
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 1%

---

# AdobeIdentity Management常见问题解答 {#adobe-identity-management-faq}

**什么是Adobe标识？**

AdobeIdentity Management System包含三个组件。

* [!DNL Adobe Identity Service]：处理最终用户的身份验证和验证，包括联合和运行时单点登录(SSO)。

* Adobe Admin Console：Admin Console提供了一个中央位置，用于管理整个组织的Adobe权限。 它处理用户管理、云服务、桌面许可证授权、联合身份验证配置，并提供数据丢失防护安全功能。

* Adobe用户管理API (UMAPI)：允许组织在Adobe Admin Console中通过API级别管理企业用户和权限。

**现有的Marketo Engage订阅何时将与IMS集成？**

现有的Marketo订阅将在今年晚些时候迁移到AdobeIdentity Management System。 Marketo支持部门将无法提供有关Adobe IMS迁移的任何更新。 Adobe客户团队将在未来几个月内完成估计的时间表。

**Adobe产品管理员和Marketo Engage管理员之间有何区别？**

* Adobe产品管理员是Marketo平台中的新角色。
* Adobe产品管理员角色已授予在Adobe Admin Console中添加为产品管理员的用户
* Adobe产品管理员是只读角色，无法编辑或从Marketo Engage中删除。
* Adobe产品管理员具有与标准Marketo管理员相同的权限。
* Marketo Engage管理员的角色仍然是管理员，并且已授予具有Marketo Engage的用户。

**用户管理API客户端支持是否有任何变化？**

是的。 已载入Adobe IMS的用户无法使用所有现有的Marketo用户管理API。 对于用户邀请、更新和删除操作，Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} 应该使用。 对于角色管理，Marketo用户管理API仍然适用。 除此之外，对Marketo REST API客户端支持没有其他更改。

**如果我们与IMS集成，我们会联系谁获取支持？**

您应遵循标准步骤联系 [Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

**如果我使用Adobe身份访问其他Adobe应用程序，能否使用该身份访问Marketo？**

即使您有其他Adobe产品，在将订阅迁移到IMS之前，您无法使用Adobe身份访问Marketo。

**Marketo用户角色（位于工作区中）是否在Adobe Admin Console中进行管理？**

否. 用户Marketo Engage管理（在工作区中）已完成。

**我是IMS集成订阅中的Marketo管理员，无权访问Admin Console。 如何获取访问权限？**

任何有权访问贵组织Admin Console的Adobe系统或产品管理员都可以为您提供访问权限。 如果您不确定贵组织中的哪些人具有控制台中的管理员权限，请联系 [Adobe客户关怀](https://helpx.adobe.com/contact.html){target="_blank"}.

**管理员如何将用户添加到Marketo [!DNL Sales Connect]？**

虽然Admin Console中会有一个产品卡 [!DNL Sales Connect]，Admin Console不应用于添加/管理用户。 以下链接将允许管理员通过Marketo管理用户 [!DNL Sales Connect]： [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**在哪里可以了解有关Adobe Admin Console的更多信息？**

[https://helpx.adobe.com/cn/enterprise/admin-guide.html](https://helpx.adobe.com/cn/enterprise/admin-guide.html){target="_blank"}.

**我是否仍要转到Marketo中的“管理员”部分，以便对我的帐户进行用户帐户更改？**

否，您需要导航到 [account.adobe.com](https://account.adobe.com){target="_blank"}.

**如何将其与Marketo的通用ID结合使用？**

已载入Adobe身份的用户可以通过产品中的订阅切换器无缝访问所有支持IMS的订阅。

**这是否适用于SSO？**

是的。 Marketo与Adobe IMS的集成支持通用ID用户和SSO。 SSO现在由Adobe IMS驱动，在Adobe Admin Console的组织级别设置。 [在此处了解详情](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**设备授权的工作原理是什么？**

Adobe IMS当前不支持Marketo的设备授权功能等任何功能。

**是否仍可以使用“在邀请用户对话框中登录”功能，使用户的登录在其电子邮件中是唯一的？**

否. 订阅启用了IMS时，用户邀请工作流不再有效，因此功能不再有效。 Adobe身份要求用户的身份由其电子邮件驱动。

**对于Adobe IMS，我们是否可以选择使用Adobe ID、Enterprise ID或Federated ID？**

是，您可以确定组织支持的身份类型。 更多信息可在此处找到： [身份概述](https://helpx.adobe.com/enterprise/using/identity.html) 此处为： [设置标识](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Adobe Admin Console支持哪些产品卡？**

支持的产品卡包括：Marketo Engage、Marketo Measure、MarketoDynamic Chat、Marketo Sales Connect和Marketo Sales Insight Actions。

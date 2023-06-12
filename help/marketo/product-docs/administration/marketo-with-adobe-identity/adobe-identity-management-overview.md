---
description: AdobeIdentity Management概述 — Marketo文档 — 产品文档
title: AdobeIdentity Management概述
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 0%

---

# AdobeIdentity Management概述 {#adobe-identity-management-overview}

如果您从2022年2月15日起拥有具有Adobe Marketo Engage的新帐户（新帐户，而不仅仅是现有帐户的新实例），则它可能会与AdobeIdentity Management System集成，具体取决于购买的产品包。 要了解您是否拥有该产品，请联系Adobe客户团队（您的客户经理）。

现有Marketo订阅将于2023年下半年开始迁移到AdobeIdentity Management System。

>[!NOTE]
>
>Marketo支持将无法提供有关Adobe IMS迁移的任何更新。 Adobe客户团队将在未来几个月内完成预计的时间表。

## 配置文件级别 {#profile-levels}

载入到AdobeIdentity Management System的Adobe Marketo Engage订阅支持各种配置文件。 以下是与此集成相关的用户配置文件类型。

<table>
 <tr>
  <td><strong>Adobe Admin Console系统管理员</strong></td>
  <td>负责在Adobe Admin Console中为Adobe组织和Marketo Engage产品设置标识概念。 在Adobe组织设置时授予的角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console产品管理员</strong></td>
  <td>负责在Adobe Admin Console中授予用户使用Marketo Engage产品的权限。 在Adobe Admin Console中授予的角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console产品配置文件管理员</strong></td>
  <td>负责管理产品配置文件中的用户。 他们不能在该特定配置文件之外管理用户。 除非以用户身份添加到产品配置文件，否则产品配置文件管理员无权访问Marketo应用程序。 他们的角色仍将是标准用户（如果有多个工作区，则为默认工作区）。
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage产品管理员</strong></td>
  <td>具有管理权限的Marketo Engage访问权限的用户。 在Marketo Engage中授予的角色，而不是Adobe Admin Console。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage用户</strong></td>
  <td>有权访问Marketo Engage的人员。 无管理权限。</td>
 </tr>
</table>

## 常见问题解答 {#faq}

**什么是Adobe身份？**

AdobeIdentity Management System包含三个组件。

* [!DNL Adobe Identity Service]：处理最终用户的身份验证和验证，包括联合身份验证和运行时单点登录(SSO)。

* Adobe Admin Console：Admin Console提供了一个中央位置，用于管理整个组织的Adobe授权。 它处理用户管理、云服务、桌面许可证授权、联合身份验证配置，并提供数据丢失防护安全功能。

* Adobe用户管理API (UMAPI)：允许组织在Adobe Admin Console中通过API级别管理企业用户和权限。

**现有的Marketo Engage订阅何时将与IMS集成？**

现有的Marketo订阅将在今年晚些时候迁移到AdobeIdentity Management System。 Marketo支持将无法提供有关Adobe IMS迁移的任何更新。 Adobe客户团队将在未来几个月内完成预计的时间表。

**Adobe产品管理员和Marketo Engage管理员之间有何区别？**

* Adobe产品管理员是Marketo平台中的新角色。
* Adobe产品管理员角色已授予在Adobe Admin Console中添加为产品管理员的用户
* Adobe产品管理员是只读角色，无法编辑或从Marketo Engage中删除。
* Adobe产品管理员具有与标准Marketo管理员相同的权限。
* Marketo Engage管理员的角色仍然是管理员，并按Marketo Engage授予用户。

**用户管理API客户端支持是否有任何变化？**

是. 已载入Adobe IMS的用户无法使用所有现有的Marketo用户管理API。 对于用户邀请、更新和删除操作，Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} 应该使用。 对于角色管理，Marketo用户管理API仍然适用。 除此之外，对Marketo REST API客户端支持没有其他更改。

**如果我们与IMS集成，我们会联系谁获取支持？**

您应遵循标准流程联系 [Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

**如果我使用Adobe身份访问其他Adobe应用程序，能否使用该身份访问Marketo？**

即使您有其他Adobe产品，也不能使用Adobe身份访问Marketo，直到将订阅迁移到IMS。

**Marketo用户角色（在工作区中）是否在Adobe Admin Console中进行管理？**

否. 用户角色管理（在工作区中）在Marketo Engage中完成。

**我是IMS集成订阅的Marketo管理员，无权访问该Admin Console。 如何获取访问权限？**

任何有权访问贵组织Admin Console的Adobe系统或产品管理员都可以为您授予访问权限。 如果您不确定贵组织中的谁具有控制台中的管理员权限，请联系 [Adobe客户关怀](https://helpx.adobe.com/contact.html){target="_blank"}.

**管理员如何将用户添加到Marketo [!DNL Sales Connect]？**

虽然Admin Console中会有一个产品卡 [!DNL Sales Connect]，Admin Console不应用于添加/管理用户。 以下链接将允许管理员通过Marketo管理用户 [!DNL Sales Connect]： [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**在哪里可以了解有关Adobe Admin Console的更多信息？**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html){target="_blank"}.

**我是否仍要转到Marketo中的“管理员”部分，以便对我的帐户进行用户帐户更改？**

否，您需要导航到 [account.adobe.com](https://account.adobe.com){target="_blank"}.

**此令牌如何与Marketo的通用ID一起使用？**

已载入Adobe身份的用户可以通过产品中的订阅切换器无缝访问所有启用了IMS的订阅。

**这是否适用于SSO？**

是. Marketo与Adobe IMS的集成支持通用ID用户和SSO。 SSO现在由Adobe IMS驱动，在Adobe Admin Console中的组织级别设置。 [在此处了解详情](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**设备授权如何工作？**

Adobe IMS当前不支持Marketo的设备授权功能等任何功能。

**是否仍可以使用“在邀请用户对话框中登录”功能，使用户的登录在其电子邮件中是唯一的？**

否. 订阅启用了IMS时，用户邀请工作流不再处于活动状态，因此该功能不再有效。 Adobe身份要求用户的身份由其电子邮件驱动。

**对于Adobe IMS，我们是否可以选择使用Adobe ID、Enterprise ID或Federated ID？**

是，由您确定组织支持的身份类型。 更多信息可在此处找到： [身份概述](https://helpx.adobe.com/enterprise/using/identity.html) 以及此处： [设置身份](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Adobe Admin Console支持哪些产品卡？**

支持的产品卡包括：Marketo Engage、Marketo Measure、MarketoDynamic Chat、Marketo Sales Connect和Marketo Sales Insight Actions。

>[!MORELIKETHIS]
>
>* [管理员设置](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [添加或删除产品管理员](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [添加或删除用户](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}

---
description: AdobeIdentity Management概述 — Marketo文档 — 产品文档
title: AdobeIdentity Management概述
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# AdobeIdentity Management概述 {#adobe-identity-management-overview}

如果您从2022年2月15日起拥有使用Adobe Marketo Engage的新帐户（新帐户，而不仅仅是现有帐户的新实例），则它可能会与AdobeIdentity Management System集成，具体取决于购买的产品包。 要了解您是否拥有该产品，请联系Adobe客户团队（您的客户经理）。

现有Marketo订阅将在2023年下半年开始迁移到AdobeIdentity Management System。

如果您拥有 [新帐户](/help/marketo/product-docs/administration/marketo-with-adobe-identity/quick-guide.md){target="_blank"} Adobe Marketo Engage （不仅是现有帐户的新实例）自2022年2月15日起，它可能会与AdobeIdentity Management System (IMS)集成，具体取决于购买的产品包。 要了解您是否拥有该产品，请联系Adobe客户团队（您的客户经理）。

现有Marketo订阅将在2023年末开始迁移到AdobeIdentity Management System。 最初，这些迁移只能在您重新签订Marketo订阅合同后进行。 Adobe计划大约在2024年年中开始在Marketo重新签约活动之外迁移用户。

>[!NOTE]
>
>Marketo支持部门无法提供任何有关Adobe IMS迁移的更新。 Adobe客户团队将在未来几个月内完成估计的时间表。 有关详细信息，请参阅 [本文](/help/marketo/product-docs/administration/marketo-with-adobe-identity/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"}, and the [Frequently Asked Questions](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## 配置文件级别 {#profile-levels}

载入到Identity Management SystemAdobe的Adobe Marketo Engage订阅支持各种配置文件。 以下是与此集成相关的用户配置文件类型。

<table>
 <tr>
  <td><strong>Adobe Admin Console系统管理员</strong></td>
  <td>负责在Adobe Admin Console中为Adobe组织和Marketo Engage产品设置标识概念。 在Adobe组织设置中授予的角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console产品管理员</strong></td>
  <td>负责在Adobe Admin Console中授予用户使用Marketo Engage产品的权限。 已在Adobe Admin Console中授予角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console产品配置文件管理员</strong></td>
  <td>负责管理产品配置文件中的用户。 他们无法在该特定配置文件之外管理用户。 产品配置文件管理员无权访问Marketo应用程序，除非以用户身份添加到产品配置文件。 他们的角色仍将是标准用户（如果有多个工作区，则为默认工作区）。
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage产品管理员</strong></td>
  <td>被授予具有管理权限的Marketo Engage访问权限的用户。 在Marketo Engage中授予的角色，而不是Adobe Admin Console。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage用户</strong></td>
  <td>被授予Marketo Engage访问权限的用户。 无管理权限。</td>
 </tr>
</table>

## 常见问题 {#faq}

常见问题解答 [可在此处找到](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [管理员设置](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [添加或删除产品管理员](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [添加或删除用户](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}

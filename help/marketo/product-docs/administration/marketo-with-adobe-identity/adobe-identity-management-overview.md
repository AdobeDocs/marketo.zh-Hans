---
description: AdobeIdentity Management概述 — Marketo文档 — 产品文档
title: AdobeIdentity Management概述
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 094a11f9544e0dba75167de229d78e8ff50cf6e8
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# AdobeIdentity Management概述 {#adobe-identity-management-overview}

所有新的Adobe Marketo Engage订阅（2023年7月31日或更高版本）都与AdobeIdentity Management System集成。 现有Marketo订阅目前正在续订和/或重新签约活动时迁移到AdobeIdentity Management System。 目前不支持在续订或重新承包事件之外进行迁移。

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

---
description: 概述 — Marketo文档 — 产品文档
title: 概述
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: 88622c5df7cf04fb9e4a3bcccbf77db5594b5fc4
workflow-type: tm+mt
source-wordcount: '1056'
ht-degree: 0%

---

# 概述 {#overview}

如果您自2022年2月15日起在Adobe Marketo Engage拥有新帐户（新帐户，而不只是现有帐户的新实例），则它可能会与AdobeIdentity Management系统集成，具体取决于购买的产品包。 要确定是否具有该功能，请联系您的Marketo管理员或您帐户的客户成功经理。

现有Marketo订阅将从今年晚些时候开始迁移到AdobeIdentity Management系统。

>[!NOTE]
>
>Marketo支持将无法提供有关Adobe IMS迁移的任何更新。 您的客户成功经理将在未来几个月内提供预计的时间表。

## 配置文件级别 {#profile-levels}

载入AdobeIdentity Management系统的AdobeMarketo Engage订阅支持各种配置文件。 以下是与此集成相关的用户配置文件类型。

<table>
 <tr>
  <td><strong>Adobe Admin Console系统管理员</strong></td>
  <td>负责在Adobe Admin Console中为Adobe组织和Marketo Engage产品设置身份概念。 已在Adobe组织设置中授予角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console产品管理员</strong></td>
  <td>负责在Adobe Admin Console中为Marketo Engage产品授予用户权限。 授予了在Adobe Admin Console的角色。</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console产品配置文件管理员</strong></td>
  <td>负责管理产品配置文件中的用户。 他们无法管理该特定配置文件之外的用户。 产品配置文件管理员无权访问Marketo应用程序，除非以用户身份添加到产品配置文件中。 其角色仍将是标准用户（如果有多个工作区，则为默认工作区）。
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage产品管理员</strong></td>
  <td>已获得具有管理权限的Marketo Engage访问权限的人员。 已在Marketo Engage中授予角色，而不是Adobe Admin Console。</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage用户</strong></td>
  <td>获得访问Marketo Engage的人员。 无管理权限。</td>
 </tr>
</table>

## 常见问题解答 {#faq}

**什么是Adobe标识？**

AdobeIdentity Management系统由三个组件组成。

* Adobe标识服务：处理最终用户的验证和验证，包括联合和运行时单点登录(SSO)。

* Adobe Admin Console:Admin Console提供了一个中心位置，用于管理整个组织中的Adobe权限。 它可处理用户管理、云服务、桌面许可证授权、联合配置，并提供数据丢失预防安全功能。

* Adobe用户管理API(UMAPI):允许组织在API级别管理Adobe Admin Console中的企业用户和权限。

**现有Marketo Engage订阅何时将与IMS集成？**

今年晚些时候，现有的Marketo订阅将迁移到AdobeIdentity Management系统。 Marketo支持将无法提供有关Adobe IMS迁移的任何更新。 您的客户成功经理将在未来几个月内提供预计的时间表。

**Adobe产品管理员和Marketo Engage管理员之间有何区别？**

* Adobe产品管理员是Marketo平台中的新角色。
* Adobe产品管理员角色授予在Adobe Admin Console中添加为产品管理员的用户
* Adobe产品管理员是只读角色，无法从Marketo Engage中编辑或删除。
* Adobe产品管理员具有与标准Marketo管理员相同的权限。
* Marketo Engage管理员的角色仍为管理员，并会授予Marketo Engage中的用户。

**用户管理API客户端支持是否有任何变化？**

是的。 已载入Adobe IMS的用户无法利用所有现有的Marketo用户管理API。 对于用户邀请、更新和删除操作，Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html) 值。 对于角色管理，Marketo用户管理API仍然适用。 除此之外，对Marketo REST API客户端支持没有其他更改。

**如果我们已与IMS集成，那么我们应该联系谁以获取支持？**

您应按照标准程序联系 [Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support).

**如果我使用Adobe标识访问其他Adobe应用程序，是否可以使用该标识访问Marketo?**

即使您有其他Adobe产品，在将订阅迁移到IMS之前，您仍无法使用Adobe标识访问Marketo。

**Marketo用户角色（在工作区内）是否在Adobe Admin Console中进行管理？**

不。 用户角色管理（在工作区内）在Marketo Engage中完成。

**我是IMS集成订阅的Marketo管理员，无权访问Admin Console。 如何获取访问权限？**

任何有权访问贵组织Adobe的Admin Console的系统或产品管理员都可以为您提供访问权限。 如果您不确定您组织中的谁在控制台中具有管理员权限，请联系 [Adobe客户关怀](https://helpx.adobe.com/contact.html).

**管理员如何将用户添加到Marketo Sales Connect?**

虽然Sales Connect的Admin Console中将有产品卡，但不应使用Admin Console来添加/管理用户。 以下链接将允许管理员通过Marketo Sales Connect管理用户： [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**我在哪里可以了解有关Adobe Admin Console的更多信息？**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**我是否仍然转到Marketo的“管理员”部分，以更改我的帐户？**

否，您需要导航到 [account.adobe.com](https://account.adobe.com).

**这如何与Marketo的通用ID一起使用？**

那些已载入到Adobe身份的用户可以通过产品中的订阅切换器，无缝访问所有支持IMS的订阅。

**这是否适用于SSO?**

是的。 Marketo与Adobe IMS集成支持通用ID用户和单点登录。 SSO现在由Adobe IMS驱动，在Adobe Admin Console的组织级别设置。 [在此处了解更多](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**设备授权的工作原理是什么？**

Adobe IMS当前不支持任何类似Marketo设备授权功能的内容。

**是否仍可以使用“在邀请用户对话框中登录”功能，使用户的登录在其电子邮件中具有唯一性？**

不。 启用了IMS订阅后，“用户邀请”工作流不再处于活动状态，因此该功能不再有效。 Adobe身份要求用户的身份由其电子邮件驱动。

**对于Adobe IMS，我们是否可以选择使用Adobe ID、Enterprise ID或Federated ID?**

是，您可以确定要获得组织支持的身份类型。 更多信息可在此处找到： [身份概述](https://helpx.adobe.com/enterprise/using/identity.html) 和此处： [设置标识](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

>[!MORELIKETHIS]
>
>* [管理员设置](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [添加或删除产品管理员](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [添加或删除用户](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)


---
description: 概述 — Marketo文档 — 产品文档
title: 概述
hide: true
hidefromtoc: true
source-git-commit: 306e08b08bf63fe51778dc51ccb9cb971fed2f4b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 概述 {#overview}

如果您的AdobeMarketo Engage订阅是在10/4/21或之后配置的，它将与AdobeIdentity Management系统集成。 AIMS允许用户使用通用的Marketo Engage身份登录到Experience Cloud和其他Adobe应用程序。

## 配置文件级别

有三个用户档案级别。

<table>
 <tr>
  <td><strong>系统管理员</strong></td>
  <td>负责在Adobe Admin Console中为Adobe组织和Marketo Engage产品设置身份概念。</td>
 </tr>
 <tr>
  <td><strong>产品管理员</strong></td>
  <td>负责在Adobe Admin Console中为Marketo Engage产品授予用户权限。</td>
 </tr>
 <tr>
  <td><strong>用户</strong></td>
  <td>获得访问Marketo Engage的人员。 无管理权限。</td>
 </tr>
</table>

## 常见问题解答

**什么是Adobe标识？**

AdobeIdentity Management系统由三个组件组成。

* Adobe标识服务：处理最终用户的验证和验证，包括联合和运行时单点登录(SSO)。

* Adobe Admin Console:Admin Console提供了一个中心位置，用于管理整个组织中的Adobe权限。 它可处理用户管理、云服务、桌面许可证授权、联合配置，并提供数据丢失预防安全功能。

* Adobe用户管理API(UMAPI):允许组织在API级别管理Adobe Admin Console中的企业用户和权限。

**Adobe产品管理员和Marketo Engage管理员之间有何区别？**

* Adobe产品管理员是Marketo平台中的新角色。
* 它是只读角色，无法从Marketo中编辑或删除。
* 它拥有与标准Marketo管理员相同的权限和权限。

**API客户端支持有任何变化吗？**

是的。 已载入Adobe IMS的用户无法利用现有的Marketo用户管理API。 它们将使用[IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html)。

**我们联系谁以寻求支持？**

您应按照联系[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support)的标准步骤操作。

**Marketo用户角色（在工作区内）是否在Adobe Admin Console中进行管理？**

不。 用户角色管理（在工作区内）在Marketo中已完成。

**我是Marketo管理员，无权访问Admin Console。如何获取访问权限？**

任何有权访问贵组织Admin Console的系统或产品管理员都可以授予您访问权限。 如果您不确定您组织中的谁在控制台中具有管理员权限，请联系[Adobe客户关怀](https://helpx.adobe.com/contact.html)。

**管理员如何将用户添加到Marketo Sales Connect?**

虽然AC中将有一张产品卡用于Sales Connect，但不应使用AC来添加/管理用户。 以下链接将允许管理员通过Marketo Sales Connect管理用户：[https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management)。

**我在哪里可以了解有关Adobe Admin Console的更多信息？**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html)。

**我是否仍然转到Marketo中的“管理员”部分进行帐户更改？**

不需要，您需要导航到[account.adobe.com](https://account.adobe.com)。

**这如何与Marketo的通用ID一起使用？**

那些已载入到Adobe身份的用户可以通过产品中的订阅切换器，无缝访问所有支持IMS的订阅。

**这是否适用于SSO?**

是的。 Marketo与Adobe IMS集成支持通用ID用户和单点登录。 SSO现在由Adobe IMS驱动，在Adobe Admin Console的组织级别设置。 [在此处了解更多信息](https://helpx.adobe.com/enterprise/using/set-up-identity.html)。

**设备授权的工作原理是什么？**

Adobe IMS当前不支持任何类似Marketo设备授权功能的内容。

**是否仍可以使用“在邀请用户对话框中登录”功能，使登录从我们的电子邮件中变得唯一？**

不。 启用了IMS订阅后，“用户邀请”工作流不再处于活动状态，因此该功能不再有效。 Adobe身份要求用户的身份由其电子邮件驱动。

**对于Adobe IMS，我们是否可以选择使用Adobe ID、Enterprise ID或Federated ID?**

是，您可以确定要获得组织支持的身份类型。 有关更多信息，请参见[此处](https://helpx.adobe.com/enterprise/using/identity.html)和[此处](https://helpx.adobe.com/enterprise/using/set-up-identity.html)。

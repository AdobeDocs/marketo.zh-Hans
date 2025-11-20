---
description: Adobe Identity Management常见问题解答 — Marketo文档 — 产品文档
title: Adobe Identity Management常见问题解答
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 95ed91736b7276dd7a5b9e09958c1f09832ae719
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 1%

---

# Adobe Identity Management常见问题解答 {#adobe-identity-management-faq}

**什么是Adobe标识？**

Adobe Identity Management System包含三个组件。

* [!DNL Adobe Identity Service]：处理最终用户的身份验证和验证，包括联合身份验证和运行时单点登录(SSO)。

* Adobe Admin Console： Admin Console提供了一个中央位置，用于管理整个组织的Adobe权限。 它处理用户管理、云服务、桌面许可证授权、联合身份验证配置，并提供数据丢失防护安全功能。

* Adobe用户管理API (UMAPI)：允许组织在Adobe Admin Console中通过API级别管理企业用户和权限。

**现有的Marketo Engage订阅何时将与IMS集成？**

现有Marketo Engage订阅目前正在根据任何销售活动迁移到Adobe IMS，包括续订、重新签约活动和/或附录。 从2024年10月起，支持在销售活动之外进行迁移。

**迁移后，Marketo Engage URL是否将保持不变？**

不是。迁移后，URL将以下列格式显示： `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (XXX表示Munchkin ID，@tenantID来自您的Adobe组织)。

**需要执行任何操作以准备进行URL更改吗？**

可以。迁移后，Marketo Engage将从experience.adobe.com提供到Adobe Experience Cloud。 您需要与IT团队合作，允许列表本文顶部[列出的所有Adobe域](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"}，以防止对Marketo Engage访问的中断。

指向engage-xx.marketo.com域&#x200B;_上Marketo Engage资源的先前链接和书签将_&#x200B;继续正常运行。 但是，您必须首先登录到要导航到的URL的Marketo Engage实例。 例如，要导航到Munchkin ID为123-ABC-456的实例中Smart Campaign的书签，您需要首先使用Munchkin ID 123-ABC-456登录Marketo Engage实例。

虽然没有进行规划，但未来的开发工作可能会破坏此重定向功能。 为避免意外中断，建议尽早更新书签。

**此项是否适用于SSO？**

可以。与Adobe IMS的集成支持通用ID用户和SSO。 SSO现在由Adobe IMS驱动，在Adobe Admin Console的组织级别设置。 但是，与Marketo Engage SP启动的支持相比，Adobe IdP启动的支持存在差异（[在此了解更多](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}）。 如果您在迁移到Admin Console后需要有关SSO差异的帮助，请联系[Adobe客户关怀](https://helpx.adobe.com/contact.html){target="_blank"}。

**Adobe产品管理员与Marketo Engage管理员有何区别？**

* Adobe产品管理员是Marketo平台中的新角色。
* Adobe产品管理员角色已授予在Adobe Admin Console中添加为产品管理员的用户
* Adobe产品管理员是只读角色，无法从Marketo Engage中进行编辑或删除。
* Adobe产品管理员具有与标准Marketo管理员相同的权限和权限。
* Marketo Engage管理员的角色仍然是管理员，并且已授予Marketo Engage中的用户。
* 只有具有Marketo默认管理员角色的用户才能在Admin Console中分配为Marketo产品管理员。

**用户管理API客户端支持是否有任何更改？**

可以。已载入Adobe IMS的用户无法使用所有现有的Marketo用户管理API。 对于用户邀请、更新和删除操作，应使用Adobe [IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"}。 对于角色管理，Marketo用户管理API仍然适用。 除此之外，对Marketo REST API客户端支持没有其他更改。

**如果我们与IMS集成，我们应当联系谁获取支持？**

* 预用户迁移： [营销国家社区](https://nation.marketo.com/t5/support/ct-p/Support)或电子邮件`customercare@marketo.com`中的文件支持案例。

* 用户迁移后： [营销国家社区](https://nation.marketo.com/t5/support/ct-p/Support)或电子邮件`customercare@marketo.com`中的文件支持案例。

* 支持后迁移完成：产品支持管理员可以通过Experience League支持门户提交案例。

如果您拥有Ultimate Success，则可以访问Admin Console迁移白手套服务。 请联系Adobe客户团队（您的客户经理）寻求帮助。

**如果我使用Adobe身份访问其他Adobe应用程序，能否使用该身份访问Marketo？**

即使您拥有其他Adobe产品，在将订阅迁移到IMS之前，您无法使用Adobe Identity访问Marketo。

**Marketo用户角色（位于工作区中）是否在Adobe Admin Console中进行管理？**

不是。用户角色管理（在工作区中）在Marketo Engage中完成。

**我是IMS集成订阅中的Marketo管理员，无权访问Admin Console。 如何获取访问权限？**

任何有权访问贵组织Admin Console的Adobe系统或产品管理员都可以为您提供访问权限。 如果您不确定贵组织中的哪些人具有控制台中的管理员权限，请联系[Adobe客户关怀团队](https://helpx.adobe.com/contact.html){target="_blank"}。

**管理员如何将用户添加到Marketo [!DNL Sales Connect]？**

虽然Admin Console中会有[!DNL Sales Connect]的产品卡，但不应使用Admin Console添加/管理用户。 以下链接将允许管理员通过Marketo [!DNL Sales Connect]管理用户： [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}。

**在哪里可以了解有关Adobe Admin Console的更多信息？**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/cn/enterprise/admin-guide.html){target="_blank"}。

**我是否仍要转到Marketo中的“管理员”部分以更改我的帐户？**

否，您需要导航到[account.adobe.com](https://account.adobe.com){target="_blank"}。

**这如何与Marketo的通用ID一起使用？**

已载入Adobe身份的用户可以通过产品中的订阅切换器无缝访问所有启用了IMS的订阅。

**此项是否适用于SSO？**

可以。Marketo与Adobe IMS的集成支持通用ID用户和SSO。 SSO现在由Adobe IMS驱动，在Adobe Admin Console的组织级别设置。 [在此了解详情](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

**我已登记使用Adobe Identity，现在我要实施SSO。 我该怎么办？**

如果要实施单点登录，并且您的订阅已登记到Adobe Identity，而没有Adobe组织中实施的SSO，请向[Marketo支持](https://nation.marketo.com/){target="_blank"}提交票证，并将主题指定为“Admin Console上的Marketo，实施SSO”。

**设备授权的工作原理是什么？**

Adobe IMS当前不支持Marketo的设备授权功能等任何功能。

**仍然可以使用“在邀请用户对话框中登录”功能来使用户的登录在其电子邮件中是唯一的？**

不是。订阅启用了IMS时，用户邀请工作流不再有效，因此功能不再有效。 Adobe身份要求用户的身份由其电子邮件驱动。

**对于Adobe IMS，我们是否可以选择使用Adobe ID、Enterprise ID或Federated ID？**

是，您可以确定组织支持的身份类型。 可在以下位置找到更多信息： [身份概述](https://helpx.adobe.com/cn/enterprise/using/identity.html)和此处： [设置身份](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

**Adobe Admin Console支持哪些产品卡？**

支持的产品卡包括：Marketo Engage、Marketo Measure、Marketo Dynamic Chat、Marketo Sales Connect和Marketo Sales Insight Actions。

**如果我迁移到Adobe身份后，我的用户登录名与电子邮件不匹配，该怎么办？**

登录名不同于其电子邮件地址的当前Marketo Engage用户，在迁移到Adobe身份后，将不再使用该凭据登录。 Adobe身份始终使用用户的电子邮件地址进行身份验证。 您可以在[account.adobe.com](https://account.adobe.com){target="_blank"}上更新Adobe身份电子邮件地址。

**如果我的订阅使用IP限制设置，则在迁移Adobe身份后会发生什么情况？**

您当前的IP限制将在2026年第1季度保持有效（这适用于在迁移前启用这些限制的订阅）。 这些限制也适用于Adobe ID用户，因此您的访问控制将继续按预期工作。

从2026年第1季度开始，将取消旧版IP限制。 从那时起，基于IP的访问将在Adobe Admin Console (AAC)中专门进行管理。 要维护安全访问，您需要在AAC中配置IP限制。 有关详细信息，请参阅此[营销国家博客文章](https://nation.marketo.com/t5/product-blogs/updated-important-update-ip-restrictions-feature-transition/ba-p/358420){target="_blank"}。

**如果我的用户具有“绕过单点登录”的选项，则在迁移Adobe Identity后会发生什么情况？**

Adobe Admin Console附带默认的Business ID目录。 在Adobe组织的Federated ID目录中声明的域以外的用户将分配到具有Adobe ID标识类型的此目录。 这些用户无需通过单点登录(SSO)即可访问Marketo Engage，并且许可证所有权将保留在公司而非个人手中。

**我有多个订阅，但并非所有订阅都启用了单点登录。 Adobe标识迁移后会发生什么情况？**

将订阅登记到Adobe Identity后，将在Adobe组织级别设置单点登录(SSO)。 这意味着SSO适用于Adobe组织中的所有产品实例。设置SSO后，它将应用于该Adobe组织中的所有Marketo实例。以前，Marketo在实例级别支持此设置。 Adobe Identity Management System不支持此功能。

**在Adobe Identity迁移之后，我们当前用于Marketo Engage的CNAME、SPF或DKIM是否需要任何更改？**

不，这些配置不会受到影响。

**如何防止会话超时？**

在[高级设置](https://helpx.adobe.com/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}中，您可以自定义所需的最长会话寿命（需要系统管理员权限）。 建议在产品迁移之后、用户迁移之前建立此设置。

**我现在必须导航到Experience Cloud才能访问Marketo Engage。 是否有办法简化此流程？**

可以。您可以为单击Marketo Engage实例入口页面上的&#x200B;**启动**&#x200B;按钮后启动的链接创建浏览器书签，以绕过该页面。

![](assets/faq-1.png)

---
description: AdobeIdentity Management常见问题解答 — Marketo文档 — 产品文档
title: AdobeIdentity Management常见问题解答
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 7a5440b3673c3ebbb181ee5e81ee202463291fe7
workflow-type: tm+mt
source-wordcount: '1456'
ht-degree: 0%

---

# AdobeIdentity Management常见问题解答 {#adobe-identity-management-faq}

**什么是Adobe标识？**

AdobeIdentity Management System包含三个组件。

* [!DNL Adobe Identity Service]：处理最终用户的身份验证和验证，包括联合身份验证和运行时单点登录(SSO)。

* Adobe Admin Console：Admin Console提供了一个中央位置，用于管理整个组织的Adobe权限。 它处理用户管理、云服务、桌面许可证授权、联合身份验证配置，并提供数据丢失防护安全功能。

* Adobe用户管理API (UMAPI)：允许组织在Adobe Admin Console中通过API级别管理企业用户和权限。

**现有Marketo Engage订阅何时将与IMS集成？**

现有Marketo Engage订阅目前正在根据任何销售活动迁移到Adobe IMS，包括续订、重新签约活动和/或附录。 从2024年10月起，支持销售活动以外的迁移。

**迁移后，Marketo EngageURL是否将保持不变？**

不会。迁移后URL的外观将有所不同。

**需要执行任何操作以准备进行URL更改吗？**

可以。迁移后，Marketo Engage将从experience.adobe.com提供给Adobe Experience Cloud。 您需要与IT团队合作，允许列表本文顶部[列出的所有Adobe域](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"}，以防止对Marketo Engage访问的中断。

以前在engage-xx.marketo.com域&#x200B;_上Marketo Engage资源的链接和书签将继续正常运行。_&#x200B;但是，您必须首先登录到要导航到的URL的Marketo Engage实例。 例如，要导航到Munchkin ID为123-ABC-456的实例中Smart Campaign的书签，您需要先登录Munchkin ID为123-ABC-456的Marketo Engage实例。

**Adobe产品管理员和Marketo Engage管理员之间有何区别？**

* Adobe产品管理员是Marketo平台中的新角色。
* Adobe产品管理员角色已授予在Adobe Admin Console中添加为产品管理员的用户
* Adobe产品管理员是只读角色，无法编辑或从Marketo Engage中删除。
* Adobe产品管理员具有与标准Marketo管理员相同的权限。
* Marketo Engage管理员的角色仍然是管理员，并且已授予具有Marketo Engage的用户。

**用户管理API客户端支持是否有任何更改？**

可以。已载入Adobe IMS的用户无法使用所有现有的Marketo用户管理API。 对于用户邀请、更新和删除操作，应使用Adobe[IMS API](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"}。 对于角色管理，Marketo用户管理API仍然适用。 除此之外，对Marketo REST API客户端支持没有其他更改。

**如果我们与IMS集成，我们应当联系谁获取支持？**

* 预用户迁移： [营销国家社区](https://nation.marketo.com/t5/support/ct-p/Support)或电子邮件`customercare@marketo.com`中的文件支持案例。

* 用户迁移后： [营销国家社区](https://nation.marketo.com/t5/support/ct-p/Support)或电子邮件`customercare@marketo.com`中的文件支持案例。

* 支持后迁移完成：产品支持管理员可以通过Experience League支持门户提交案例。

如果您获得最终成功，则可以访问Admin Console迁移白手套服务。 请联系Adobe客户团队（您的客户经理）寻求帮助。

**如果我使用Adobe身份访问其他Adobe应用程序，能否使用该身份访问Marketo？**

即使您有其他Adobe产品，在将订阅迁移到IMS之前，您无法使用Adobe身份访问Marketo。

**Marketo用户角色（位于工作区中）是否在Adobe Admin Console中进行管理？**

不会。用户Marketo Engage管理（在工作区中）已完成。

**我是IMS集成订阅中的Marketo管理员，无权访问该Admin Console。 如何获取访问权限？**

任何有权访问贵组织Admin Console的Adobe系统或产品管理员都可以为您提供访问权限。 如果您不确定组织中的哪些人具有控制台中的管理员权限，请联系[Adobe客户关怀](https://helpx.adobe.com/contact.html){target="_blank"}。

**管理员如何将用户添加到Marketo [!DNL Sales Connect]？**

虽然[!DNL Sales Connect]的Admin Console中会有产品卡，但不应使用Admin Console添加/管理用户。 以下链接将允许管理员通过Marketo [!DNL Sales Connect]管理用户： [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}。

**在哪里可以了解有关Adobe Admin Console的更多信息？**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/cn/enterprise/admin-guide.html){target="_blank"}。

**我是否仍要转到Marketo中的“管理员”部分以更改我的帐户？**

否，您需要导航到[account.adobe.com](https://account.adobe.com){target="_blank"}。

**这如何与Marketo的通用ID一起使用？**

已载入Adobe身份的用户可以通过产品中的订阅切换器无缝访问所有支持IMS的订阅。

**此项是否适用于SSO？**

可以。Marketo与Adobe IMS的集成支持通用ID用户和SSO。 SSO现在由Adobe IMS驱动，在Adobe Admin Console的组织级别设置。 [在此了解详情](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

**我已登记使用Adobe身份，现在我要实施SSO。 我该怎么办？**

如果您希望实施单点登录并且您的订阅已登记到Adobe身份，但未在Adobe组织中实施SSO，请将票证提交到[Marketo支持](https://nation.marketo.com/){target="_blank"}，并将主题指定为“Admin Console上的Marketo，实施SSO”。

**设备授权的工作原理是什么？**

Adobe IMS当前不支持Marketo的设备授权功能等任何功能。

**仍然可以使用“在邀请用户对话框中登录”功能来使用户的登录在其电子邮件中是唯一的？**

不会。订阅启用了IMS时，用户邀请工作流不再有效，因此功能不再有效。 Adobe身份要求用户的身份由其电子邮件驱动。

**对于Adobe IMS，我们是否可以选择使用Adobe ID、Enterprise ID或Federated ID？**

是，您可以确定组织支持的身份类型。 可在以下位置找到更多信息： [身份概述](https://helpx.adobe.com/cn/enterprise/using/identity.html)和此处： [设置身份](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

**Adobe Admin Console支持哪些产品卡？**

支持的产品卡包括：Marketo Engage、Marketo Measure、MarketoDynamic Chat、Marketo Sales Connect和Marketo Sales Insight Actions。

**如果我迁移到Adobe身份后，我的用户登录与电子邮件不符，该怎么办？**

登录名不同于其电子邮件地址的当前Marketo Engage用户在迁移到Adobe身份后，将不再使用该凭据登录。 Adobe身份始终使用用户的电子邮件地址进行身份验证。 您可以在[account.adobe.com](https://account.adobe.com){target="_blank"}上更新Adobe身份电子邮件地址。

**如果我的订阅使用IP限制设置，则在Adobe身份迁移之后会发生什么情况？**

将订阅登记到Adobe身份后，IP限制设置不会迁移到Adobe Admin Console。 Marketo的IP限制设置包括仅允许从特定IP地址访问，以及阻止特定IP地址访问。 目前，AdobeIdentity Management System不支持IP限制功能。

Identity Management SystemAdobe功能将于2025年初推出，将发布一项支持仅允许特定IP地址的功能，支持当前使用此功能的Marketo用户进行过渡。 在功能发布之前，当前使用此功能的用户将不会进行用户迁移。 交付功能后，用户将收到其迁移已安排的通知。 有关该功能的更多信息，将在可用时提供。

当前使用IP限制并阻止特定地址访问的用户在迁移到Adobe身份后将无法再使用此功能，因为AdobeIdentity Management System不支持此功能。

**如果我的Adobe具有“绕过单点登录”的选项，则在用户身份迁移后会发生什么情况？**

将订阅登记到Adobe身份后，将在Adobe组织级别为所有用户设置单点登录(SSO)。 设置单点登录后，将对该Adobe组织中的所有Marketo用户/所有Marketo实例强制实施该设置。以前，Marketo支持将用户角色设置为“绕过单点登录”选项。 AdobeIdentity Management System不支持此功能。

**我有多个订阅，但并非所有订阅都启用了单点登录。 Adobe身份迁移后会发生什么情况？**

将订阅登记到Adobe身份后，将在Adobe组织级别设置单点登录(SSO)。 这意味着SSO适用于Adobe组织中的所有产品实例。设置SSO后，它将应用于该Adobe组织中的所有Marketo实例。以前，Marketo在实例级别支持此设置。 AdobeIdentity Management System不支持此功能。

**我现在必须导航到Experience Cloud才能访问Marketo Engage。 是否有办法简化此流程？**

可以。您可以为单击Marketo Engage实例入口页面上的&#x200B;**启动**&#x200B;按钮后启动的链接创建浏览器书签，以绕过该页面。

![](assets/faq-1.png)

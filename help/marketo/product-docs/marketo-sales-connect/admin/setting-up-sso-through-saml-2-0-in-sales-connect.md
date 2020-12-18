---
unique-page-id: 14352405
description: 在Sales Connect - Marketo Docs —— 产品文档中通过SAML 2.0设置SSO
title: 在Sales Connect中通过SAML 2.0设置SSO
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# 在Sales Connect {#setting-up-sso-through-saml-in-sales-connect}中通过SAML 2.0设置SSO

我们通过SAML 2.0规范支持SSO。 但是，目前我们没有与任何提供商直接集成。 我们需要从您的SSO提供商收集一些信息，才能获得此设置。

>[!NOTE]
>
>**提醒**
>
>这仅适用于&#x200B;**Marketo Sales Connect**&#x200B;客户。 如果您没有Sales Connect，但想了解更多信息，请与您的客户成功经理联系。

## 要求{#requirements}

* SSO帐户
* Marketo Sales connect订阅
* 来自SSO帐户的metadata.xml（问题URL、验证的端点和公钥）

## 设置{#setup}

团队SSO实例中的metadata.xml应包含颁发者URL、验证端点和公钥。

我们还需要您公司的SSO帐户的SSO位置作为唯一域。 例如，我们`require a unique subdomain`喜欢“toutapp.pingidentity.com”或类似。 如果没有此类型的唯一标识符，我们将无法从仪表板设置SAML。

在分配URL时，一个登录名和Okta并不始终提供唯一标识符。 如果您使用Okta或One Login，则意味着我们无法从仪表板按钮设置一次登录。 我们仍然能够从[Web应用程序](http://toutapp.com/login)的“单一登录”按钮设置它。

获得这些信息后，我们将与我们的工程团队合作，为您的订阅设置这些信息。

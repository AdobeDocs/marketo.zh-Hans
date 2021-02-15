---
unique-page-id: 14352405
description: 在Sales Connect - Marketo Docs — 产品文档中通过SAML 2.0设置SSO
title: 在Sales Connect中通过SAML 2.0设置SSO
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# 在Sales Connect {#setting-up-sso-through-saml-in-sales-connect}中通过SAML 2.0设置SSO

我们通过SAML 2.0规范支持SSO。 但是，目前我们没有与任何提供商进行直接集成。 我们需要从您的SSO提供商收集一些信息，才能获得此设置。

>[!NOTE]
>
>这仅适用于&#x200B;**Marketo Sales Connect**&#x200B;客户。 如果您没有Sales Connect，但想了解更多信息，请联系您的客户成功经理。

## 要求{#requirements}

* SSO帐户
* Marketo Sales connect订阅
* 来自SSO帐户的Metadata.xml（问题URL、验证的端点和公钥）

## 设置{#setup}

您团队的SSO实例中的metadata.xml应包含颁发者URL、验证的端点和公钥。

我们还需要您公司的SSO帐户的SSO位置作为唯一域。 例如，我们需要一个唯一的子域，如`toutapp.pingidentity.com`或类似的子域。 如果没有此类型的唯一标识符，我们将无法从仪表板设置SAML。

在分配URL时，一个登录名和Okta并不始终提供唯一标识符。 如果您使用Okta或One Login，则意味着我们无法从“仪表板”按钮设置一次登录。 我们仍然能够从[Web应用程序](https://toutapp.com/login)上的“单点登录”按钮进行设置。

获得该信息后，我们将与我们的工程团队合作，为您的订阅设置此信息。

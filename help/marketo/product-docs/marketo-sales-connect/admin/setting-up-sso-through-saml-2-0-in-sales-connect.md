---
unique-page-id: 14352405
description: 在Sales Connect - Marketo文档 — 产品文档中通过SAML 2.0设置单点登录
title: 在Sales Connect中通过SAML 2.0设置单点登录
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 在Sales Connect中通过SAML 2.0设置单点登录 {#setting-up-sso-through-saml-in-sales-connect}

我们通过SAML 2.0规范支持单点登录。 但是，我们目前没有与任何提供商进行直接集成。 我们需要从您的SSO提供商收集一些信息才能进行此设置。

>[!NOTE]
>
>这仅适用于 **Marketo Sales Connect** 用户。 如果您没有Sales Connect，但想了解更多信息，请联系Adobe客户团队（您的客户经理）。

## 要求 {#requirements}

* SSO帐户
* Marketo Sales Connect订阅
* 来自SSO帐户的metadata.xml（问题URL、验证端点和公钥）

## 设置 {#setup}

您团队的SSO实例中的metadata.xml应包含颁发者URL、验证的端点和公钥。

我们还需要您公司的SSO帐户的SSO位置作为唯一域。 例如，我们需要一个唯一的子域，如 `toutapp.pingidentity.com` 或类似。 如果没有此类型的唯一标识符，我们将无法从仪表板设置SAML。

在分配URL时，一次登录和Okta并不总是提供唯一标识符。 如果您使用Okta或一次登录，则意味着我们将无法从功能板按钮设置一次登录。 我们仍然可以通过 [Web应用程序](https://toutapp.com/login).

获取该信息后，我们将与我们的工程团队合作，为您的订阅设置此信息。

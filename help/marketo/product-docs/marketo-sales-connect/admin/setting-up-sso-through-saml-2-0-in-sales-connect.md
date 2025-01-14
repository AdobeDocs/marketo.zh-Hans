---
unique-page-id: 14352405
description: 在Sales Connect中通过SAML 2.0设置SSO - Marketo文档 — 产品文档
title: 通过Sales Connect中的SAML 2.0设置SSO
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# 通过Sales Connect中的SAML 2.0设置SSO {#setting-up-sso-through-saml-in-sales-connect}

我们通过SAML 2.0规范支持SSO。 但是，我们目前未与任何提供商直接集成。 我们需要从您的SSO提供商处收集一些信息才能进行此设置。

>[!NOTE]
>
>这仅适用于&#x200B;**Marketo Sales Connect**&#x200B;用户。 如果您没有Sales Connect但想了解更多信息，请联系Adobe客户团队（您的客户经理）。

## 要求 {#requirements}

* SSO帐户
* Marketo Sales Connect订阅
* SSO帐户中的Metadata.xml（问题URL、验证端点和公钥）

## 设置 {#setup}

您团队的SSO实例中的metadata.xml应包含颁发者URL、验证端点和公钥。

我们还需要贵公司的SSO帐户的SSO位置作为唯一域。 例如，我们需要唯一的子域，如`toutapp.pingidentity.com`或类似项。 如果没有此类唯一标识符，我们将无法从仪表板设置SAML。

在分配URL时，一个Login和Okta并不总是提供唯一标识符。 如果您使用Okta或“一次登录”，这意味着我们将无法从仪表板按钮设置一次登录。 我们仍可以通过[Web应用程序](https://toutapp.com/login)上的“单点登录”按钮进行设置。

收到该信息后，我们将与工程团队合作，为您的订阅设置此项。

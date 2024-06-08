---
unique-page-id: 2359828
description: 将SSL添加到登陆页面 — Marketo文档 — 产品文档
title: 将SSL添加到登陆页面
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: d5993d7c638994ea93446d20cbd1f1ae0b25e622
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# 将SSL添加到登陆页面 {#add-ssl-to-your-landing-pages}

通过SSL（安全套接字层）加密，您可以确保Marketo Engage实例的所有登陆页面安全。

在填写Web表单或访问由Marketo Engage托管的登陆页时，默认情况下，信息会通过非安全协议(HTTP)发送。 根据贵公司的策略，您可能希望保护通过(HTTPS)提交到Marketo的信息。 例如，当您访问 `http://info.mydomain.com/` 现在将是 `https://info.mydomain.com/`.

默认情况下，Marketo Engage会通过非安全HTTP协议跟踪“已访问的网页”和“单击网页上的链接”。 如果您希望使用自己的证书来保护跟踪链接，则需要让Marketo构建单独的非共享服务器来启用它。 要确保联系人与您交互的各个方面的安全，通常意味着同时保护登陆页面和跟踪链接。

2022年底，对登陆页面和跟踪链接域的安全方式进行了更改。 [在此处了解它们](https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305){target="_blank"}.

如果您希望为Marketo Engage登陆页面使用SSL，请联系Adobe客户团队（您的客户经理）。

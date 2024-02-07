---
description: 通知 — Websocket连接 — Marketo文档 — 产品文档
title: 通知 — Websocket连接
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 10fe526c672867b93b54e99e492e59c0541c3f36
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# 通知： Websocket连接 {#notification-websocket-connection}

本文适用于在其Marketo实例中收到以下通知的Marketo Engage用户： `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are connected to now on March 3, 2024. Please work with your IT team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

如果您或您的组织使用限制性的防火墙或代理服务器设置，则您或您的网络管理员可能需要允许列表某些域和IP地址范围，以确保Adobe Marketo Engage按预期工作。

Marketo支持未设置为协助实施以下协议。 如果您需要帮助，请与您的IT团队分享此文章。 如果他们使用允许列表限制Web访问，请让他们添加以下域（包括星号）以允许所有Marketo资源和Web套接字：

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

---
description: 收到“无法建立Websocket连接”通知的Marketo Engage用户的通知详细信息
title: 通知 — Websocket连接
hide: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
TQID: https://experienceleague.adobe.com/NpcRnxQPi03CF8z77Urrfs2P2phkuRbh2pd5J1UquFk
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 123
ht-degree: 30%

---

# 通知：Websocket 连接 {#notification-websocket-connection}

本文档适用于在其Marketo实例中收到以下通知的Marketo Engage用户：`"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

如果您或您的组织使用了较为严格的防火墙或代理服务器设置，您或您的网络管理员可能需要将某些域名和 IP 地址范围加入允许列表，以确保 Adobe Marketo Engage 能够正常运行。

Marketo支持未设置为协助实施以下协议。 如果您需要帮助，请将此文档与您的IT团队共享。 如果他们使用允许列表限制Web访问，请让他们添加以下域（包括星号）以允许所有Marketo资源和Web套接字：

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

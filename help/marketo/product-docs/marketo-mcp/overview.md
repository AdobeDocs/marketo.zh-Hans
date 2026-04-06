---
description: 即将推出。
title: MCP概述文档
hide: true
hidefromtoc: true
source-git-commit: 62f5166e6a77c8ef50e7c596754205e8f02c6dc7
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# MCP概述文档 {#overview}

ATHER的文本：

Marketo Engage公共MCP服务器是一种基于云的服务，它使AI代理能够将Marketo REST API作为结构化工具访问。 基于模型上下文协议(MCP)，它提供了一个标准化的模式驱动接口，允许AI系统安全高效地与Marketo交互。

MCP服务器不会将Marketo端点手动集成到每个应用程序中，而是会提供一个AI本机网关，以便与MCP兼容的代理能够发现可用的操作、了解所需的参数并通过一致的协议执行操作。

有许多可用工具包含公共REST API和内部API，它们像在UI中一样执行Marketo核心功能，但通过API调用。 随着工具的开发，将不断添加更多工具。 &lt;----需要说明

MCP服务器作为自助服务提供，并且可以通过构建端点和验证连接来通过Adobe IO框架进行设置。 有关更多信息和设置详细信息，请访问Adobe Developer网站（在此处添加链接）。 这个？ https://developer.adobe.com/marketo-apis/

显示为SOAP API的Campaign工具已转换为REST API并已添加。

配置完毕后，要查看可用工具列表，请在此处按照这些说明（超链接）操作。

注意：不可用的工具有“停用营销活动”和“删除静态列表”（待定）。

/////////////////////////////////////

## 设置 {#settings}

请按照以下步骤将NAME连接到您的Marketo Engage帐户。

1. 在“我的Marketo”中，单击&#x200B;**使用AI构建**&#x200B;拼贴。

屏幕快照

1. 单击齿轮图标

将需要尚未连接的实例
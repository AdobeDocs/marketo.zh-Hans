---
description: 代理管理 — Marketo文档 — 产品文档
title: 代理管理
feature: Dynamic Chat
exl-id: 151d8cf2-a5b7-43c4-8418-cc22252108b2
source-git-commit: 42e2a23c1c451c61fd62237fd1305924b51437b2
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 1%

---

# 代理管理 {#agent-management}

在代理管理中，查看Dynamic Chat实例中的代理列表、管理团队并设置回退规则。

![](assets/agent-management-1.png)

## 代理 {#agents}

此选项卡列出了您的Dynamic Chat实例中的所有座席，并包括他们的姓名、电子邮件地址、实时聊天状态等信息。

![](assets/agent-management-2.png){width="800" zoomable="yes"}

>[!NOTE]
>
>没有看到您&#x200B;_只添加了_&#x200B;的代理？ 在Adobe Admin Console中添加它们后，它们最多可能需要两个小时才能显示在此处。

## 团队 {#teams}

管理员可以创建座席小组，以便于路由到特定的销售座席组。

>[!AVAILABILITY]
>
>要访问Teams，需要订阅Dynamic Chat Prime。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

![](assets/agent-management-3.png)

### 创建团队 {#create-a-team}

1. 单击&#x200B;**+创建团队**。

   ![](assets/agent-management-4.png)

1. 为您的团队命名。

   ![](assets/agent-management-5.png)

1. 单击&#x200B;**添加代理**&#x200B;下拉列表并选择所需的代理。

   ![](assets/agent-management-6.png)

1. 单击&#x200B;**创建**。

   ![](assets/agent-management-7.png)

## 回退规则 {#fallback-rules}

### 会议回退 {#meeting-fallback}

选择标准（系统）消息或编写自定义消息，以供访客在会议预订不可用时查看。

![](assets/agent-management-8.png)

### 实时聊天后备 {#live-chat-fallback}

选择标准（系统）消息或编写自定义消息，以供访客在实时聊天不可用时查看。

![](assets/agent-management-9.png)

>[!NOTE]
>
>* 选中&#x200B;_包括会议预约选项_&#x200B;复选框将使聊天访客能够在没有座席可供实时聊天时预约会议。
>
>* **对于任何自定义规则/团队作为实时聊天卡**：在检查代理时，如果代理不可用或无法连接，则将回退到循环调度以尝试“可用的代理”（当时所有可用的代理，无论在流中放置了哪个路由逻辑/规则）。

>[!TIP]
>
>创建自定义消息时，您可以设置字体样式，使用链接，甚至插入表情符号！`:)`

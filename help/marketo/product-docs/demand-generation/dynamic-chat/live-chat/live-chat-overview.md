---
description: 实时聊天概述 — Marketo文档 — 产品文档
title: 实时聊天概述
feature: Dynamic Chat
source-git-commit: 8b2eed5e28c46ea9c467fd25dd732c1654a09bed
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 1%

---

# 实时聊天概述 {#live-chat-overview}

通过实时聊天，网站访客可与您的销售代理进行实时聊天对话。

## 添加实时聊天代理 {#add-live-chat-agents}

要开始实时聊天，您需要将实时聊天代理添加为 [Adobe Admin Console中的用户](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. 完成此操作后，您可以添加 [实时聊天卡](#using-the-live-chat-card) 到新的或现有的对话框。

当访客通过Dialog请求与座席聊天时，座席将拥有多个 [通知选项](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} 在那里他们可以和访客聊天。

## 使用实时聊天卡 {#using-the-live-chat-card}

使用中的实时聊天卡 [流设计器](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} 您希望访客与实时座席聊天的情况。

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>实时聊天卡必须始终是分支中的最后一张卡。 如果该卡片放置在分支中的随机点上，则可能会突然将访客与代理连接起来，从而令访客感到惊讶。

### 最佳实践 {#best-practices}

* 在实时聊天卡之前使用问题卡询问访客是否愿意连接。
* 在访客同意连接后，使用信息捕获卡收集其某些信息，如名字/姓氏、电子邮件地址、职位等。 （建议至少请求提供名字和电子邮件地址）。

## 实时聊天卡选项 {#live-chat-card-options}

单击流中的实时聊天卡允许您选择访客的路由方式。 从循环配置资源、代理、自定义规则或团队中进行选择。

![](assets/live-chat-overview-2.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>循环</b></td>
   <td>聊天按顺序分配给座席。</td>
  </tr> 
  <tr> 
   <td><b>代理</b></td>
   <td>选择要接收聊天的特定座席。</td>
  </tr>
    <tr> 
   <td><b>自定义规则</b></td>
   <td>在考虑将访客路由到何处时，所有自定义规则都将循环使用。 如果访客不符合任何自定义规则的条件，他们将获得 <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">实时聊天后备消息</a>.</td>
  </tr> 
  <tr> 
   <td><b>团队</b></td>
   <td>选择要接收聊天的特定团队。 如果选择该选项，将在该组内为其分配循环调度法。</td>
  </tr>
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[代理收件箱](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}

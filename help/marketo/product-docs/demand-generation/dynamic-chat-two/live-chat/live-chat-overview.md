---
description: 实时聊天概述 — Marketo文档 — 产品文档
title: 实时聊天概述
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 863e5e542e2006ee15f44ad949e876e56a9b39e3
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 2%

---

# 实时聊天概述 {#live-chat-overview}

使用中的实时聊天卡 [流设计器](/help/marketo/product-docs/demand-generation/dynamic-chat-two/automated-chat/stream-designer.md){target="_blank"} 您希望访客与实时座席聊天的情况。

## 使用实时聊天卡 {#using-the-live-chat-card}

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>实时聊天卡必须始终是分支中的最后一张卡。 如果该卡片放置在分支中的随机点上，则可能会突然将访客与代理连接起来，从而令访客感到惊讶。

**最佳实践**

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
   <td>在考虑将访客路由到何处时，所有自定义规则都将循环使用。 如果访客不符合任何标准，他们将使用“回退规则”???</td>
  </tr> 
  <tr> 
   <td><b>团队</b></td>
   <td>选择要接收聊天的特定团队。 如果选择该选项，将在该组内为其分配循环调度法。</td>
  </tr>
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>* [代理收件箱](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/agent-inbox.md){target="_blank"}
>* [通知](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/notifications.md){target="_blank"}
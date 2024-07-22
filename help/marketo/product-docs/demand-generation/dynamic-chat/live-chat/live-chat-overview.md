---
description: 实时聊天概述 — Marketo文档 — 产品文档
title: 实时聊天概述
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: 14ccfe39059b9c900a5e5e00b082146bb500d79d
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 0%

---

# 实时聊天概述 {#live-chat-overview}

通过实时聊天，网站访客可与您的销售代理进行实时聊天对话。

>[!NOTE]
>
>对于Dynamic ChatSelect程序包上的用户，实时聊天是一项试用功能，其生命周期限制为100次参与。 当达到此限制时，任何请求与实时代理进行聊天的访客都不会连接，而是会收到全局回退消息。 要提高限制，请联系您的Adobe客户代表以讨论包升级选项。

## 添加实时聊天代理 {#add-live-chat-agents}

要开始实时聊天，您需要将实时聊天代理添加为[Adobe Admin Console中的用户](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"}，并授予他们[实时聊天权限](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}。 完成此操作后，您可以将[实时聊天卡](#using-the-live-chat-card)添加到新的或现有的对话框中。

当访客通过Dialog请求与代理聊天时，代理将有多个[通知选项](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}。 当他们单击通知时，会被转到其[代理收件箱](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}，以便开始与访客聊天。

>[!NOTE]
>
>实时座席头像使用座席的Adobe帐户个人资料中的个人资料图片。 要更新图像，请执行[这些步骤](https://helpx.adobe.com/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"}。

## 使用实时聊天卡 {#using-the-live-chat-card}

当您希望访客与实时代理聊天时，请使用[流Designer](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}中的实时聊天卡。

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
   <td>在考虑将访客路由到何处时，所有自定义规则都将循环使用。 如果访客不符合任何自定义规则的条件，他们将获得<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">实时聊天后备消息</a>。</td>
  </tr> 
  <tr> 
   <td><b>团队</b></td>
   <td>选择要接收聊天的特定团队。 如果选择该选项，将在该组内为其分配循环调度法。</td>
  </tr>
 </tbody> 
</table>

## 实时聊天通知 {#live-chat-notifications}

>[!IMPORTANT]
>
>为了接收用于实时聊天的浏览器通知，所有实时聊天代理必须在出现提示时启用Dynamic Chat的浏览器通知。

### 启用通知 {#enabling-notifications}

实时聊天代理登录时，会在屏幕顶部看到一条横幅，上面显示“请启用浏览器通知以接收实时聊天通知”。 单击&#x200B;**启用**。

![](assets/live-chat-overview-4.png)

随后，浏览器将提示实时聊天代理显示通知。 单击&#x200B;**允许**。

![](assets/live-chat-overview-5.png)

如果座席在允许浏览器进入后仍未收到浏览器通知，则可能需要在操作系统通知设置中为浏览器启用通知：

Mac的[步骤](https://support.apple.com/guide/mac-help/change-notifications-settings-mh40583/mac){target="_blank"}

用于Windows的[步骤](https://support.microsoft.com/en-us/windows/change-notification-settings-in-windows-8942c744-6198-fe56-4639-34320cf9444e){target="_blank"}

### 当实时聊天路由到座席时 {#when-a-live-chat-is-routed-to-an-agent}

当实时聊天被路由到座席时，他们将看到屏幕顶部有一条蓝色横幅要求他们接受。

![](assets/live-chat-overview-3.png)

>[!TIP]
>
>您还可以选择设置浏览器通知，如果您未登录Dynamic Chat，通知会提醒您。
>
>* 在[Google Chrome](https://support.google.com/chrome/answer/3220216?hl=en&amp;co=GENIE.Platform%3DDesktop){target="_blank"}中启用浏览器通知
>* 在[Mozilla Firefox](https://support.mozilla.org/en-US/kb/push-notifications-firefox){target="_blank"}中启用浏览器通知

### 注意事项 {#things-to-note}

* 在“接受聊天”消息超时之前，工程师有45秒的时间进行响应。 之后，访客将收到[回退消息](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback){target="_blank"}。 对于路由选项设置为&#x200B;**团队**&#x200B;的Dynamic ChatPrime订阅者，将在显示回退消息之前再尝试一个代理。
* 目前每个代理最多只能进行10次实时聊天。

>[!MORELIKETHIS]
>
>[代理收件箱](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}

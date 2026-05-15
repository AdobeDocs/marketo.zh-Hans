---
description: 发行说明 — 2025年9月 — Marketo文档 — 产品文档
title: 发行说明 — 2025年9月
feature: Release Information
exl-id: fd40d9df-67ba-4fc4-891f-81aebfd07b0a
TQID: https://experienceleague.adobe.com/WfcIv3NWuYLgVCvHGcGmKbE6pDLOJ6FBk0OAX5uNJDE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 960
ht-degree: 0%

---

# 发行说明：2025年9月 {#release-notes-sep-25}

在下方，您会找到2025年9月版本中包含的所有功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

可以在此处[&#128279;](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}找到特定于Adobe Dynamic Chat 的发行说明。

>[!AVAILABILITY]
>
>以星号（![星号](assets/yellow-star.png)）表示的功能是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

## 标准发行周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2025年9月19日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 发行功能和日期可能会发生更改。 请检查每个功能旁边的状态信息。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>按需网络研讨会活动保留</strong>：交互式网络研讨会用户现在拥有超过30天的按需网络研讨会仪表板数据（以前，从网络研讨会开始算起最多只能使用30天）。</td>
   <td>已发布</td>
   <td><a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/event-workflows#manual-sync">手动同步</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer - AI助手权限</strong>： Marketo管理员可以为特定用户提供对GenAI功能的访问权限。</td>
   <td>已发布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/ai-assistant.md#set-up-permissions">设置权限</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 深色模式</strong>：您现在可以使用深色模式，该模式允许支持电子邮件客户端和应用程序显示具有更暗背景和更浅颜色的电子邮件，以用于文本、按钮和其他UI元素。</td>
   <td>已发布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md">深色模式</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>向Designer发送电子邮件 — Content Collaboration工作流程</strong>：您现在可以在电子邮件资源中评论并与Marketo同事协作。 标记团队成员（具有相应资源权限的Marketo用户），他们将会收到电子邮件或脉冲通知。</td>
   <td>已发布</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/email-collaboration.md">电子邮件协作</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 重定向修复</strong>：某些用户在使用新Designer创建的电子邮件的URL时遇到重定向问题（例如，直接粘贴URL或为电子邮件资源添加书签并不总是有效）。 此问题已得到解决。 此外，从<b>电子邮件模板</b> &gt; <b>详细信息</b> &gt; <b>用于</b>的电子邮件资源链接将重定向到相应的电子邮件资源。</td>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **弃用REST API双斜杠**： 2025年9月16日，Adobe为利用新技术的REST API URL过渡到了更现代的托管基础架构，从而增加了安全性和可扩展性。 如果您的订阅在URL中使用了带有双正斜杠(//)的API，请阅读[此国家/地区帖子](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"}以了解后续步骤。

* **在新电子邮件Designer中切换回Velocity脚本**： Adobe Marketo Engage在过去的6月为新电子邮件Designer发布了一项名为&#x200B;_条件内容_&#x200B;的功能。 该功能由Handlebar脚本而不是Velocity脚本提供支持，旨在为您的动态内容提供更大的灵活性。 但是，当我们发现它导致某些令牌无法正确解析时，我们决定暂时禁用它。 [了解更多](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage标识生命周期结束**： 2025年8月，Adobe开始逐步停止对Marketo Engage标识的支持（通过`login.marketo.com`登录）。 要防止对Marketo Engage的访问中断，您必须不迟于2025年9月30日过渡到[Adobe身份](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}。

   * _IP限制弃用_：对[基于IP限制Marketo登录的支持](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}已于2025年7月30日结束。 该功能将保持可操作状态，直到完成到Adobe Identity的过渡。 Adobe Admin Console中针对Adobe Identity的基于位置的新访问控制功能即将推出。

   * _单点登录(SSO)弃用_：对[Marketo标识SSO](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"}的支持已于2025年7月30日结束。 该功能将保持可操作状态，直到完成到Adobe Identity的过渡。 Adobe Admin Console中Adobe Identity的单一登录必须单独配置。 有关设置步骤，请参阅[设置标识和单点登录](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

* **弃用&#x200B;_转发给Friend_功能**：2025年9月29日，Marketo Engage 2.0电子邮件（旧版电子邮件编辑器）中的&#x200B;_转发给Friend_&#x200B;功能将完全对所有订阅弃用。 这会影响已发送或将使用该令牌发送的电子邮件中的“转发给朋友”令牌和“转发给朋友”链接。 [了解详情](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Rest API &#39;access_token&#39;参数弃用**：用于验证Marketo REST API调用的`access_token`查询参数已被弃用，并将在2026年3月31日之后不可用。 所有新的和现有的集成都应使用“授权”标头[来验证REST API调用，如此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}所述。

* **SOAP API弃用**：对Marketo SOAP API的支持将于2026年3月31日终止。 使用SOAP API功能的服务应迁移到[REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

* **弃用旧版商机活动数据流**：在2026年6月底之前，用户必须从旧版商机活动数据流迁移到新的Adobe I/O商机活动数据流(LADS)。 此弃用仅影响少数在与Adobe I/O Events集成之前载入潜在客户活动数据流的用户。 如果您是新数据流用户，或者已经通过I/O事件管理潜在客户活动数据流，这对您没有任何影响。 有关迁移详细信息，请参阅[本文](https://developer.adobe.com/events/docs/guides/using/marketo/marketo-lead-activity-data-stream-migration){target="_blank"}。

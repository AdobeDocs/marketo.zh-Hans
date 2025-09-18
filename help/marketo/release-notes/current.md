---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 29c1b59c9d2598626f546554a8bdc1b26b9e1590
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 72%

---

# 发行说明：2025 年 9 月 {#release-notes-sep-25}

以下是 2025 年 9 月版本中包含的所有功能。请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。请联系您的 Marketo Engage 代表了解更多信息。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发布周期，将于 **2025 年 9 月 19 日**&#x200B;开始发布，并在接下来的数周内分阶段推出其余功能。功能及发布时间可能会有变动。请查看每个功能旁的状态标记。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>按需网络研讨会活动保留</strong>：交互式网络研讨会用户现在可以获得按需网络研讨会仪表板数据超过 30 天（以前，从网络研讨会之日起最多只能获得 30 天）。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer - Content Collaboration工作流程</strong>：您现在可以在电子邮件资源中评论并与Marketo同事协作。 标记团队成员(具有相应资源权限的Marketo用户)，他们将会收到电子邮件或脉冲通知。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer - AI助手权限</strong>： Marketo管理员可以为特定用户提供对GenAI功能的访问权限。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>深色模式</strong>：您现在可以使用深色模式，该模式允许支持电子邮件客户端和应用显示具有更暗背景和更浅颜色的电子邮件，用于文本、按钮和其他UI元素。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 重定向修复</strong>：某些用户在使用新Designer创建的电子邮件的URL时遇到重定向问题（例如，直接粘贴URL或为电子邮件资源添加书签并不总是有效）。 此问题已得到解决。 此外，从<b>电子邮件模板</b> &gt; <b>详细信息</b> &gt; <b>用于</b>的电子邮件资源链接将重定向到相应的电子邮件资源。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **在新的电子邮件设计器中切换回 Velocity 脚本**：Adobe Marketo Engage 于今年 6 月为新的电子邮件设计器发布了一项名为&#x200B;_条件内容_&#x200B;的功能。该功能由 Handlebar 脚本而不是 Velocity 脚本提供支持，旨在为您的动态内容提供更多的灵活性。但当我们发现它导致一些令牌被错误解析时，我们决定暂时禁用它。[了解详情](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage Identity 结束**：自 2025 年 8 月起，Adobe 开始逐步停止对 Marketo Engage Identity（通过 `login.marketo.com` 登录）的支持。为避免对 Marketo Engage 的访问中断，您必须在 2025 年 9 月 30 日前切换至 [Adobe Identity](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}。

   * _弃用 IP 限制功能_：对[基于 IP 限制 Marketo 登录](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}的支持已于 2025 年 7 月 30 日结束。该功能将在过渡到 Adobe Identity 完成前保持可用。Adobe Admin Console 中 Adobe Identity 的基于位置的全新访问控制功能即将推出。

   * _弃用单点登录（SSO）_：对 [Marketo Identity SSO](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} 的支持已于 2025 年 7 月 30 日结束。该功能将在过渡到 Adobe Identity 完成前保持可用。在 Adobe Admin Console 中为 Adobe Identity 配置单点登录需单独进行。有关设置步骤，请参阅[设置身份标识和单点登录](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

* **弃用&#x200B;_转发给好友_功能**：自 2025 年 9 月 29 日起，Marketo Engage 2.0 电子邮件（旧版电子邮件编辑器）中的&#x200B;_转发给好友_&#x200B;功能将在所有订阅中完全弃用。这会影响已经或将要使用相应令牌发送的电子邮件中的“转发给好友”令牌和“转发给好友”链接。[了解详情](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Rest API &#39;access_token&#39;参数弃用**：用于验证Marketo REST API调用的`access_token`查询参数已被弃用，并将在2026年1月31日之后不可用。 所有新建及现有集成都应使用 &#39;Authorization&#39; 标头验证 REST API 调用，[详细说明请参阅此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API弃用**：对Marketo SOAP API的支持将于2026年1月31日终止。 使用 SOAP API 功能的服务应迁移至 [REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

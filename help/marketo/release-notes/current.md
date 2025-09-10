---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 95dda7d6e09f0e64fbce8e5bd39613f10ebde382
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 70%

---

# 发行说明：2025 年 9 月 {#release-notes-sep-25}

在下方，您会找到2025年9月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。请联系您的 Marketo Engage 代表了解更多信息。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2025年9月19日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。请查看每个功能旁的状态标记。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>按需网络研讨会活动保留</strong>：交互式网络研讨会用户现在拥有超过30天的按需网络研讨会仪表板数据（以前，从网络研讨会开始算起最多只能使用30天）。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **在新电子邮件Designer中切换回Velocity脚本**： Adobe Marketo Engage在过去的6月为新电子邮件Designer发布了一项名为&#x200B;_条件内容_&#x200B;的功能。 该功能由Handlebar脚本而不是Velocity脚本提供支持，旨在为您的动态内容提供更大的灵活性。 但是，当我们发现它导致某些令牌无法正确解析时，我们决定暂时禁用它。 [了解详情](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage Identity 结束**：自 2025 年 8 月起，Adobe 开始逐步停止对 Marketo Engage Identity（通过 `login.marketo.com` 登录）的支持。为避免对 Marketo Engage 的访问中断，您必须在 2025 年 9 月 30 日前切换至 [Adobe Identity](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}。

   * _弃用 IP 限制功能_：对[基于 IP 限制 Marketo 登录](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}的支持已于 2025 年 7 月 30 日结束。该功能将在过渡到 Adobe Identity 完成前保持可用。Adobe Admin Console 中 Adobe Identity 的基于位置的全新访问控制功能即将推出。

   * _弃用单点登录（SSO）_：对 [Marketo Identity SSO](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} 的支持已于 2025 年 7 月 30 日结束。该功能将在过渡到 Adobe Identity 完成前保持可用。在 Adobe Admin Console 中为 Adobe Identity 配置单点登录需单独进行。有关设置步骤，请参阅[设置身份标识和单点登录](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

* **弃用&#x200B;_转发给好友_功能**：自 2025 年 9 月 29 日起，Marketo Engage 2.0 电子邮件（旧版电子邮件编辑器）中的&#x200B;_转发给好友_&#x200B;功能将在所有订阅中完全弃用。这会影响已经或将要使用相应令牌发送的电子邮件中的“转发给好友”令牌和“转发给好友”链接。[了解详情](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **REST API ‘access_token’ 参数弃用**：用于验证 Marketo REST API 调用的 `access_token` 查询参数将被弃用，并将在 2025 年 10 月 31 日之后不可用。所有新建及现有集成都应使用 &#39;Authorization&#39; 标头验证 REST API 调用，[详细说明请参阅此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API 弃用**：对 Marketo SOAP API 的支持将于 2025 年 10 月 31 日结束。使用 SOAP API 功能的服务应迁移至 [REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

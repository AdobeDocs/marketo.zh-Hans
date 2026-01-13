---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: c6b8dd17c4337b32c6bb4f0a1b9ce22c1e3b8715
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 48%

---

# 发行说明：2026 年 1 月 {#release-notes-jan-26}

在下方，您会找到2026年1月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。请联系您的 Marketo Engage 代表了解更多信息。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2026年1月30日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。请查看每个功能旁的状态标记。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>功能标题</strong>：功能描述。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>功能标题</strong>：功能描述。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>功能标题</strong>：功能描述。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Adobe Connect功能 {#adobe-connect-features}

Adobe Connect团队已发布这些功能。 Marketo Engage [交互式网络研讨会](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/interactive-webinars-overview){target="_blank"}由Adobe Connect提供支持。 因此，以下功能仅适用于交互式网络研讨会用户。

* **调查Pod**： Adobe Connect 12.11引入了一个新的Survey Pod，允许主机直接在实时会话中设计和提交结构化反馈表单。

* **资源Pod**：新的资源Pod取代了以前的“文件”和“Web链接”Pod，为在实时会话期间共享资源提供了单一、统一的方式。

* **增强的房间界面体验**： Adobe Connect 12.11引入了一个刷新和更现代的房间界面，该界面构建于Adobe最新的Spectrum 2设计框架之上，与跨其他Adobe产品(如Creative Cloud和Experience Cloud)使用的视觉语言一致。

有关完整的详细信息，请参阅[Adobe Connect 12.11发行说明](https://helpx.adobe.com/adobe-connect/release-note/adobe-connect-12-11-release-notes.html){target="_blank"}。

## 公告 {#announcements}

* **Rest API &#39;access_token&#39;参数弃用**：用于验证Marketo REST API调用的`access_token`查询参数已被弃用，并将在2026年3月31日之后不可用。 所有新集成和现有集成都应使用 &#39;Authorization&#39; 头部进行 REST API 调用的身份验证，详细说明[请参阅此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API弃用**：对Marketo SOAP API的支持将于2026年3月31日终止。 使用 SOAP API 功能的服务应迁移至 [REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

* **Marketo Engage标识生命周期结束**：

   * _弃用 IP 限制功能_：对[基于 IP 限制 Marketo 登录](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}的支持已于 2025 年 7 月 30 日结束。该功能将在过渡到 Adobe Identity 完成前保持可用。Adobe Admin Console 中 Adobe Identity 的基于位置的全新访问控制功能即将推出。

   * _弃用单点登录（SSO）_：对 [Marketo Identity SSO](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} 的支持已于 2025 年 7 月 30 日结束。该功能将在过渡到 Adobe Identity 完成前保持可用。在 Adobe Admin Console 中为 Adobe Identity 配置单点登录需单独进行。有关设置步骤，请参阅[设置身份标识和单点登录](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

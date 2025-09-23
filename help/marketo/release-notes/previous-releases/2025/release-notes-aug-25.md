---
description: 发行说明 — 2025年8月 — Marketo文档 — 产品文档
title: 发行说明 - 2025 年 8 月
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 92%

---

# 发行说明：2025 年 8 月 {#release-notes-aug-25}

以下是 2025 年 8 月版本中包含的所有功能。请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。请联系您的 Marketo Engage 代表了解更多信息。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发布周期，将于 **2025 年 8 月 22 日**&#x200B;开始发布，并在接下来的数周内分阶段推出其余功能。功能及发布时间可能会有变动。请查看每个功能旁的状态标记。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>电子邮件设计器 - 报告</strong>：电子邮件性能和电子邮件链接性能报告现在显示使用新的电子邮件设计器创建的电子邮件的数据。</td>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件设计器 - 移除自动完成功能</strong>：令牌个性化编辑器中的自动完成选项指向错误的对象，已被移除。目前没有重新实施此功能的计划。</td>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件设计器 - 电子邮件预览优化</strong>：以前，有些用户在尝试在电子邮件/电子邮件模板/片段详细信息页面中预览电子邮件时遇到加载缓慢的问题。现在优化了此体验，加载速度可提高 60%。</td>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件设计器 - 模板修复</strong>：以前，一些开箱即用的模板存在渲染问题（例如，在特定的浏览器/深色模式下无法正确渲染、图像未对齐、CTA 按钮位置错误及其他一些问题）。此版本已修复所有这些问题。</td>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件设计器 - 内容锁定修复</strong>：以前，如果在内容锁定的情况下创建电子邮件模板，然后将该模板用于创建电子邮件，则即使重置电子邮件或选择“更改设计”，内容仍会一直锁定。此问题已在此版本中修复。</td>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>编辑智能营销活动限制的权限</strong>：管理员现在可以将更改智能营销活动限制的能力限制为仅赋予有权限的用户。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Marketo Engage Identity 结束**：自 2025 年 8 月起，Adobe 开始逐步停止对 Marketo Engage Identity（通过 `login.marketo.com` 登录）的支持。为避免对 Marketo Engage 的访问中断，您必须在 2025 年 9 月 30 日前切换至 [Adobe Identity](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}。

   * _弃用 IP 限制功能_：对[基于 IP 限制 Marketo 登录](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}的支持已于 2025 年 7 月 30 日结束。该功能将在过渡到 Adobe Identity 完成前保持可用。Adobe Admin Console 中 Adobe Identity 的基于位置的全新访问控制功能即将推出。

   * _弃用单点登录（SSO）_：对 [Marketo Identity SSO](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} 的支持已于 2025 年 7 月 30 日结束。该功能将在过渡到 Adobe Identity 完成前保持可用。在 Adobe Admin Console 中为 Adobe Identity 配置单点登录需单独进行。有关设置步骤，请参阅[设置身份标识和单点登录](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

* **弃用&#x200B;_转发给好友_功能**：自 2025 年 9 月 29 日起，Marketo Engage 2.0 电子邮件（旧版电子邮件编辑器）中的&#x200B;_转发给好友_&#x200B;功能将在所有订阅中完全弃用。这会影响已经或将要使用相应令牌发送的电子邮件中的“转发给好友”令牌和“转发给好友”链接。[了解详情](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Rest API &#39;access_token&#39;参数弃用**：用于验证Marketo REST API调用的`access_token`查询参数已被弃用，并将在2026年1月31日之后不可用。 所有新建及现有集成都应使用 &#39;Authorization&#39; 标头验证 REST API 调用，[详细说明请参阅此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API弃用**：对Marketo SOAP API的支持将于2026年1月31日终止。 使用 SOAP API 功能的服务应迁移至 [REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

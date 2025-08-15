---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 8101d9c73571948847d00dfc21f21c39bcd1d975
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 46%

---

# 发行说明：2025 年 8 月 {#release-notes-aug-25}

在下方，您会找到2025年8月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。请联系您的 Marketo Engage 代表了解更多信息。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2025年8月22日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。请查看每个功能旁的状态标记。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 报表</strong>：电子邮件性能和电子邮件链接性能报表现在显示使用新电子邮件Designer创建的电子邮件中的数据。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 电子邮件预览优化</strong>：某些用户尝试在电子邮件/电子邮件模板/片段详细信息页面中预览其电子邮件时，加载时间较慢。 此体验已经过优化，加载时间最多可缩短60%。</td>
   <td><i>即将推出</i></td>
   <td>不适用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 模板修复</strong>：一些现成的模板存在渲染问题(例如，在某些浏览器/深色模式下无法正确渲染、图像未对齐、CTA按钮放置错误等)。 这些功能在此版本中均已修复。</td>
   <td><i>即将推出</i></td>
   <td>不适用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 内容锁定修复</strong>：以前，如果创建了包含内容锁定的电子邮件模板，并且该模板用于创建电子邮件，则即使重置了电子邮件或选择了“更改设计”，内容锁定也会持续存在。 此版本中已修复此问题。</td>
   <td><i>即将推出</i></td>
   <td>不适用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 自动完成删除</strong>：令牌个性化编辑器中的自动完成选项指向错误对象，已被删除。 目前没有计划重新实施它。</td>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
 </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Marketo Engage标识生命周期结束**： 2025年8月，Adobe开始逐步停止对Marketo Engage标识的支持（通过`login.marketo.com`登录）。 为避免对 Marketo Engage 的访问中断，您必须在 2025 年 9 月 30 日前切换至 [Adobe Identity](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}。

   * _IP限制弃用_：对[基于IP限制Marketo登录的支持](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}已于2025年7月30日结束。 该功能将在过渡到 Adobe Identity 完成前保持可用。Adobe Admin Console中针对Adobe Identity的基于位置的新访问控制功能即将推出。

   * _单点登录(SSO)弃用_：对[Marketo标识SSO](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"}的支持已于2025年7月30日结束。 该功能将在过渡到 Adobe Identity 完成前保持可用。在 Adobe Admin Console 中为 Adobe Identity 配置单点登录需单独进行。有关设置步骤，请参阅[设置身份标识和单点登录](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

* **REST API ‘access_token’ 参数弃用**：用于验证 Marketo REST API 调用的 `access_token` 查询参数将被弃用，并将在 2025 年 10 月 31 日之后不可用。所有新建及现有集成都应使用 &#39;Authorization&#39; 标头验证 REST API 调用，[详细说明请参阅此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API 弃用**：对 Marketo SOAP API 的支持将于 2025 年 10 月 31 日结束。使用 SOAP API 功能的服务应迁移至 [REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

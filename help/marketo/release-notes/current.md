---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 49068be70579166eaf0e90a8b2769081a873edd9
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 55%

---

# 发行说明：2025 年 10 月 {#release-notes-oct-25}

在下方，您会找到2025年10月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。请联系您的 Marketo Engage 代表了解更多信息。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2025年10月31日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。请查看每个功能旁的状态标记。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>模板导入器</strong>：从经典电子邮件编辑器导入电子邮件模板，以创建与Design Studio中的新电子邮件Designer兼容的模板。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 条件内容</strong>：新电子邮件Designer的奇偶校验功能，允许您实现令牌以外的电子邮件个性化。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer - A/B测试</strong>：新电子邮件Designer的奇偶校验功能，允许您执行A/B测试以查看哪些类型的内容接收最佳响应。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>向Designer发送电子邮件 — 品牌主题</strong>：您现在可以在Marketo Engage中定义品牌主题。 样式配置可以跨电子邮件模板和其他电子邮件资产重复使用和应用，以实现品牌一致性。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
 <tr>
   <td><strong>Email Designer — 图像到HTML Converter</strong>：上传电子邮件的兼容PNG/JPEG图像文件，该文件将自动转换为HTML以供在新电子邮件Designer中使用。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 克隆电子邮件操作</strong>：您现在可以将电子邮件克隆到营销活动中的另一个项目文件夹中，并快速重用现有电子邮件。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **弃用REST API双斜杠**： 2025年9月16日，Adobe为利用新技术的REST API URL过渡到了更现代的托管基础架构，从而增加了安全性和可扩展性。 如果您的订阅在URL中使用了带有双正斜杠(//)的API，请阅读[此国家/地区帖子](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"}以了解后续步骤。

* **在新的电子邮件设计器中切换回 Velocity 脚本**：Adobe Marketo Engage 于今年 6 月为新的电子邮件设计器发布了一项名为&#x200B;_条件内容_&#x200B;的功能。该功能由 Handlebar 脚本而不是 Velocity 脚本提供支持，旨在为您的动态内容提供更多的灵活性。但当我们发现它导致一些令牌被错误解析时，我们决定暂时禁用它。[了解详情](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage Identity 结束**：自 2025 年 8 月起，Adobe 开始逐步停止对 Marketo Engage Identity（通过 `login.marketo.com` 登录）的支持。为避免对 Marketo Engage 的访问中断，您必须在 2025 年 9 月 30 日前切换至 [Adobe Identity](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}。

   * _弃用 IP 限制功能_：对[基于 IP 限制 Marketo 登录](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"}的支持已于 2025 年 7 月 30 日结束。该功能将在过渡到 Adobe Identity 完成前保持可用。Adobe Admin Console 中 Adobe Identity 的基于位置的全新访问控制功能即将推出。

   * _弃用单点登录（SSO）_：对 [Marketo Identity SSO](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} 的支持已于 2025 年 7 月 30 日结束。该功能将在过渡到 Adobe Identity 完成前保持可用。在 Adobe Admin Console 中为 Adobe Identity 配置单点登录需单独进行。有关设置步骤，请参阅[设置身份标识和单点登录](https://helpx.adobe.com/cn/enterprise/using/set-up-identity.html){target="_blank"}。

* **弃用&#x200B;_转发给Friend_功能**：2025年9月29日，Marketo Engage 2.0电子邮件（旧版电子邮件编辑器）中的&#x200B;_转发给Friend_&#x200B;功能在所有订阅中完全弃用。 这会影响电子邮件中的“转发给朋友”令牌和“转发给朋友”链接，这些电子邮件已使用令牌发送或计划使用该令牌发送。 [了解详情](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **弃用 Rest API ‘access_token’ 参数**：用于 Marketo REST API 调用的身份验证的 `access_token` 查询参数将被弃用，在 2026 年 1 月 31 日之后不可用。所有新集成和现有集成都应使用 &#39;Authorization&#39; 头部进行 REST API 调用的身份验证，详细说明[请参阅此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **弃用 SOAP API**：对 Marketo SOAP API 的支持将于 2026 年 1 月 31 日结束。使用 SOAP API 功能的服务应迁移至 [REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

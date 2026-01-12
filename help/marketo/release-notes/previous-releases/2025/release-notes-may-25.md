---
description: 发行说明 — 2025年5月 — Marketo文档 — 产品文档
title: 发行说明 - 2025 年 5 月
feature: Release Information
exl-id: 99cd1d54-0a80-40fa-9d0c-1cb437be90f0
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 25%

---

# 发行说明：2025 年 5 月 {#release-notes-may-25}

在下方，您会找到2025年5月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。请联系您的 Marketo Engage 代表了解更多信息。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2025年5月23日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。请查看每个功能旁的状态标记。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>适用于电子邮件Designer Assets的基于角色的访问控制</strong>：对基于角色的访问控制(RBAC)系统的新增强功能提供了更细粒度的权限，并改进了由新电子邮件Designer支持的资产的用户管理。</td>
   <td>已发布</td>
   <td><a href="https://nation.marketo.com/t5/latest-product-innovations/product-updates-granular-permissions-to-new-email-designer/ba-p/357057">新电子邮件Designer的粒度权限（博客帖子）</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>克隆在Email Designer中创建的电子邮件</strong>：您现在能够克隆使用新Email Designer创建的现有电子邮件。</td>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>任意属性的触发器令牌</strong>：扩展的触发器令牌列表，支持使用Smart Campaign字段中任意活动属性的数据。</td>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
 </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Facebook离线转化集成更新**：在2025年5月29日，Marketo Engage的[Facebook离线转化](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions){target="_blank"}集成将迁移到新的Meta [转化API](https://developers.facebook.com/docs/marketing-api/conversions-api){target="_blank"}，因为Meta将弃用[离线转化API](https://developers.facebook.com/docs/marketing-api/offline-conversions/){target="_blank"}以便进行图形API版本控制。 有关详细信息，请查看Meta的[通过转化API](https://developers.facebook.com/docs/marketing-api/conversions-api/offline-events/){target="_blank"} （CAPI用于离线）发送离线事件的指南。

* **新Analytics功能 — 公共Beta**：[高级BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"}(以前称为Revenue Explorer和Advanced Report Builder)在4月中旬开始向所有当前Revenue Cycle Explorer用户推出。 此新工具提供了有关Marketo Engage数据的灵活报表和可视化界面，提供了有关进度、性能等内容的精细详细信息。 它具有更丰富的交互性和可视化功能、更快的性能以及更顺畅和直观的用户体验。

要访问此功能，您必须已购买高级BI Analytics加载项。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

* **Rest API &#39;access_token&#39;参数弃用**：用于验证Marketo REST API调用的`access_token`查询参数已被弃用，并将在2026年3月31日之后不可用。 所有新集成和现有集成都应使用 &#39;Authorization&#39; 头部进行 REST API 调用的身份验证，详细说明[请参阅此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API弃用**：对Marketo SOAP API的支持将于2026年3月31日终止。 使用 SOAP API 功能的服务应迁移至 [REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

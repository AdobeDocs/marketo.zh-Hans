---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 48aeac444cca4abfc4393eb53dc091b8e73a5b63
workflow-type: tm+mt
source-wordcount: 421
ht-degree: 28%

---

# 发行说明：2026年5月 {#release-notes-may-26}

在下方，您会找到2026年5月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2026年5月22日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。 请查看每个功能旁的状态标记。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 电子邮件片段的条件内容</strong>： <i>与旧电子邮件编辑器对等</i>。 片段现在支持条件内容。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Picklist管理</strong>：您现在可以指定可以在Marketo Engage的字段中使用的值。
   </td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **社交功能弃用字段**：在2025年，Marketo Engage弃用了以下社交功能：

   * 投票
   * 社交按钮
   * 推荐优惠
   * 分享视频
   * 抽奖活动

今年早些时候，剩下的相关油田从Marketo被移除。 不久，引用某些与社交相关的潜在客户字段的API请求返回“字段未找到”错误，导致中断。 在受影响的字段再次可用后，服务已恢复，因此为防止进一步中断，Marketo已将Social字段与Social功能永久性分离（因此，将在您的Marketo帐户中提供）。 建议用户审查引用Marketo Social相关字段的API查询和集成，并确定这些字段是否仍为持续业务流程所必需。

* **Rest API &#39;access_token&#39;参数弃用**：用于验证Marketo REST API调用的`access_token`查询参数已被弃用，并将在2026年7月31日之后不可用。 所有新的和现有的集成都应使用 &#39;Authorization&#39; 请求头对 REST API 调用进行身份验证，[具体说明请参见此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API弃用**：对Marketo SOAP API的支持将于2026年7月31日终止。 使用 SOAP API 功能的服务应迁移至 [REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

* **Get Lead活动和Get Lead更改的静态列表大小限制**：从2026年9月30日开始，如果目标静态列表包含10,000个或更多潜在客户，则对Get Lead活动和包含`listId`参数的Get Lead Changes端点的调用将返回1003错误代码。 有关详细信息，请参阅[迁移指南](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}。

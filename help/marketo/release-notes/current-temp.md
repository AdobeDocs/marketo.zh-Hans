---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
hide: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
TQID: https://experienceleague.adobe.com/RZsCx9HAyJuDLO46WfshT30be-rMMDZjnygvU32NGfk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: df650f93bedc7202ad82f8f725616cd25e4a99ef
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 18%
---
# 发行说明：2026年9月 {#release-notes-sep-26}

在下方，您会找到2026年9月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2026年9月25日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。 请查看每个功能旁边的状态。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>Marketo Engage新UI</strong>： Marketo Engage界面具有更新的外观，包括更新的菜单、图标和布局，可提供更清晰、更现代的体验。 此为仅可视更新，任何现有功能或工作流都不会受到影响。 <i>经典UI的选择功能将在2027年1月版中提供</i>。
</td>
   <td>在9月底之前正式发布</td>
   <td><i>不适用</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>导入时选择分区</strong>：在启用了工作区和分区的环境中导入人员记录时，现在可以从本地工作区的分区列表中进行选择。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>CRM同步上的Instant Alert </strong>：订阅了CRM通知的用户将在其本机CRM同步的“已启用”状态更改时收到即时通知，从而使管理员能够更清楚地了解其CRM同步状态。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>自助流程步骤 — 回调超时时间增加</strong>：自助流程步骤的回调超时时间从1小时增加到4小时。 您无需执行任何操作。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **自定义活动属性的API名称限制**：通过API或UI创建的自定义活动属性的API名称现在只能包含字母数字字符和下划线，并且必须以字母数字字符开头。

* **Get Lead活动和Get Lead更改的静态列表大小限制**：从2026年9月30日开始，如果目标列表包含10,000个或更多潜在客户，对包含`listId`参数的Get Lead活动或Get Lead Changes端点的调用将失败，并显示1003错误代码（指示目标静态列表包含太多记录）。 请参阅[迁移指南](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}以获取更多信息。

* **REST API &#39;access_token&#39;参数弃用**：从2026年8月31日起，已弃用用于验证Marketo REST API调用的`access_token`查询参数。 所有新的和现有的集成都应使用 &#39;Authorization&#39; 请求头对 REST API 调用进行身份验证，[具体说明请参见此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **REST API营销活动运行ID**：在某些情况下，有时在两对引号（例如，`"campaignRunId": ""102938""`）之间返回活动的营销活动运行ID值格式不正确。<br/>从8月版本开始，此值将始终以正确的数字格式(`"campaignRunId": 102938`)返回。

* **弃用从Web获取图像**：为了符合现代安全和隐私最佳实践，从10月版本起，[从Web获取图像](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"}功能将被弃用。

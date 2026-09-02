---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f71e690b-4480-4b67-9ef5-88f42f9cdfdbid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: b40977d6745fdf31a48c6e08a7b070cd164408c8
workflow-type: tm+mt
source-wordcount: 477
ht-degree: 19%

---

# 发行说明：2026年8月 {#release-notes-aug-26}

在下方，您会找到2026年8月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2026年8月14日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。 请查看每个功能旁边的状态。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>Marketo Engage新UI</strong>： Marketo Engage界面具有更新的外观，包括更新的菜单、图标和布局，可提供更清晰、更现代的体验。 这只是可视更新，现有功能或工作流不会受到影响。
</td>
   <td>已在8月份分阶段推出</td>
   <td><i>不适用</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>在存档上禁用营销活动</strong>：存档文件夹现在会禁用并取消该文件夹树中的所有营销活动，从而防止意外执行已存档的智能营销活动。
</td>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
    <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 脚本生成器</strong>：脚本生成器是AI支持的助手，可帮助您更快地创建个性化脚本。
</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Marketo AI现在是Marketo Engage的协作者**： Marketo Engage的协作者提供了旨在自动执行耗时的营销功能的代理技能。 所有用户都可以使用新名称、相同功能。 [了解详情](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/coworker-for-marketo/overview){target="_blank"}

* **Rest API &#39;access_token&#39;参数弃用**：用于验证Marketo REST API调用的`access_token`查询参数已被弃用，并将在2026年8月31日之后不可用。 所有新的和现有的集成都应使用 &#39;Authorization&#39; 请求头对 REST API 调用进行身份验证，[具体说明请参见此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **REST API营销活动运行ID**：在某些情况下，有时在两对引号（例如，`"campaignRunId": ""102938""`）之间返回活动的营销活动运行ID值格式不正确。<br/>从8月版本开始，此值将始终以正确的数字格式(`"campaignRunId": 102938`)返回

* **Get Lead活动和Get Lead更改的静态列表大小限制**：从2026年9月30日开始，如果目标列表包含10,000个或更多潜在客户，并且1003错误代码指示目标静态列表包含过多记录，则对Get Lead活动或Get Lead Changes端点（包括`listId`参数）的调用将失败。 请参阅[迁移指南](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}以获取更多信息。

* **REST API合并潜在客户限制**：从2026年7月31日起，合并潜在客户API调用的leadIds参数中包含超过25个ID的调用会导致1080错误代码，并跳过该调用。 需要将超过25条记录合并为一个的工作应该被拆分为多个工作，以确保这些调用成功。

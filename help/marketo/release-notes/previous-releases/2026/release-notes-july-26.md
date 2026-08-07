---
description: 发行说明 — 2026年7月 — Marketo文档 — 产品文档
title: 发行说明 — 2026年7月
feature: Release Information
source-git-commit: ebd911b99e1c4c8f8a76db3a14235ee0d4ee0485
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 20%

---

# 发行说明： 2026年7月 {#release-notes-july-26}

在下方，您会找到2026年7月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2026年7月10日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。 请查看每个功能旁边的状态。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>Marketo AI技能 — 产品知识</strong>：产品知识可让您按需访问Marketo专业知识，而无需离开平台。 使用简单的语言提问，Marketo人工智能会利用Adobe的官方文档提供答案。
</td>
   <td>开放Beta版</td>
   <td><a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/marketo-ai/skills/product-knowledge" target="_blank">产品知识</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Marketo AI技能 — 调查潜在客户</strong>：了解为什么特定人员/潜在客户未达到里程碑（如MQL、计划资格或营销活动），并简单解释所发生的情况。
</td>
   <td>开放Beta版</td>
   <td><a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">调查潜在客户</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer - AI助手上下文菜单</strong>：现在可以从上下文菜单（黑色栏）访问Email Designer的AI助手功能。 例如，当您选择文本内容时，AI助手图标会出现在上下文菜单中，允许您从该处执行快速操作。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **Rest API &#39;access_token&#39;参数弃用**：用于验证Marketo REST API调用的`access_token`查询参数已被弃用，并将在2026年8月31日之后不可用。 所有新的和现有的集成都应使用 &#39;Authorization&#39; 请求头对 REST API 调用进行身份验证，[具体说明请参见此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。
* **REST API合并潜在客户限制**：从2026年7月31日开始，在合并潜在客户API调用的leadIds参数中包含超过25个ID的调用将导致1080错误代码，并且将跳过该调用。 需要将超过25条记录合并为一个的工作应该被拆分为多个工作，以确保这些调用成功。
* **SOAP API弃用**：对Marketo SOAP API的支持将于2026年7月31日终止。 使用 SOAP API 功能的服务应迁移至 [REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。
* **Get Lead活动和Get Lead更改的静态列表大小限制**：从2026年9月30日开始，如果目标静态列表包含10,000个或更多潜在客户，则对Get Lead活动和包含`listId`参数的Get Lead Changes端点的调用将返回1003错误代码。 有关详细信息，请参阅[迁移指南](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"}。

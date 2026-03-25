---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 70939d387dcfe6064e179e4e7e91b16c6baa7b8b
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 25%

---

# 发行说明：2026 年 3 月 {#release-notes-mar-26}

在下方，您会找到2026年3月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2026年3月27日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。请查看每个功能旁的状态标记。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>向Designer发送电子邮件 — 管理品牌（测试版）</strong>：根据您组织/品牌的特定撰稿准则生成电子邮件内容。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer - Brand Quality Checker</strong>：评估一般内容质量，以识别可读性、内容一致性和有效性方面的潜在问题，而不依赖于您的品牌指南。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer - Outlook渲染修复</strong>：此更新修复了渲染问题，尤其是在MS Outlook中。 “专家模式”允许您进行细微的HTML/CSS编辑，或向电子邮件添加脚本标记（最佳实践是不对电子邮件的HTML进行任何其他更改，以使可视化元素保持原样）。
   </td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>向Designer发送电子邮件 — 快速操作</strong>： <i>与旧电子邮件编辑器对等</i>。 快速操作现在可用于所有电子邮件Designer资源（电子邮件、电子邮件模板、片段）。 支持的快速操作包括：复制、删除、移动、创建/编辑草稿。
   </td>
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
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>推送通知</strong>：在推送通知消息中配置的重定向URL现在支持Marketo Engage令牌（仅适用于<i>启动应用程序URL</i>）。
   </td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **SEO功能弃用**：在2026年3月31日星期二，Marketo Engage将弃用搜索引擎优化功能(SEO)。 如果您未主动使用SEO，则无需执行任何操作。 如果您最近使用了SEO，则可以选择导出数据。 [了解详情](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617?profile.language=zh-Hans){target="_blank"}。

* **REST API合并潜在客户限制**：从2026年3月31日开始，在合并潜在客户API调用的leadIds参数中包含超过25个ID的调用将导致1080错误代码，并且将跳过该调用。 需要将超过25条记录合并为一个的工作应该被拆分为多个工作，以确保这些调用成功。

* **Rest API &#39;access_token&#39;参数弃用**：用于验证Marketo REST API调用的`access_token`查询参数已被弃用，并将在2026年7月31日之后不可用。 所有新的和现有的集成都应使用 &#39;Authorization&#39; 请求头对 REST API 调用进行身份验证，[具体说明请参见此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API弃用**：对Marketo SOAP API的支持将于2026年7月31日终止。 使用 SOAP API 功能的服务应迁移至 [REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

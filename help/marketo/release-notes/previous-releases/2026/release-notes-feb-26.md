---
description: 发行说明 — 2026年2月 — Marketo文档 — 产品文档
title: 发行说明 - 2026 年 2 月
feature: Release Information
exl-id: 679d2fca-99ba-4321-ad0d-a297b7f193fc
source-git-commit: 70939d387dcfe6064e179e4e7e91b16c6baa7b8b
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 24%

---

# 发行说明：2026 年 2 月 {#release-notes-feb-26}

在下方，您会找到2026年2月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2026年2月20日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。请查看每个功能旁的状态标记。

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>电子邮件Designer — 文件夹操作</strong>：与旧电子邮件编辑器对等。
   <ul>
   <li>为电子邮件Designer资源共享和存档文件夹操作。</li>
   <li>跨工作区共享文件夹，右键单击文件夹以创建新资产，通过拖放操作移动资产。</li>
   </ul>
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
   <td><strong>向Designer发送电子邮件 — API</strong>：您现在可以使用Designer电子邮件的API调用。</td>
   <td>已发布</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/asset#">Marketo资产API</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>电子邮件Designer - AI助手图像生成</strong>：现在，除了Firefly之外，您还可以使用Nano Banana模型通过AI助手生成电子邮件内容的图像。</td>
   <td>已发布</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-designer/ai-assistant#create-content-for-a-specific-section">为电子邮件的特定部分创建内容</a></td>
  </tr>
  </tbody>
</table>
<br/>

## 公告 {#announcements}

* **SEO功能弃用**：在2026年3月31日星期二，Marketo Engage将弃用搜索引擎优化功能(SEO)。 如果您未主动使用SEO，则无需执行任何操作。 如果您最近使用了SEO，则可以选择导出数据。 [了解详情](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617){target="_blank"}。

* **REST API合并潜在客户限制**：从2026年3月31日开始，在合并潜在客户API调用的leadIds参数中包含超过25个ID的调用将导致1080错误代码，并且将跳过该调用。 需要将超过25条记录合并为一个的工作应该被拆分为多个工作，以确保这些调用成功。

* **Rest API &#39;access_token&#39;参数弃用**：用于验证Marketo REST API调用的`access_token`查询参数已被弃用，并将在2026年7月31日之后不可用。 所有新的和现有的集成都应使用 &#39;Authorization&#39; 请求头对 REST API 调用进行身份验证，[具体说明请参见此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}。

* **SOAP API弃用**：对Marketo SOAP API的支持将于2026年7月31日终止。 使用 SOAP API 功能的服务应迁移至 [REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

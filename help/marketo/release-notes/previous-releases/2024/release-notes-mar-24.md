---
description: 发行说明 — 2024年3月 — Marketo文档 — 产品文档
title: 发行说明 — 2024年3月
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: fd92f5307880019f54bb2f1778093c110a53ed2c
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# 发行说明： 2024年3月 {#release-notes-mar-24}

在下方，您会找到2024年3月版本中包含的所有功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![星形](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

## 标准发行周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，并将于以下日期开始发行 **2024年3月8日**，在接下来的几周内分阶段推出剩余的功能。 发行功能和日期可能会发生更改。 请检查每个功能旁边的状态信息。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr> 
   <td><strong>高级对话流逻辑</strong>：添加其他字段以供在单个选项中进行评估，以进行对话流跟进。</td> 
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Marketo EngageForms的对话流设置</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>重新排序对话流逻辑</strong>：在Marketo EngageForms中，您现在可以重新排序对话流程选项，而不必删除并重新添加。</td> 
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Marketo EngageForms的对话流设置</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>API活动元数据</strong>：Web和电子邮件活动现在包含用户代理、平台和设备等元数据，这有助于通过Marketo REST API提供有关这些活动的一致见解。</td> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **获取项目成员API修复**：最近进行了更改以更正的行为 [获取计划成员](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Program_Members/getProgramMembersUsingGET){target="_blank"} 端点。 以前，在使用 `updatedAt` 筛选器类型要指定日期范围，该范围内更新的计划成员资格记录可能未包含在响应中。 此外，指定日期范围之外更新的项目成员资格记录可能会错误地包含在响应中。 这两个问题均已得到解决。

* **弃用帐户分析浏览器插件**：Adobe正在删除Target帐户管理 [帐户分析浏览器插件](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} from the Chrome Web Store on April 8, 2024. Existing users: you can continue to use the plug-in until you migrate your Marketo Engage instance to Adobe Identity and Admin Console. This change **will not impact** any other TAM features/data within Marketo Engage or the Chrome and Outlook email plug-ins that work with Sales Insight. [Learn more](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.

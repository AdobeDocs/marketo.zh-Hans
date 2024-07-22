---
description: 发行说明 — 2024年3月 — Marketo文档 — 产品文档
title: 发行说明 — 2024年3月
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# 发行说明： 2024年3月 {#release-notes-mar-24}

在下方，您会找到2024年3月版本中包含的所有功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号（![星号](assets/yellow-star.png)）表示的功能是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

## 标准发行周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2024年3月8日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 发行功能和日期可能会发生更改。 请检查每个功能旁边的状态信息。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr> 
   <td><strong>高级会话流逻辑</strong>：为会话流跟进添加用于评估的附加字段。</td> 
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
   <td><strong>重新排序对话流逻辑</strong>：在Marketo EngageForms中，您现在可以重新排序对话流选择，而不必删除并重新添加。</td> 
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Marketo EngageForms的对话流设置</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>API活动元数据</strong>： 
   Web活动和电子邮件活动现在包含用户代理、平台和设备等元数据，这有助于通过Marketo REST API提供对这些活动的一致见解。</td> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **获取程序成员API修复**：最近进行了更改，以更正[获取程序成员](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"}终结点的行为。 以前，当使用`updatedAt`筛选器类型指定日期范围时，在该范围内更新的项目成员资格记录可能未包含在响应中。 此外，指定日期范围之外更新的项目成员资格记录可能会错误地包含在响应中。 这两个问题均已得到解决。

* **帐户分析浏览器插件弃用**：Adobe将于2024年4月8日从Chrome网上应用商店中删除Target帐户管理[帐户分析浏览器插件](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"}。 现有用户：您可以继续使用插件，直到将Marketo Engage实例迁移到Adobe身份和Admin Console为止。 此更改&#x200B;**不会影响Marketo Engage或Chrome和Outlook电子邮件插件中与Sales Insight配合使用的任何其他TAM功能/数据**。 [了解更多](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}。

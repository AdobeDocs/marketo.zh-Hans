---
description: 发行说明 — 2025年4月 — Marketo文档 — 产品文档
title: 发行说明 - 2025 年 4 月
feature: Release Information
exl-id: 94010780-41aa-4212-a1d4-1b78806bd728
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 3%

---

# 发行说明：2025年4月 {#release-notes-apr-25}

在下方，您会找到2025年4月版本中包含的所有功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

可以在此处[找到特定于Adobe Dynamic Chat ](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}的发行说明。

>[!AVAILABILITY]
>
>以星号（![星号](assets/yellow-star.png)）表示的功能是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

## 标准发行周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2025年4月25日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 发行功能和日期可能会发生更改。 请检查每个功能旁边的状态信息。

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
  <tr>
   <td><strong>安全套接字层(SSL)自助服务</strong>： SSL加密允许您使Marketo Engage实例的登录页安全。 启用此功能过去需要Adobe支持团队的帮助。 Marketo用户现在可以自行启用该功能，从而节省宝贵的时间。</td>
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-ssl-to-your-landing-pages.md">将SSL添加到登陆页面</a></td>
  </tr>
 </tbody>
</table>
<br/>

## 公告 {#announcements}

* **新Analytics功能 — 公共Beta**：[高级BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"}(以前称为Revenue Explorer和Advanced Report Builder)在4月中旬开始向所有当前Revenue Cycle Explorer用户推出。 此新工具提供了有关Marketo Engage数据的灵活报表和可视化界面，提供了有关进度、性能等内容的精细详细信息。 它具有更丰富的交互性和可视化功能、更快的性能以及更顺畅和直观的用户体验。

要访问此功能，您必须已购买高级BI Analytics加载项。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

* **Rest API &#39;access_token&#39;参数弃用**：用于验证Marketo REST API调用的`access_token`查询参数已被弃用，并将在2025年10月31日之后不可用。 所有新的和现有的集成都应使用“授权”标头[来验证REST API调用，如此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication){target="_blank"}所述。

* **SOAP API弃用**：对Marketo SOAP API的支持将于2025年10月31日终止。 使用SOAP API功能的服务应迁移到[REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

* **弃用社交功能**：在2024年7月31日星期三，Marketo Engage开始弃用产品中的以下社交功能：

   * 投票
   * 社交按钮
   * 推荐优惠
   * 分享视频
   * 抽奖活动

截至那时，用户无法在Marketo Engage中创建、克隆或嵌入任何这些Social功能。 现有社会资产继续运作至2025年1月31日。 2025年2月1日，Social Assets停止运行。 需要删除登陆页面中嵌入的任何社交功能。 [了解详情](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

---
description: 发行说明 — 2024年10月 — Marketo文档 — 产品文档
title: 发行说明 - 2024 年 10 月
feature: Release Information
exl-id: 2e28ae7f-51de-4510-b3e8-79a989f0daf5
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 2%

---

# 发行说明：2024年10月 {#release-notes-oct-24}

在下方，您会找到2024年10月版本中包含的所有功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

可以在此处[找到特定于Adobe Dynamic Chat ](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}的发行说明。

>[!AVAILABILITY]
>
>以星号（![星号](assets/yellow-star.png)）表示的功能是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

## 标准发行周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2024年10月4日开始发行**，并在接下来的几周内分阶段推出剩余功能。 发行功能和日期可能会发生更改。 请检查每个功能旁边的状态信息。

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
    <tr>
   <td><strong>交互式网络研讨会的令牌化</strong>：您现在可以使用令牌在电子邮件和登陆页面中推广交互式网络研讨会，而无需手动添加网络研讨会详细信息。</td>
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/promoting-an-interactive-webinar.md#interactive-webinars-tokens" target="_blank">推广交互式网络研讨会</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr>
   <td><strong>智能列表“设置为影响”计数</strong>：查看编辑Smart Campaign的资格规则时受影响的人员数量。</td>
   <td>已发货</td>
   <td>不适用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr>
   <td>导航边栏中的<strong>我的帐户按钮</strong>：对于已迁移到Adobe Identity Management System的用户，左侧导航边栏中新增的“我的帐户”按钮允许您配置时区并访问订阅详细信息。</td>
   <td>已发货</td>
   <td>不适用</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>电子邮件性能报表增强功能</strong>：对电子邮件报表量度和活动跟踪进行了多项改进，提供了更多见解并提高了准确性。
   <ul>
   <li>从电子邮件性能量度中过滤删除和合并的人员</li>
   <li>电子邮件在等待响应活动三天后现在被分类为<i>已中止</i></li>
   <li>每个智能营销活动将电子邮件打开数计为单独唯一打开</li>
   </td>
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md" target="_blank">电子邮件性能报表</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Salesforce同步积压量度</strong>：监视同步吞吐量和积压趋势，以计划和计划CRM更新以获得最佳同步体验。
   </td>
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-backlog-metrics.md" target="_blank">Salesforce同步积压量度</a></td>
  </tr>
 </tbody>
</table>
<br/>

## 公告 {#announcements}

* **批量提取API更新**：我们修复了批量提取API中涉及columnHeaderNames选项的问题，该选项允许您在导出的文件中指定自定义列标题名称。 以前，包含非ASCII字符的列标题名称可能会损坏。

* **Rest API access_token参数弃用**：用于验证Marketo REST API调用的“access_token”查询参数已被弃用，并将在2025年10月31日之后不可用。 所有新集成和现有集成都应使用“授权”标头[对REST API调用进行身份验证，如此处](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/authentication#using-an-access-token)所述。

* **QR代码弃用**： 2024年10月4日，将弃用推送通知和应用程序内消息传送资产中使用的该QR代码功能。 这包括为新的测试设备使用二维码，以及创建具有二维码的新资产。 弃用使用率较低的功能后，我们可以重新分配其资源用于Marketo Engage的整体维护。

* **Munchkin更改**

   * **新版本**：从2024年9月17日起，[Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164将开始推广到&#x200B;**管理员** > **Treasure Chest**&#x200B;中启用了“Munchkin Beta”设置的Marketo Engage实例。 该应用程序计划于10月29日开始推广到所有其他实例。 此版本会更新Munchkin Cookie的创建。 功能没有变化。

   * **已移除URL中的字符**：Munchkin JS创建的“访问网页”和“点击链接”活动现在将从所有URL字段中移除非URL编码的控制字符。 此更改旨在防止与这些类型的字符传播到不支持这些字符并在Marketo Engage中无效使用的系统相关的错误。

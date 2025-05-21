---
description: 发行说明 — 2025年1月 — Marketo文档 — 产品文档
title: 发行说明 - 2025 年 1 月
feature: Release Information
exl-id: fd816b9c-9e06-4292-87d6-9fa991c4681f
source-git-commit: 701155a5beccf3725fe26d2bc75c541c989d4af4
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 2%

---

# 发行说明：2025年1月 {#release-notes-jan-25}

在下方，您会找到2025年1月版本中包含的所有功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

可以在此处](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}找到特定于Adobe Dynamic Chat [的发行说明。

>[!AVAILABILITY]
>
>以星号（![星号](assets/yellow-star.png)）表示的功能是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

## 标准发行周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2025年1月17日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 发行功能和日期可能会发生更改。 请检查每个功能旁边的状态信息。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
    <tr> 
   <td><strong>新电子邮件Designer</strong>：在Marketo Engage中使用新的本机电子邮件Designer创建现代而高效的电子邮件。 访问其中一个预设计的现成电子邮件模板，或轻松创建您自己的模板。 使用动态内容并从Adobe Experience Manager云服务访问图像。 使用Content Accelerator Gen-AI功能大规模创建创新和性能优异的电子邮件。
   <p><img src="assets/note-icon.png" alt="注释图标"> 注意：要访问新的电子邮件设计器，必须将您的Marketo Engage订阅迁移到<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview">Adobe Identity Management System (IMS)</a>。 如果尚未收到请求并想请求加急，请联系Adobe客户团队（您的客户经理）或<a href="https://nation.marketo.com/t5/support/ct-p/Support">Marketo支持</a>。 要访问Content Accelerator Gen-AI功能，请联系Adobe客户团队。</td>
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">通过电子邮件发送Designer概述</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>在交互式网络研讨会中取消注册注册者</strong>：现在，如果您由于任何原因不想在网络研讨会中注册者，则可以取消注册。 该工作流会从Marketo事件项目和Adobe Connect中删除注册者。</td> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>存档时禁用营销活动</strong>：在存档时禁用活动触发器营销活动并取消文件夹中任何计划的营销活动批量运行。 由于对包含活动营销活动（激活触发器营销活动和计划批量营销活动）的存档文件夹进行了额外的权限检查，因此此功能在此版本中默认处于禁用状态，可以通过导航到Marketo Engage订阅中的<b>管理员</b> &gt; <b>Treasure Chest</b>来启用此功能。</td> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **弃用社交功能**：在2024年7月31日星期三，Marketo Engage开始弃用产品中的以下社交功能：

   * 投票
   * 社交按钮
   * 推荐优惠
   * 分享视频
   * 抽奖活动

截至那时，用户无法在Marketo Engage中创建、克隆或嵌入任何这些Social功能。 现有社会资产继续运作至2025年1月31日。 2025年2月1日，Social资产将停止运行。 需要删除嵌入到登陆页面中的社交功能。 [了解详情](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **获取计划成员API更新**：我们已增强[获取计划成员](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} API以支持检索计划成员标识符的功能。 这是通过向在API请求的字段参数中指定的字段列表添加ID来完成的。

* **Rest API &#39;access_token&#39;参数弃用**：用于验证Marketo REST API调用的`access_token`查询参数已被弃用，并将在2025年10月31日之后不可用。 所有新的和现有的集成都应使用“授权”标头[来验证REST API调用，如此处](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}所述。

* **SOAP API弃用**：对Marketo SOAP API的支持将于2025年10月31日终止。 使用SOAP API功能的服务应迁移到[REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}。

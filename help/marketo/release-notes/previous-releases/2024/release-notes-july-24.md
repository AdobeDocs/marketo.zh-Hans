---
description: 发行说明 — 2024年7月 — Marketo文档 — 产品文档
title: 发行说明 - 2024 年 7 月
feature: Release Information
source-git-commit: 9087709e0572687b80022b73a1fde0dca8dc1a7e
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 3%

---

# 发行说明： 2024年7月 {#release-notes-july-24}

在下方，您会找到2024年7月版本中包含的所有功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

可以在此处[&#128279;](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}找到专门用于Adobe Dynamic Chat的发行说明。

>[!AVAILABILITY]
>
>以星号（![星号](assets/yellow-star.png)）表示的功能是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

## 标准发行周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2024年7月26日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 发行功能和日期可能会发生更改。 请检查每个功能旁边的状态信息。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
     <tr> 
   <td><strong>交互式网络研讨会的参与仪表板</strong>：获取网络研讨会性能汇总视图以及网络研讨会期间每位与会者的参与情况综合视图，以便您通过Marketo Engage编排工具决定要定位哪些潜在客户。</td> 
    <td>已发货</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/engagement-dashboard.md" target="_blank">参与仪表板</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>交互式网络研讨会的文件室管理</strong>：访问已创建的各个文件室（并根据需要进行修改），以及访问内容和录制（如果需要，请清除这些文件室以优化存储）。</td> 
    <td>已发货</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/room-management.md" target="_blank">房间管理</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>交互式网络研讨会的网络研讨会自定义</strong>：通过使用公共会议室界面、中间屏幕（如与会者入门屏幕背景）以及自定义视频背景，提供组织批准的统一品牌体验，以便网络研讨会策略可以更轻松地与品牌策略保持一致。</td> 
    <td>已发货</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/customization.md" target="_blank">交互式网络研讨会自定义</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Marketo REST API更改</strong>：我们即将对<a href="https://developers.marketo.com/rest-api/user-management/">用户管理API</a>进行细微更改。 <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">浏览用户</a>和<a href="https://developers.marketo.com/rest-api/user-management/#delete_user">删除用户</a>端点现在都支持<a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">目标帐户管理</a>用户。</td> 
   <td>已发货</td>
   <td>不适用</td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **新的开发人员文档网站**：作为我们努力改进Marketo Engage用户体验的一部分，我们将在2024年7月将所有开发人员文档迁移到Adobe Experience League和Adobe Developer网站。 [了解详情](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **弃用社交功能**：2024年7月31日星期三，Marketo Engage将开始弃用产品中的以下社交功能：

   * 投票
   * 社交按钮
   * 推荐优惠
   * 分享视频
   * 抽奖活动

用户将无法再在Marketo Engage中创建、克隆或嵌入任何这些Social功能。 现有社会资产将继续运作到2025年1月31日。 [了解详情](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **查询参数弃用中的访问令牌**：在未来版本中，将移除对Marketo EngageREST API调用的查询参数中使用访问令牌的身份验证的支持（具体日期待定）。 现有集成应迁移到此处[&#128279;](https://developers.marketo.com/rest-api/authentication/){target="_blank"}描述的授权标头的使用情况。 新开发应仅使用Authorization标头进行Marketo Engage身份验证。

* **需要对LinkedIn进行重新身份验证**： LinkedIn正在升级其Marketo EngageLinkedIn集成所使用的营销API。 在2024年7月26日至12月15日之间，这些更改将需要重新验证您&#x200B;**管理员** > **LaunchPoint**&#x200B;菜单中的所有LinkedIn LaunchPoint服务，以避免服务中断。 您可以在此处找到有关Forms潜在客户如何完成此[的说明](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"}和[此处提供的有关匹配受众的说明](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}。 Lead Gen Form服务具有“LinkedIn Lead Gen”类型，而Matched Audience服务具有“LinkedIn Matched Audiences”类型。 有关详细信息，请访问[迁移常见问题解答](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}。

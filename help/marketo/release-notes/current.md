---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 10a77a09f5ca9ce57e7a357fe1b6736b7bdb95e3
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 1%

---

# 发行说明： 2024年7月 {#release-notes-july-24}

在下方，您会找到2024年6月版本中包含的所有功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

专门用于Adobe Dynamic Chat的发行说明 [可在此处找到](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>以星号(![星形](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

## 标准发行周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，并将于以下日期开始发行 **2024年7月26日**，在接下来的几周内分阶段推出剩余的功能。 发行功能和日期可能会发生更改。 请检查每个功能旁边的状态信息。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
     <tr> 
   <td><strong>交互式网络研讨会的参与仪表板</strong>：在网络研讨会期间获取每位与会者的汇总网络研讨会性能视图和参与情况的全面视图，以便您能够通过Marketo Engage编排工具确定目标销售线索。</td> 
    <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>交互式网络研讨会的会议室管理</strong>：访问已创建的各个文件室（并根据需要进行修改），以及访问内容和录制（并根据需要清除它们以优化存储）。</td> 
    <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>网络研讨会自定义交互式网络研讨会</strong>：通过使用公共会议室界面、中间屏幕（如与会者入门屏幕背景）以及自定义视频背景，提供组织批准的统一品牌体验，以便网络研讨会策略可以更轻松地与品牌策略保持一致。</td> 
    <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Marketo REST API更改</strong>：我们正在对 <a href="https://developers.marketo.com/rest-api/user-management/">用户管理API</a>. 两者都是 <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">浏览用户</a> 和 <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">删除用户</a> 现在支持端点 <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">目标帐户管理</a> 用户。</td> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **新建开发人员文档网站**：作为我们不断努力改进的Marketo Engage用户体验的一部分，我们将于2024年7月将所有开发人员文档迁移到Adobe Experience League和Adobe Developer网站。 [了解详情](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **查询参数中的访问令牌已弃用**：在将来的版本中，将移除对Marketo EngageREST API调用的查询参数中使用访问令牌进行身份验证的支持（具体日期待定）。 现有集成应迁移到授权标头的使用 [此处说明](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. 新开发应仅使用Authorization标头进行Marketo Engage身份验证。

* **linkedIn需要重新身份验证**：LinkedIn正在升级其由Marketo EngageLinkedIn集成使用的营销API。 这些更改将需要重新验证您网站上的所有LinkedIn LaunchPoint服务 **管理员** > **启动点** 2024年7月26日至12月15日之间的菜单，以避免服务中断。 您可以找到有关如何完成此操作的说明 [此处联系潜在客户Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} 和 [此处显示匹配的受众](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. Lead Gen Form服务具有“LinkedIn Lead Gen”类型，而Matched Audience服务具有“LinkedIn Matched Audiences”类型。 欲知更多信息，请参见 [迁移常见问题解答](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.

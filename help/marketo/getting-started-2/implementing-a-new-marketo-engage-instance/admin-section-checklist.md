---
description: 为您的新Marketo Engage实例设置“管理员”部分。
title: 新实例最佳实践 — 管理员部分核对清单
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: fa5b686aabd3aab2d9020758fde00ed06564c76c
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# 新实例最佳实践：管理员部分核对清单 {#new-instance-best-practices-admin-section-checklist}

作为新管理员，请应用以下清单来帮助指导您完成实施Marketo Engage。 与所有这些指南一样，您可以下载核对清单 [链接] 并跟踪您的进度。

## 角色 {#roles}

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>角色</td>
    <td><li>查看预建角色，并确认每个角色具有哪些权限/访问权限。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role" target="_blank">创建新角色</a> 或 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role" target="_blank">编辑角色</a> 根据贵组织的需求而定。</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">将用户分配给适当的角色</a>. 必须先将用户添加到Adobe Admin Console中的订阅，然后才能授予他们在角色中的角色。 请参阅的“用户”部分 <a href="/help/marketo/getting-started-2/initial-setup/user-setup.md">初始设置核对清单</a>.</li>
    <li>为用户分配角色后，查看每个角色的用户数。</li>
    <li>为每个API用户实施唯一的角色，以便轻松进行故障排除。</li></td>
  </tr>
  <tr>
    <td>文档</td>
    <td><li>为您的组织定义用户和角色。</li>
    <li>定义添加新用户/管理员的过程。</li></td>
  </tr>
  <tr>
    <td>沙盒（如果适用）</td>
    <td><li>查看以上类别中的 <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md">沙盒</a>.</li></td>
  </tr>
</tbody>
</table>

## 工作区和分区 {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>工作区和分区（如果适用）</td>
    <td><li>确定数量<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html" target="_blank"> 工作区</a> 和/或您的组织需要拥有的和/或分区 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html" target="_blank">每个工作区有多少用户具有访问权限。</a></li>
    <li>定义每个工作区和分区的主要用途。</li>
    <li>定义工作区和分区之间的关系。</li></td>
  </tr>
  <tr>
    <td>文档</td>
    <td><li>记录工作区的定义方式以及它与数据库分区的关系（例如，显示每个人相对于业务部门的全局工作区）。</li>
    <li>将新记录导入相应的分区。</li>
    <li>在CRM中定义将用户放入相应分区的值。</li></td>
  </tr>
</tbody>
</table>

## Smart Campaign设置 {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Smart Campaign设置</td>
    <td><li>添加 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html" target="_blank">Smart Campaign大小限制</a>，防止意外地通过电子邮件发送整个数据库。</li></td>
  </tr>
</tbody>
</table>

## 电子邮件设置 {#email-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>电子邮件默认值</td>
    <td><li>在品牌策略域下，选择您的域并添加电子邮件CNAME。 其格式应为： [EmailTrackingCNAME]。[CompanyDomain].com.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console" target="_blank">联系Marketo支持</a> 以通过SSL证书配置保护它。 完成此过程最多可能需要3个工作日。</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html" target="_blank">设置SPF和DKIM</a> 实现电子邮件可投放性。</li></td>
  </tr>
</tbody>
</table>

## 通信限制 {#communication-limits}

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>通信限制</td>
    <td><li>启动 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank">通信限制</a>.</li>
    <li>确定您的企业是否需要有关通信限制的策略。</li></td>
  </tr>
</tbody>
</table>

## 标记 {#tags}

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>渠道</td>
    <td><li>定义使用方法 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html" target="_blank">渠道</a>.</li></td>
  </tr>
  <tr>
    <td>标记</td>
    <td><li>定义使用方法 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html" target="_blank">标记</a>.</li></td>
  </tr>
  <tr>
    <td>日历（如果适用）</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html" target="_blank">问题营销日历名额</a> 给那些需要访问的人。</li>
    <li>设置 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank">日历</a>.</li></td>
  </tr>
</tbody>
</table>

## 数据库管理 {#database-management}

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>字段管理</td>
    <td><li>实施命名约定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">自定义字段</a> （例如，以“MKTO”开头）。</li>
    <li>选择您同步的字段。 同步字段越多，同步周期越慢。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">阻止更新字段</a> 您需要写入一次性（例如，原始商机来源、原始商机来源详细信息、首次联系UTM字段等）。</li></td>
  </tr>
  <tr>
    <td>自定义活动</td>
    <td><li>定义 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html">自定义活动</a> 特定于您的业务。</li></td>
  </tr>
  <tr>
    <td>自定义对象</td>
    <td><li>查看数量 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html">自定义对象</a> 你需要。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html">将这些自定义对象同步到您的CRM</a>.</li></td>
  </tr>
</tbody>
</table>

## 集成 {#integrations}

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM </td>
    <td><li>启动CRM同步。 根据贵公司使用的CRM，从以下内容中进行选择： <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html">Microsoft Dynamics</a>.</li>
    <li>确定访问CRM所需的访问权限类型。</li>
    <li>确定您的CRM管理员以进行疑难解答。</li></td>
  </tr>
  <tr>
    <td>Web服务</td>
    <td><li>确定可以进行的用户/应用程序 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html">API调用</a> 在您的实例中。</li>
    <li>审查将发起API调用的所有应用程序，并确定是否需要增加或减少API调用。</li></td>
  </tr>
  <tr>
    <td>启动点</td>
    <td><li>设置 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html">启动点</a> 服务您的业务。 每个LaunchPoint都应与唯一的API用户配对，以帮助进行故障排除。</li></td>
  </tr>
  <tr>
    <td>交互式网络研讨会（如果适用）</td>
    <td>注意：交互式网络研讨会仅提供给生产实例。
    <li>要创建交互式网络研讨会，内置网络研讨会功能， <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management">将用户添加到“用户”部分</a> 在交互式网络研讨会选项卡上。</li></td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat（如果适用）</td>
    <td><li>将用户分配到 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role">“访问Dynamic Chat”角色</a> 在Marketo Engage&gt;管理员&gt;用户和角色中。</li></td>
  </tr>
  <tr>
    <td>销售分析（如果适用）</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account">设置销售分析操作</a> “销售分析”&gt;“操作配置”中的。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions">将名额发给适当的用户</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html">配置API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html">自定义潜在客户得分</a>.</li></td>
  </tr>
  <tr>
    <td>Sales Connect （如果适用）</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance">邀请适当的Marketo Engage管理员加入Sales Connect实例</a>.</li>
    <li>完成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins">其他Sales Connect管理员设置</a> Sales Connect和Salesforce中的。</li></td>
  </tr>
  <tr>
    <td>Webhook（如果适用）</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html">创建任何所需的Webhook</a> 为了你的生意。</li>
    </td>
  </tr>
</tbody>
</table>

## 宝箱 {#treasure-chest}

<table>
<thead>
  <tr>
    <th style="width:20%">区域</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>宝箱 </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html">启用Treasure Chest</a> 以试用功能。</li>
    <li>确定要打开或关闭的功能。</li></td>
  </tr>
  <tr>
    <td>活动检查器 </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html">打开活动检查器</a> 一次查看您的所有Smart Campaigns。</li></td>
  </tr>
</tbody>
</table>

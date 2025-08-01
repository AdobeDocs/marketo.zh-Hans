---
description: 为您的新Marketo Engage实例设置“管理员”部分。
title: 新实例最佳实践 — 管理员部分核对清单
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 2%

---

# 新实例最佳实践：管理员部分核对清单 {#new-instance-best-practices-admin-section-checklist}

作为新管理员，请应用以下核对清单来帮助指导您完成实施过程。Marketo Engage新实例包括： 与所有这些指南一样，您也可以[下载核对清单](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)并跟踪您的进度。

## 角色 {#roles}

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>角色</td>
    <td><li>查看预建角色，并确认每个角色具有哪些权限/访问权限。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=zh-Hans#create-a-new-role" target="_blank">创建新角色</a>或<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=zh-Hans#edit-a-role" target="_blank">根据您组织的需求编辑角色</a>。</li>
    <li><a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">将用户分配给适当的角色</a>。 必须先将用户添加到Adobe Admin Console中的订阅，然后才能授予他们在“角色”中的角色。 请参阅<a href="/help/marketo/getting-started/initial-setup/user-setup.md">初始设置核对清单</a>中的“用户”部分。</li>
    <li>为用户分配角色后，查看每个角色的用户数。</li>
    <li>为每个API用户实施唯一的角色，以便轻松进行故障排除。</li></td>
  </tr>
  <tr>
    <td>沙盒（如果适用）</td>
    <td><li>查看您的<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">沙盒</a>的上述类别。</li></td>
  </tr>
</tbody>
</table>

## 工作区和分区 {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>工作区和分区（如果适用）</td>
    <td><li>确定您的组织需要具有<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html?lang=zh-Hans" target="_blank">个工作区</a>和/或分区的数量，以及<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html?lang=zh-Hans" target="_blank">每个工作区有多少用户有权访问。</a></li>
    <li>定义每个工作区和分区的主要用途。</li>
    <li>定义工作区和分区之间的关系。</li></td>
  </tr>
</tbody>
</table>

## Smart Campaign设置 {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Smart Campaign设置</td>
    <td><li>添加Smart Campaign大小<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html?lang=zh-Hans" target="_blank">的</a>限制，以防止意外通过电子邮件发送整个数据库。</li></td>
  </tr>
</tbody>
</table>

## 通信限制 {#communication-limits}

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>通信限制</td>
    <td><li>实施<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html?lang=zh-Hans" target="_blank">通信限制</a>。</li>
    <li>确定您的企业是否需要有关通信限制的策略。</li></td>
  </tr>
</tbody>
</table>

## 标记 {#tags}

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>渠道</td>
    <td><li>定义如何使用<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html?lang=zh-Hans" target="_blank">渠道</a>。</li></td>
  </tr>
  <tr>
    <td>标记</td>
    <td><li>定义如何使用<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html?lang=zh-Hans" target="_blank">标记</a>。</li></td>
  </tr>
  <tr>
    <td>日历<br>
    （如果适用）</td>
    <td><li>向需要访问的人发放<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html?lang=zh-Hans" target="_blank">营销日历名额</a>。</li>
    <li>设置<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html?lang=zh-Hans" target="_blank">日历</a>。</li></td>
  </tr>
</tbody>
</table>

## 数据库管理 {#database-management}

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>字段管理</td>
    <td><li>为<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html?lang=zh-Hans" target="_blank">自定义字段</a>实施命名约定（例如，以“MKTO”开头）。</li>
    <li>选择您同步的字段。 同步字段越多，同步周期越慢。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html?lang=zh-Hans" target="_blank">阻止对要写入一次的字段</a>的更新（例如，原始商机源、原始商机源详细信息、首次联系UTM字段等）。</li></td>
  </tr>
  <tr>
    <td>自定义活动</td>
    <td><li>定义特定于您的业务的<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html?lang=zh-Hans" target="_blank">自定义活动</a>。</li></td>
  </tr>
  <tr>
    <td>自定义对象</td>
    <td><li>查看您需要的<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html?lang=zh-Hans" target="_blank">自定义对象</a>的数量。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html?lang=zh-Hans" target="_blank">将这些自定义对象</a>同步到您的CRM。</li></td>
  </tr>
</tbody>
</table>

## 集成 {#integrations}

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM </td>
    <td><li>确定访问CRM所需的权限。</li>
    <li>确定您的CRM管理员以进行疑难解答。</li></td>
  </tr>
  <tr>
    <td>Web服务</td>
    <td><li>确定可在您的实例中进行<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html?lang=zh-Hans" target="_blank">API调用</a>的用户/应用。</li>
    <li>审查将发起API调用的所有应用程序，并确定是否需要增加或减少API调用。</li></td>
  </tr>
  <tr>
    <td>启动点</td>
    <td><li>为您的企业设置<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html?lang=zh-Hans" target="_blank">LaunchPoint</a>服务。 每个LaunchPoint都应与唯一的API用户配对，以帮助进行故障排除。</li></td>
  </tr>
  <tr>
    <td>交互式网络研讨会（如果适用）</td>
    <td><li>若要创建交互式网络研讨会(Marketo Engage内置网络研讨会功能)，请<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management" target="_blank">将用户添加到“交互式网络研讨会”选项卡上的“用户”部分</a>。</li>
    <p><img src="assets/note-icon.png" alt="注释图标"> 注意：交互式网络研讨会仅提供给生产实例。</td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat（如果适用）</td>
    <td><li>在“Marketo Engage”&gt;“管理员”&gt;“用户和角色”中，将用户分配给<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role" target="_blank">“访问Dynamic Chat的角色</a>”。</li></td>
  </tr>
  <tr>
    <td>销售Insight（如果适用）</td>
    <td><li><a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account" target="_blank">在Sales Insight &gt;操作配置中设置Sales Insight操作</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html?lang=zh-Hans#invite-individual-users-to-msi-actions" target="_blank">将名额</a>发给适当的用户。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html?lang=zh-Hans" target="_blank">配置API</a>。</li>
    <li>自定义<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html?lang=zh-Hans" target="_blank">潜在客户得分</a>。</li></td>
  </tr>
  <tr>
    <td>Sales Connect （如果适用）</td>
    <td><li>邀请适当的Marketo Engage管理员加入<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance" target="_blank">Sales Connect实例</a>。</li>
    <li>完成Sales Connect和Salesforce中的<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins" target="_blank">其他Sales Connect管理员设置</a>。</li></td>
  </tr>
  <tr>
    <td>Webhook（如果适用）</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html?lang=zh-Hans" target="_blank">为您的企业创建任何必需的Webhook</a>。</li>
    </td>
  </tr>
</tbody>
</table>

## 宝箱 {#treasure-chest}

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>宝箱 </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html?lang=zh-Hans" target="_blank">启用Treasure Chest</a>以试用功能。</li>
    <li>确定要打开或关闭的功能。</li></td>
  </tr>
  <tr>
    <td>活动检查器 </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html?lang=zh-Hans" target="_blank">打开营销活动检查器</a>以在一个位置查看您的所有Smart营销活动。</li></td>
  </tr>
</tbody>
</table>

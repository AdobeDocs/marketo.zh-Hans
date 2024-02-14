---
description: 新区域 — Marketo文档 — 产品文档
title: 新建区域
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: c0f0134972138eb4fa3498028a4acf5233dbe2fe
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 2%

---

# 新区域：管理员核对清单 {#new-area-admin-checklist}

正在打开模糊

## 角色 {#roles}

<table>
<thead>
  <tr>
    <th>区域 </th>
    <th>操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>角色 </td>
    <td><li>查看预建角色，并确认每个角色具有哪些权限/访问权限。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">创建新角色</a> 或 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">编辑角色</a> 基于贵组织的需求和用户登录频率。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">将用户分配给适当的角色</a>.</li>
    <li>为用户分配角色后，查看每个角色的用户数。</li>  <li>为每个API用户实施唯一的角色，以便轻松进行故障排除。</li></td>
  </tr>
  <tr>
    <td>文档 </td>
    <td>为您的组织定义用户和角色。 <br>定义添加新用户/管理员的过程。 </td>
  </tr>
  <tr>
    <td>沙盒（如果适用） </td>
    <td>如果您有沙盒，请查看上面的类别。 </td>
  </tr>
</tbody>
</table>

## 工作区和分区 {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>区域</th>
    <th>操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>工作区和分区 </td>
    <td><li>确定数量<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> 工作区</a> 和/或您的组织需要拥有的和/或分区 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">每个工作区有多少用户具有访问权限。</a></li>
    <li>定义每个工作区和分区的主要用途。</li>
    <li>定义工作区和分区之间的关系。</li></td>
  </tr>
  <tr>
    <td>文档 </td>
    <td><li>记录工作区的定义方式以及它与数据库分区（即，可看到每个人而非业务部门的全局工作区）的关系。</li>
    <li>将新记录导入相应的分区。</li>
    <li>在CRM中定义将用户放置到相应分区的值。</li></td>
  </tr>
</tbody>
</table>

## Smart Campaign设置 {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>区域</th>
    <th>操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Smart Campaign设置 </td>
    <td><li>添加 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">Smart Campaign大小限制</a>，防止意外地通过电子邮件发送整个数据库。</li>
    <li>为智能营销活动启用人员限制</li></td>
  </tr>
</tbody>
</table>

## 电子邮件设置 {#email-settings}

<table>
<thead>
  <tr>
    <th>区域</th>
    <th>操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>电子邮件默认值</td>
    <td><li>在品牌策略域下，选择您的域并添加电子邮件CNAME。 其格式应为： [EmailTrackingCNAME]。[CompanyDomain].com.</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">设置SPF和DKIM</a> 实现电子邮件可投放性。</li></td>
  </tr>
</tbody>
</table>

## 通信限制 {#communication-limits}

<table>
<thead>
  <tr>
    <th>区域</th>
    <th>操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>通信限制</td>
    <td><li>地标 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">通信限制</a>.</li>
    <li>确定您的企业是否需要有关通信限制的策略。</li></td>
  </tr>
</tbody>
</table>

## 标记 {tags}

<table>
<thead>
  <tr>
    <th>区域</th>
    <th>操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>渠道</td>
    <td><li>定义使用方法 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">渠道</a>.</li></td>
  </tr>
  <tr>
    <td>标记 </td>
    <td><li>定义使用方法 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">标记</a>.</li></td>
  </tr>
  <tr>
    <td>日历（如果适用） </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">问题营销日历名额</a> 给那些需要访问的人。</li> 
    <li>设置 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">日历</a>.</li></td>
  </tr>
</tbody>
</table>

## 数据库管理 {#database-management}

<table>
<thead>
  <tr>
    <th>区域</th>
    <th>操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>字段管理</td>
    <td><li>实施命名约定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank" rel="noopener noreferrer">自定义字段。</a> 例如，以“MKTO”开头。</li>
    <li>选择您同步的字段。 您同步的字段越多，同步周期就越慢。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank" rel="noopener noreferrer">阻止更新字段</a> 您需要写入一次（即，原始商机来源、原始商机来源详细信息、首次联系UTM字段等）。</li></td>
  </tr>
  <tr>
    <td>自定义活动 </td>
    <td><li>定义 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank" rel="noopener noreferrer">自定义活动</a> 特定于您的业务。</li></td>
  </tr>
  <tr>
    <td>自定义对象 </td>
    <td><li>查看数量 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank" rel="noopener noreferrer">自定义对象</a> 你需要。</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank" rel="noopener noreferrer">将这些自定义对象同步到您的CRM</a>.</li></td>
  </tr>
</tbody>
</table>

## 集成 {#integrations}

<table>
<thead>
  <tr>
    <th>区域</th>
    <th>操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>启动CRM同步。 根据贵公司使用的CRM，从以下内容中进行选择： <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank" rel="noopener noreferrer">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank" rel="noopener noreferrer">Microsoft Dynamics</a>.</li>
    <li>确定访问CRM所需的访问权限类型。</li>
    <li>确定您的CRM管理员以进行疑难解答。</li></td>
  </tr>
  <tr>
    <td>销售分析（如果适用）</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank" rel="noopener noreferrer">设置销售分析。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank" rel="noopener noreferrer">将名额发给适当的用户。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank" rel="noopener noreferrer">配置API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank" rel="noopener noreferrer">自定义潜在客户得分。</a></li></td>
  </tr>
</tbody>
</table>

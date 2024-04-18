---
description: 新区域 — Marketo文档 — 产品文档
title: 新建区域
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 14ccfe39059b9c900a5e5e00b082146bb500d79d
workflow-type: tm+mt
source-wordcount: '1113'
ht-degree: 1%

---

# 新区域：管理员核对清单 {#new-area-admin-checklist}

介绍文本。

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
    <td><li>查看预建角色，并确认每个角色具有哪些权限/访问权限。<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role" target="_blank">创建新角色</a> 或 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role" target="_blank">编辑角色</a> 基于贵组织的需求和用户登录频率。<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html%22%20/l%20%22assign-roles-to-a-user" target="_blank">将用户分配给适当的角色</a>. 必须先将用户添加到Adobe Admin Console中的订阅，然后才能授予他们在角色中的角色。 请参阅“初始设置”核对清单[LINK]中的“用户”一节。 <br>为用户分配角色后，查看每个角色的用户数。<br>为每个API用户实施唯一的角色，以便轻松进行故障排除。</td>
  </tr>
  <tr>
    <td>文档</td>
    <td>为您的组织定义用户和角色。<br>定义添加新用户/管理员的过程。</td>
  </tr>
  <tr>
    <td>沙盒（如果适用）</td>
    <td>如果您有沙盒，请查看上面的类别。</td>
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
    <td>确定数量<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html" target="_blank"> 工作区</a> 和/或您的组织需要拥有的和/或分区 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html" target="_blank">每个工作区有多少用户具有访问权限。</a><br>定义每个工作区和分区的主要用途。<br>定义工作区和分区之间的关系。</td>
  </tr>
  <tr>
    <td>文档</td>
    <td>记录工作区的定义方式以及它与数据库分区（即，可看到每个人而非业务部门的全局工作区）的关系。 <br>将新记录导入相应的分区。<br>在CRM中定义将用户放置到相应分区的值。</td>
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
  <tr>
    <th>区域</th>
    <th>操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Smart Campaign设置</td>
    <td>添加 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html" target="_blank">Smart Campaign大小限制</a>，防止意外地通过电子邮件发送整个数据库。</td>
  </tr>
  <tr>
    <td>文档</td>
    <td>记录工作区的定义方式以及它与数据库分区（即，可看到每个人而非业务部门的全局工作区）的关系。  <br>将新记录导入相应的分区。<br>在CRM中定义将用户放置到相应分区的值。</td>
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
    <td>在品牌策略域下，选择您的域并添加电子邮件CNAME。 其格式应为： [EmailTrackingCNAME]。[CompanyDomain].com.  <br><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console" target="_blank">联系Marketo支持</a> 以通过SSL证书配置保护它。 完成此过程最多可能需要3个工作日。</td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html" target="_blank">设置SPF和DKIM</a> 实现电子邮件可投放性。</td>
  </tr>
  <tr>
  </tr>
  <tr>
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
    <td>地标 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank" rel="noopener noreferrer">通信限制</a>.<br>确定您的企业是否需要有关通信限制的政策 </td>
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
    <td>定义使用方法 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html" target="_blank" rel="noopener noreferrer">渠道</a>.</td>
  </tr>
  <tr>
    <td>标记</td>
    <td>定义使用方法 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html" target="_blank" rel="noopener noreferrer">标记</a>.</td>
  </tr>
  <tr>
    <td>日历（如果适用）</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html" target="_blank" rel="noopener noreferrer">问题营销日历名额</a> 给那些需要访问的人。 <br>设置 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank" rel="noopener noreferrer">日历。</a></td>
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
    <td>实施命名约定 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank" rel="noopener noreferrer">自定义字段。</a> 例如，以“MKTO”开头。<br>选择您同步的字段。 您同步的字段越多，同步周期就越慢。<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank" rel="noopener noreferrer">阻止更新字段</a> 您需要写入一次（即，原始商机来源、原始商机来源详细信息、首次联系UTM字段等）</td>
  </tr>
  <tr>
  </tr>
  <tr>
    <td>自定义活动</td>
    <td>定义 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html">自定义活动</a> 特定于您的业务。  </td>
  </tr>
  <tr>
    <td>自定义对象</td>
    <td>查看数量 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html">自定义对象</a> 你需要。 <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html">将这些自定义对象同步到您的CRM</a>. </td>
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
    <td>启动CRM同步。 根据贵公司使用的CRM，从以下内容中进行选择： <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html">Microsoft Dynamics</a>. <br>确定访问CRM所需的访问权限类型。 <br>确定您的CRM管理员以进行疑难解答。 </td>
  </tr>
  <tr>
    <td>登陆页面</td>
    <td>注意：您是否为Launch Pack客户？ 您可以跳过此步骤。 您的顾问将在您的启动电话中为您提供IT设置说明文档。 <br>使用设置登陆页面域 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html">CNAME</a> 和 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html">输入域和页面信息</a>. 其格式应为： [LandingPageCNAME]。[公司域].com <br>为您的登陆页面选择一个CNAME。 一些示例： <br>* **开始**。[公司域].com <br>* **www2**。[公司域].com <br>* **lp**。[公司域].com <br><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console">联系Marketo支持</a> 开始预配SSL证书的进程。 完成此过程最多可能需要3个工作日。 <br>提示：简明扼要！ 较短的URL更容易记忆。 我们建议“开始”作为域。 <br>将Analytics跟踪代码(例如Google Analytics或Adobe Analytics)添加到您的登陆页面模板。 </td>
  </tr>
  <tr>
    <td>蒙奇金</td>
    <td>注意：如果您是Launch Pack客户，请跳过此步骤。 您的顾问将在IT设置说明文档中为您提供Munchkin代码说明。 <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html">添加Munchkin跟踪代码</a> 到您的网站。 Munchkin代码可以是 <a href="https://developers.marketo.com/javascript-api/lead-tracking/">硬编码</a> 或通过Google Tag Manager部署。  </td>
  </tr>
  <tr>
    <td>Web服务</td>
    <td>启用 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html">IP限制</a> 如果适用。 <br>确定可以进行的用户/应用程序 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html">API调用</a> 在您的实例中。 <br>审查将发起API调用的所有应用程序，并确定API调用是否需要增加或减少。  </td>
  </tr>
  <tr>
    <td>启动点</td>
    <td>需要设置 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html">启动点</a> 服务您的业务。 每个LaunchPoint都应与唯一的API用户配对，以帮助进行故障排除。  </td>
  </tr>
  <tr>
    <td>交互式网络研讨会（如果适用）</td>
    <td>注意：交互式网络研讨会仅提供给生产实例。 <br>要创建交互式网络研讨会，内置网络研讨会功能， <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management">将用户添加到“用户”部分</a> 在交互式网络研讨会选项卡上。 </td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat（如果适用）</td>
    <td>使用 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html">Dynamic Chat</a>，即Marketo Engage中的本机对话自动化渠道，您将按照以下步骤继续设置用户权限： <a href="https://adminconsole.adobe.com/">Adobe Admin Console</a>. <br>确认您的Adobe组织系统管理员是否向您授予Adobe产品管理员角色。 联系人 <a href="https://helpx.adobe.com/contact.html">Adobe客户关怀</a> 以了解贵组织中的哪些人员具有控制台中的管理员权限。 <br>Accept <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">“Dynamic Chat产品管理员”邀请</a>. 此 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">欢迎电子邮件</a> 当您在Marketo Engage实例中启用了Dynamic Chat并且您被指定为系统管理员时，将会发送此事件。  <br>在Adobe Admin Console中为Dynamic Chat的产品配置文件分配所有适当的用户。 <br>如果将不需要的用户添加到多个产品配置文件，则必须从所有产品配置文件中删除该用户。 否则，他们仍可以访问Dynamic Chat。 <br>您可以 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">在Dynamic Chat中编辑产品配置文件</a> 并创建具有自定义集的自定义配置文件 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">您的订阅中可用的权限</a>. <br>将用户分配到 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role">“访问Dynamic Chat”角色</a> 位于“Marketo Engage”/“管理员”/“用户和角色”。 </td>
  </tr>
  <tr>
    <td>销售分析（如果适用）</td>
    <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account">设置销售分析操作</a> “销售分析”&gt;“操作配置”中的。  <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions">将名额发给适当的用户。</a>  <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html">配置API</a>. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html">自定义潜在客户得分。</a> </td>
  </tr>
  <tr>
    <td>Sales Connect （如果适用）</td>
    <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance">邀请适当的Marketo Engage管理员加入Sales Connect实例</a>. <br>完成 <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins">其他Sales Connect管理员设置</a> Sales Connect和Salesforce中的。 </td>
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
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html">启用Treasure Chest</a> 以试用功能。  <br>确定要打开或关闭的功能。 </td>
  </tr>
  <tr>
    <td>活动检查器 </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html">打开活动检查器</a> 一次查看您的所有Smart Campaigns。 </td>
  </tr>
</tbody>
</table>

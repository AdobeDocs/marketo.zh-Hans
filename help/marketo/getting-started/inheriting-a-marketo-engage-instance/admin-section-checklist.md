---
description: 继承实例管理员核对清单 — Marketo文档 — 产品文档
title: 继承实例管理员核对清单
feature: Getting Started
exl-id: 088f3ce9-bf3d-4323-9cde-c39fec06c20e
source-git-commit: b95458ffab422901ef5e674756ae5e413ec542fd
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 1%

---

# 继承实例：管理员部分核对清单 {#inherited-instance-admin-section-checklist}

以下核对清单（链接到每篇文章底部的后续核对清单）由Adobe Professional Services与Marketo Champions的输入汇总在一起，可帮助您快速上手。 您也可以[下载核对清单](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx)并跟踪您的进度。

>[!TIP]
>
>如果您是Marketo Engage的新用户并且不熟悉其中的许多术语，请查看[Marketo Engage术语表](/help/marketo/getting-started/things-to-know/marketo-engage-glossary.md){target="_blank"}。

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>这仅适用于登记到[Adobe Identity Management System (IMS)](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}的Marketo Engage订阅。 如果您的订阅尚未载入Adobe IMS，请在“Marketo Engage”>“管理员”>“用户和角色”中继续[旧版用户角色和权限体验](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}。

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">面积</th> 
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>订阅和Marketo Engage产品管理员</td> 
   <td><li>您的Marketo Engage订阅是否已迁移到<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a>？ 
<br/>     如果是这样，您的“Adobe Admin Console系统管理员”是否已向您授予“Adobe Admin Console产品管理员”角色？ 如果您不确定贵组织中的哪些人具有控制台中的管理员权限，请联系<a href="https://helpx.adobe.com/contact.html" target="_blank">Adobe客户关怀团队</a>。</li>
<li>您是否接受了“Marketo Engage产品管理员”邀请？ 在Adobe Admin Console中分配角色后，将发送电子邮件。
<br/>     如果没有，请在收件箱中查找<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#initial-setup" target="_blank">欢迎电子邮件</a>，并接受邀请以激活您的Adobe ID。</li></td>
  </tr>
  <tr> 
   <td>产品配置文件</td> 
   <td><li>是否已将所有适当的用户分配给Adobe Admin Console中的Marketo Engage产品配置文件？
<br/>     如果不能，请确保在Adobe Admin Console中<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md" target="_blank">添加和/或删除Marketo Engage产品配置文件中的用户</a>。 如果已将用户添加到产品配置文件，则无法在Marketo Engage &gt;管理员&gt;用户和角色中分配用户角色。</li>
<p><img src="assets/note-icon.png" alt="注释图标"> 注意：如果将不需要的用户添加到多个产品配置文件，则必须将该用户从所有产品配置文件中删除。 否则，他们仍可以访问Marketo Engage。</td>
  </tr>
  <tr> 
   <td>用户管理API</td> 
   <td><li>您的订阅是否使用任何Marketo用户管理API？
<br/>     如果是，您将需要使用<a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">Adobe IMS API</a>来邀请、更新和删除用户。</li>
<p><img src="assets/note-icon.png" alt="注释图标"> 注意：“角色管理”仍保留在Marketo Engage中，并且Marketo用户管理API仍可用于角色管理。</td>
  </tr>
 </tbody> 
</table>

## 用户和角色 {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>用户</td> 
   <td><img src="assets/note-icon.png" alt="注释图标"> 注意：如果您的订阅已经在Adobe IMS上，请继续在Adobe Admin Console中进行以下用户管理审查。 否则，请在Marketo Engage中转到管理员&gt;用户和角色&gt;用户。
   <p>
   <li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">有多少用户</a>？</li>
<li>是否有任何应<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md#remove-a-user" target="_blank">移除</a>的用户？</li>
<li>贵公司是否有删除用户的相关政策？</li> 
<li>有多少用户具有<a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">管理员权限</a>？</li>
<li>这些用户中的任何一个是否应更改为<a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">其他角色？</a></li> 
<li>此实例中的<a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">API用户</a>是谁？</li></td>
  </tr>
  <tr> 
   <td>角色</td> 
   <td><img src="assets/note-icon.png" alt="注释图标"> 注意：无论您是否将Marketo与Adobe身份一起使用，请继续在“管理员”&gt;“用户和角色”&gt;“角色”下查看Marketo Engage中的角色权限。
   <p><li>有多少角色？</li>  
<li>每个角色具有哪些<a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">权限/访问权限</a>？ 是否应对任何内容进行调整？</li>
<li>每个角色有多少用户？</li>
<li>用户<a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">登录</a>的频率如何？</li>
<li>每个API用户是否都有自己的<a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">用户角色</a>？ 如果不能，请考虑实施此操作以更轻松地排除故障。</li> 
<li>您的用户角色和权限是否与公司数据隐私政策保持一致，以符合法规（例如，<a href="https://gdpr-info.eu/" target="_blank">GDPR</a>）？ 公司数据<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">隐私策略</a>是否允许用户下载和共享Marketo Engage用户数据？ 需要许可业务吗？</li></td>
  </tr>
  <tr> 
   <td>支持用户</td> 
   <td><li>您在支持门户中是否设置了适当的<a href="/help/marketo/getting-started/initial-setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">授权联系人</a>？</li></td>
  </tr>
  <tr> 
   <td>内部文档</td> 
   <td><li>您的组织中是否明确定义了用户和角色？</li>
<li>您添加新用户/管理员的流程是什么？</li></td>
  </tr>
  <tr> 
   <td>沙盒（如果适用）</td> 
   <td><li>您是否有<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">沙盒实例</a>？
   <br/>     如果是这样的话，请查看上面针对沙盒的类别。</li>
<li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">项目导入</a>是否与您的沙盒关联？</li></td>
  </tr>
 </tbody> 
</table>

## 审核记录 {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>审核记录</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">谁正在实例中工作</a>？</li></td>
  </tr>
 </tbody> 
</table>

## 工作区和分区 {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>工作区和分区</td> 
   <td><li>您有多少个<a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">工作区和/或分区</a>？</li>
<li>每个Workspace和分区的主要用途是什么？</li>
<li>是否需要审核/更改您的<a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">工作区</a>或<a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">分区</a>？</li>
<li>工作区和分区之间的关系是什么？</li>
<li>有多少用户<a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">有权访问每个Workspace</a>？</li></td>
  </tr>
  <tr> 
   <td>内部文档</td> 
   <td><li>如何定义工作区和分区？</li>
<li>将工作区添加到实例或将用户添加到Workspace的过程是怎样的？</li></td>
  </tr>
 </tbody> 
</table>

## 智能营销活动 {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>智能营销活动</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">您是否对Smart Campaign的大小有限制</a>？ 
   <br/>     如果不能，请考虑添加一个。 我们建议将Smart Campaign限制为数据库的25%，以避免在工作流程中过度通信或处理整个数据库；这不仅可以保护您的品牌，还有助于保护实例的性能。</li></td>
  </tr>
 </tbody> 
</table>

## 通信限制 {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>通信限制</td> 
   <td><li>是否存在<a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">通信限制</a>？ 贵企业是否有可能需要通信限制的政策？</li>
<p><img src="assets/note-icon.png" alt="注释图标"> 注意：我们建议将您的通信限制为每天1封，每7天3封，并阻止<b>非</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">可操作</a>电子邮件。</td>
  </tr>
 </tbody> 
</table>

## 标记 {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>标记</td> 
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">有多少标记</a>？ 正在使用多少个标记？ 是否需要添加任何内容？</li>
<li>您的项目中是否需要标记？</li></td>
  </tr>
  <tr> 
   <td>渠道</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">有多少个渠道</a>？ 有多少项正在使用？</li>
<li>是否所有<a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">渠道计划状态都适合</a>？ 它们是否在计划中显示进度？</li>
<li>您的渠道是否与特定项目类型相关？</li>
<li>哪些状态被视为每个渠道的成功？ 这些是否符合您的营销目标？</li>
<li>是否正确使用了操作渠道？</li>
<li>对于高级Report Builder (Revenue Cycle Explorer/RCE)，您的渠道分析行为是否设置为与纳入期间成本的计划实践保持一致？</li></td>
  </tr>
  <tr> 
   <td>营销日历（如果适用）</td> 
   <td><li>有多少个<a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">日历条目类型</a>？ 它们仍然相关吗？</li></td>
  </tr>
 </tbody> 
</table>

## 数据库管理 {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>字段管理</td> 
   <td><li>有多少田？ 
   <br/>     单击<a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">导出字段名称</a>可查看您的字段、自定义字段及其API名称的列表。</li>
<li>有多少个<a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">自定义字段</a>？</li>
<li>使用了多少字段？ 
<br/>     在“字段操作”下拉列表中选择<a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">导出所用者</a>，以查看字段的相关资源。</li>
<li>Marketo Engage与您的CRM之间同步了多少个字段？</li>
<li>CRM字段是否已同步到相应的对象？</li>
<li>人员详细信息是否有<a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">自定义视图集</a>？ 应该有吗？</li>
<li>您的字段是否具有基于源的命名约定？ 
<br/>     如果不能，请考虑实施此操作。</li>
<li>是否存在任何字段<a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">已阻止</a>？ 
<br/>     如果是这样的话，请务必理解为什么会出现这种情况。</li></td>
  </tr>
  <tr> 
   <td>自定义活动</td> 
   <td><li>是否有任何<a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">自定义活动</a>？
<br/>     如果是这样的话，请单击它们以了解哪些活动与Marketo表单、电子邮件或登陆页面无关。</li></td>
  </tr>
  <tr> 
   <td>自定义对象</td> 
   <td><li>有多少个<a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">自定义对象</a>？ 它们如何同步到您的CRM？</li>
<li>您的程序和列表查询如何使用这些自定义对象？</li></td>
  </tr>
 </tbody> 
</table>

## 电子邮件 {#email}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>电子邮件默认设置</td> 
   <td><li>在“管理员”&gt;“电子邮件”中，所有默认设置都是最新状态（例如，<a href="/help/marketo/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.md" target="_blank">“来自”电子邮件/标签</a>、<a href="/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md" target="_blank">品牌化域</a>、<a href="/help/marketo/product-docs/administration/email-setup/edit-the-unsubscribe-message.md" target="_blank">取消订阅消息</a>等）？</li></td>
  </tr>
 </tbody> 
</table>

## 集成 {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>您正在同步到哪个CRM？ Salesforce？ MS Dynamics？ 维耶娃？</li>
<li>您是否正在使用<a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">自定义同步</a>？</li>
<li>[仅限Salesforce]您的实例是否已实施自定义同步过滤器？ 
<p><img src="assets/note-icon.png" alt="注释图标"> 注意：请联系Marketo支持以确定自定义同步筛选器或请求实施自定义同步规则。</li></td>
  </tr>
  <tr> 
   <td>登陆页面</td> 
   <td><li><a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">域设置为</a>是什么？</li>
   <li>主页设置为什么？</li>
<li><a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">回退集为</a>是什么？</li>
<li>是否启用表单预填充？</li>
<li>是否启用<a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">个性化URL</a>？</li>
<li>是否为<a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">重定向</a>设置了规则？</li>
<li>您是否已设置域别名？ 您是否跟踪您的域别名的利用方式？</li>
<li>是否启用了登陆页面的<a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">安全域</a>？ 
<br/>     确认登陆页面资产是否包含“http”URL。</li></td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>您的<a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Munchkin跟踪代码</a>是否在您的网站(不是Marketo Engage登录页面)上？</li>
<li>是否启用<a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">Do Not Track</a>浏览器请求？</li>
<li>您的<a href="https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking" target="_blank">Munchkin API</a>是否已配置？ 
<p><img src="assets/tip-icon.png" alt="提示图标">提示：如果您缺少有关munchkin代码在您网站上的位置的文档，可以通过创建<a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">网页活动报告</a>来查看所有URL。</li></td>
  </tr>
  <tr> 
   <td>Web服务</td> 
   <td><li>是否启用<a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">IP限制</a>？ 他们应该这样做吗？</li>
<li>哪些用户/应用程序正在您的实例中进行API调用？</li>
<li>您是否达到或接近达到API限制？
<br/>     如果是这样的话，请考虑增加调用次数或审核您的实例，以停止这些API调用。</li></td>
  </tr>
  <tr> 
   <td>Adobe Dynamic Chat（如果适用）</td> 
<td>执行以下步骤需要访问<a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>。 如果您尚未设置Adobe ID，请<a href="https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html" target="_blank">在此学习如何执行该操作</a>。
<br/>
<li>您是否接受了<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.md" target="_blank">Dynamic Chat产品管理员</a>邀请？ 当您在Marketo Engage实例中启用Dynamic Chat并且您被指定为系统管理员时，将发送电子邮件。
<br/>     如果没有，请在收件箱中查找欢迎电子邮件，并接受邀请来设置您的Adobe ID。</li>   
<li>您是否已将<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user" target="_blank">所需用户</a>添加到Adobe Admin Console中的Dynamic Chat产品配置文件？
<li>确保已将符合条件的用户的Dynamic Chat产品配置文件添加到其Adobe身份中。 如果将“访问Dynamic Chat”角色添加到产品配置文件，则您无法在Marketo Engage &gt;管理员&gt;用户和角色中分配这些角色。</li>
<li>在“产品配置文件”选项卡中，默认配置文件权限是否符合您组织的需求？<br/> 
如果没有，请编辑特定配置文件的权限。 </li>
<li>如果您有多个订阅，您的用户是否会添加到正确的订阅？</li>
<br>
完成用户和角色设置的审核后，请登录Dynamic Chat以继续审核。  
<li>您是否已<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md" target="_blank">将您的Marketo Engage实例</a>连接到Dynamic Chat？</li>
<li>具有预定义权限的五个默认配置文件是否适用于您的组织？<br/> 
     如果不能，您可以<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#edit-existing-permissions" target="_blank">在Dynamic Chat中编辑它们</a>。 您还可以<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#create-a-profile" target="_blank">创建具有自定义权限集的自定义配置文件</a>。</li>
<li>要向用户提供对Dynamic Chat的访问权限，您是否在“管理员”&gt;“用户和角色”&gt;“角色”下选中了适用的Marketo Engage角色的“访问Dynamic Chat”？
<br/><img src="assets/note-icon.png" alt="注释图标">注意：“管理员”和“营销用户”角色应具有对Dynamic Chat的访问权限。</li>
</td>
  </tr>
  <td>Marketo Sales Insight （如果适用）</td> 
   <td><li>是否已安装<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI包</a>？</li>
<li>您是否<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">升级到最新版本的Sales Insight</a>？</li>
<li>您是否已完成Sales Insight配置？ <br/>     Enterprise/Unlimited用户<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">单击此处</a>，Professional用户<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">单击此处</a>。</li>
<li>您是否根据已购买的名额向您的用户<a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">授予访问权限</a>？</li>
<li><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">星星和火焰</a>是否已自定义？</li></td>
  </tr>
  <tr> 
   <td>启动点（如果适用）</td> 
   <td><li>您已配置哪些服务（例如，<a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>、<a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">缩放</a>等）？ 是否有任何产品即将到期？</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">您的集成使用了多少次API调用</a>？</li>
<li>您是否针对用例实施了正确的集成？</li></td>
  </tr>
  <tr> 
   <td>Webhook（如果适用）</td> 
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">您设置了哪些连接</a>？</li>
<li>是否不再使用任何内容？</li></td>
  </tr>
  <tr> 
   <td>移动设备应用程序（如果适用）</td> 
   <td><li>您拥有哪些<a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">移动应用</a>？</li>
<li>是否添加了任何<a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">测试设备</a>？</li></td>
  </tr>
 </tbody> 
</table>

## 宝箱 {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>宝箱</td> 
   <td><li><a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">宝藏箱</a>中打开了哪些内容？</li>
<li>是否应该打开或关闭某些功能？</li></td>
  </tr>
  <tr> 
   <td>活动检查器</td> 
   <td><li><a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">营销活动检查器</a>是否已打开？
<br/>如果没有，请考虑启用它以轻松识别哪些营销活动处于活动状态：活动、与您的CRM同步，以及/或删除记录。</li></td>
  </tr>
 </tbody> 
</table>

## 警报和更新 {#alerts-and-updates}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>Marketo Engage状态更新</td> 
   <td><li>您的实例是否已订阅<a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">Marketo Engage状态更新</a>？</li></td>
  </tr>
  <tr> 
   <td>警报</td> 
   <td><li>是否有任何<a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">活动警报</a>从Marketo Engage发送到内部团队？</li>
<li>如果是，这些警报是否正常运行？</li></td>
  </tr>
  <tr> 
   <td>通知</td> 
   <td><li>您订阅了相应的管理员<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">通知</a>吗？</li></td>
  </tr>
 </tbody> 
</table>

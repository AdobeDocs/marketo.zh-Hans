---
description: 继承实例管理员核对清单 — Marketo文档 — 产品文档
title: 继承实例管理员核对清单
hide: true
hidefromtoc: true
source-git-commit: 8660e8a7afa239c51cfed9e6e90e35aeedf6884f
workflow-type: tm+mt
source-wordcount: '1444'
ht-degree: 1%

---

# 继承实例：管理员部分核对清单 {#inherited-instance-admin-section-checklist}

以下核对清单（链接到每篇文章底部的后续核对清单）与Marketo Champions的输入一起放在一起，帮助您快速上手。 您还可以下载核对表并跟踪您的进度。

>[!TIP]
>
>如果您是新Marketo Engage用户并且不熟悉许多术语，请查看 [Marketo Engage术语表](/help/marketo/getting-started/marketo-engage-glossary.md){target="_blank"}.

## AdobeIdentity Management {#adobe-identity-management}

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th> 
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>订阅</td> 
   <td><li>您的Marketo Engage订阅是否位于 <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">AdobeIdentity Management System</a> (Adobe IMS)了吗？ 
<br/>     如果是这样，您的“Adobe Admin Console系统管理员”是否已向您授予“Adobe Admin Console产品管理员”角色？ 如果您不确定贵组织中的哪些人具有控制台中的管理员权限，请联系 <a href="https://helpx.adobe.com/contact.html" target="_blank">Adobe客户关怀</a>.  
<br/>     否则，您将继续 <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">旧版用户角色和权限体验</a> 在Marketo Engage&gt;管理员&gt;用户和角色中，直到续订您的订阅。</li></td>
  </tr>
  <tr> 
   <td>产品配置文件</td> 
   <td>(Adobe IMS上的订阅 <b>仅限</b>)
<p>
<li>您是否已被授予“Marketo Engage产品管理员”角色(Marketo Engage/管理员/用户和角色)？</li> 
<li>您是否已经将Marketo Engage分配给Adobe Admin Console中所有相应的用户的产品配置文件？
<br/>     如果不能，请确保先为其Adobe IMS产品配置文件分配Marketo Engage，然后再分配其Marketo Engage/管理员/用户和角色角色。</li>
<p><img src="assets/note-icon.png" alt="注释图标"> 注意：如果您的订阅具有75个以上的用户，并且您刚刚迁移到Adobe IMS，则您可以选择分批迁移并管理其Adobe标识的用户，也可以一次性管理这些用户。 详细了解期待完成的任务 <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md#prepare-users-for-migration-day" target="_blank">Adobe IMS迁移日</a>.</td>
  </tr>
  <tr> 
   <td>用户管理API</td> 
   <td><li>您的订阅是否使用了任何Marketo用户管理API？
<br/>     如果是这样的话，您需要使用 <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">Adobe IMS API</a> 以邀请、更新和删除用户。</li></td>
  </tr>
 </tbody> 
</table>

## 用户和角色 {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>用户</td> 
   <td><li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">用户数量</a> 有吗？</li>
<li>是否有任何应过期的用户？</li>
<li>贵公司是否有删除用户的相关政策？</li> 
<li>有多少用户 <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">管理员权限</a>？</li>
<li>如果这些用户中的任何一个更改为 <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">其他角色？</a></li> 
<li>谁是 <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">API用户</a> 在这个例子里？</li></td>
  </tr>
  <tr> 
   <td>角色</td> 
   <td><li>有多少角色？</li>  
<li>什么 <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">权限/访问</a> 每个角色都有吗？ 是否应对任何内容进行调整？</li>
<li>每个角色有多少用户？</li>
<li>用户的频率 <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">登录</a>？</li>
<li>每个API用户是否都有 <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">自己的用户角色</a>？ 如果不能，请考虑实施此操作以更轻松地排除故障。</li> 
<li>您的用户角色和权限是否与公司数据保持一致 <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">隐私政策</a>？</li></td>
  </tr>
  <tr> 
   <td>支持用户</td> 
   <td><li>是否已设置适当的 <a href="/help/marketo/getting-started/setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">授权联系人</a> 在支持门户中？</li></td>
  </tr>
  <tr> 
   <td>内部文档</td> 
   <td><li>您的组织中是否明确定义了用户和角色？</li>
<li>您添加新用户/管理员的流程是什么？</li></td>
  </tr>
  <tr> 
   <td>沙盒（如果适用）</td> 
   <td><li>您是否拥有 <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">沙盒实例</a>？
   <br/>     如果是这样的话，请查看上面针对沙盒的类别。</li>
<li>是 <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">项目导入</a> 与您的沙盒相关联？</li></td>
  </tr>
 </tbody> 
</table>

## 审核记录 {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>审核记录</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">谁在工作</a> 在实例中？</li></td>
  </tr>
 </tbody> 
</table>

## 工作区和分区 {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>工作区和分区</td> 
   <td><li>数量 <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">工作区和/或分区</a> 您有吗？</li>
<li>每个工作区和分区的主要用途是什么？</li>
<li>执行以下任一操作 <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">工作区</a> 或 <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">分区</a> 需要审核/更改？</li>
<li>工作区和分区之间的关系是什么？</li>
<li>用户数量 <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">具有访问权限</a> 每个工作区？</li></td>
  </tr>
  <tr> 
   <td>内部文档</td> 
   <td><li>如何定义工作区和分区？</li>
<li>将工作区添加到实例或将用户添加到工作区的流程是什么？</li></td>
  </tr>
 </tbody> 
</table>

## 智能营销活动 {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>Smart Campaign设置</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">您是否有限制</a> Smart Campaign规模？ 
   <br/>     如果不能，请考虑添加一个。 我们建议将Smart Campaign限制为数据库的25%，以避免在工作流程中过度通信或处理整个数据库；这不仅可以保护您的品牌，还有助于保护实例的性能。</li></td>
  </tr>
 </tbody> 
</table>

## 通信限制 {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>通信限制</td> 
   <td><li>是否存在 <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">通信限制</a> 就位？ 贵企业是否有可能需要通信限制的政策？</li>
<p><img src="assets/note-icon.png" alt="注释图标"> 注意：我们建议将通信限制为每天1次，每7天3次，使用 <b>非</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">可操作</a> 电子邮件被阻止。</td>
  </tr>
 </tbody> 
</table>

## 标记 {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>标记</td> 
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">标记数量</a> 有吗？ 正在使用多少个标记？ 是否需要添加任何内容？</li>
<li>您的项目中是否需要标记？</li></td>
  </tr>
  <tr> 
   <td>渠道</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">渠道数量</a> 有吗？ 有多少项正在使用？</li>
<li>全部 <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">渠道计划状态适当</a>？ 它们是否在计划中显示进度？</li>
<li>您的渠道是否与特定项目类型相关？</li>
<li>哪些状态被视为每个渠道的成功？ 这些是否符合您的营销目标？</li>
<li>是否正确使用了操作渠道？</li>
<li>对于高级Report Builder(Revenue Cycle Explorer/RCE)，您的渠道分析行为是否设置为与纳入期间成本的计划实践保持一致？</li></td>
  </tr>
  <tr> 
   <td>营销日历（如果适用）</td> 
   <td><li>数量 <a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">日历条目类型</a> 有吗？ 它们仍然相关吗？</li></td>
  </tr>
 </tbody> 
</table>

## 数据库管理 {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>字段管理</td> 
   <td><li>有多少田？ 
   <br/>     单击 <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">导出字段名称</a> 查看您的字段、自定义字段及其API名称的列表。</li>
<li>数量 <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">自定义字段</a> 有吗？</li>
<li>使用了多少字段？ 
<br/>     选择 <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">导出使用者</a> 字段操作下拉列表中的以查看字段的相关资源。</li>
<li>Marketo Engage与您的CRM之间同步了多少个字段？</li>
<li>CRM字段是否已同步到相应的对象？</li>
<li>是否存在 <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">自定义视图集</a> 人员详细信息？ 应该有吗？</li>
<li>您的字段是否具有基于源的命名约定？ 
<br/>     如果不能，请考虑实施此操作。</li>
<li>是否存在任何字段 <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">已阻止</a>？ 
<br/>     如果是这样的话，请务必理解为什么会出现这种情况。</li></td>
  </tr>
  <tr> 
   <td>自定义活动</td> 
   <td><li>是否有任何 <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">自定义活动</a>？
<br/>     如果是这样的话，请单击它们以了解哪些活动与Marketo表单、电子邮件或登陆页面无关。</li></td>
  </tr>
  <tr> 
   <td>自定义对象</td> 
   <td><li>数量 <a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">自定义对象</a> 有吗？ 它们如何同步到您的CRM？</li>
<li>您的程序和列表查询如何使用这些自定义对象？</li></td>
  </tr>
 </tbody> 
</table>

## 集成 {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>您正在同步到哪个CRM？ Salesforce? MS Dynamics？ 维耶娃？</li>
<li>您是否正在利用 <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">自定义同步</a>？</li>
<li>[仅限Salesforce]您的实例是否实施了自定义同步过滤器？ 
<p><img src="assets/note-icon.png" alt="注释图标"> 注意：请联系Marketo支持以确定自定义同步筛选器或请求实施自定义同步规则。</li></td>
  </tr>
  <tr> 
   <td>登陆页面</td> 
   <td><li>什么是 <a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">域集为</a>？</li>
   <li>主页设置为什么？</li>
<li>什么是 <a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">回退集为</a>？</li>
<li>是否启用表单预填充？</li>
<li>是 <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">个性化URL</a> 已启用？</li>
<li>是否已为以下对象设置规则 <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">重定向</a>？</li>
<li>您是否已设置域别名？ 您是否跟踪您的域别名的利用方式？</li>
<li>是 <a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">登陆页面的安全域</a> 已启用？ 
<br/>     确认登陆页面资产是否包含“http”URL。</li></td>
  </tr>
  <tr> 
   <td>蒙奇金</td> 
   <td><li>是您的 <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Munchkin跟踪代码</a> (不在Marketo中)？</li>
<li>是 <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">不跟踪</a> 是否启用了浏览器请求？</li>
<li>是您的 <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">Munchkin API</a> 已配置？ 
<p><img src="assets/tip-icon.png" alt="提示图标">提示：如果您缺少有关munchkin代码在您的网站上的位置的文档，则可以通过创建 <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">网页活动报表</a>.</li></td>
  </tr>
  <tr> 
   <td>Web服务</td> 
   <td><li>是 <a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">IP限制</a> 已启用？ 他们应该这样做吗？</li>
<li>哪些用户/应用程序正在您的实例中进行API调用？</li>
<li>您是否达到或接近达到API限制？ 
<br/>     如果是这样的话，请考虑增加调用次数或审核您的实例，以停止这些API调用。</li></td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight （如果适用）</td> 
   <td><li>具有 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">已安装MSI包</a>？</li>
<li>您是否拥有 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">已升级到最新版本的Sales Insight</a>？</li>
<li>您是否已完成Sales Insight配置？ <br/>     企业/无限用户 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">单击此处</a>，专业用户 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">单击此处</a>.</li>
<li>您是否拥有 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">授予您的用户访问权限</a> 根据你买的座位数？</li>
<li>是 <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">星星和火焰</a> 自定义？</li></td>
  </tr>
  <tr> 
   <td>启动点（如果适用）</td> 
   <td><li>您已配置哪些服务(例如， <a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>， <a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">缩放</a>等)？ 是否有任何产品即将到期？</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">API调用数</a> 您的集成使用的是？</li>
<li>您是否针对用例实施了正确的集成？</li></td>
  </tr>
  <tr> 
   <td>Webhook（如果适用）</td> 
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">哪些连接</a> 你准备好了吗？</li>
<li>是否不再使用任何内容？</li></td>
  </tr>
  <tr> 
   <td>移动设备应用程序（如果适用）</td> 
   <td><li>哪个 <a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">移动应用程序</a> 您有吗？</li>
<li>拥有任何 <a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">测试设备</a>  已添加？</li></td>
  </tr>
 </tbody> 
</table>

## 宝箱 {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>宝箱</td> 
   <td><li>中打开的内容 <a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">宝箱</a>？</li>
<li>是否应该打开或关闭某些功能？</li></td>
  </tr>
  <tr> 
   <td>活动检查器</td> 
   <td><li>是 <a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">活动检查器</a> 打开？
<br/>如果不能，请考虑启用它以轻松识别哪些营销活动处于活动状态：活动、与您的CRM同步，以及/或删除记录。</li></td>
  </tr>
 </tbody> 
</table>

## 警报和更新 {#alerts-and-updates}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th>
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>Marketo Engage状态更新</td> 
   <td><li>您的实例是否已订阅 <a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">Marketo Engage状态更新</a>？</li></td>
  </tr>
  <tr> 
   <td>警报</td> 
   <td><li>是否有任何 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">活动警报</a> 被Marketo Engage派去内部团队吗？</li>
<li>如果是，这些警报是否正常运行？</li></td>
  </tr>
  <tr> 
   <td>通知</td> 
   <td><li>您是否订阅了相应的管理员 <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">通知</a>？</li></td>
  </tr>
 </tbody> 
</table>

<br> 

[审核继承的实例：数据库►](/help/marketo/getting-started/inheriting-a-marketo-instance/new-inherit-doc-2.md)

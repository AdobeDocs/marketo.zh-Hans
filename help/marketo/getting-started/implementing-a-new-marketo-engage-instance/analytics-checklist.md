---
description: 为您的新Marketo Engage实例设置Analytics部分。
title: 新实例最佳实践 — 分析核对清单
feature: Getting Started
exl-id: ddbb9bc7-d06a-4a2e-a560-9d308630ae3f
source-git-commit: 7a847ece020ea0c0001241abf8e49b9eadf8edce
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# 新实例最佳实践：Analytics清单 {#new-instance-best-practices-analytics-checklist}

Analytics部分提供可分析营销工作性能的全局报表。 了解导航所需的步骤。

请记住[下载核对清单](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)并跟踪您的进度。

## 树 {#tree}

<table>
<thead>
  <tr>
    <th style="width:20%">面积图</th>
    <th style="width:80%">操作项</th>
    <th></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>组织：命名、文件夹和存档</td>
    <td><li>使用报告命名惯例来区分“全局报告”选项卡中的报告。
    <ul><li>良好命名惯例的示例是[报告类型] [全局与特定于BU的标记] [报告描述]，如[电子邮件性能]-[全局]-[180天电子邮件参与]。</li></ul><br>
    <li>确定应与您组织中不同用户组（例如，销售团队、营销领导层）共享的报表，并在Analytics for Global Reports的“组报表”文件夹内按文件夹整理报表。</li> 
    <li>存档应限制为全局报告文件夹，因为这些报告始终处于开启状态。   <ul><li>将存档限制为组织更改，例如，如果您根据业务部门结构报告，则减少或添加相关的业务部门。</li></ul>
    </td>
  </tr>
  <tr>
    <td>工作区（如果适用）</td>
    <td><li>跨工作区复制全局报告和文件夹结构，以保持团队的报告一致。 这些报告将位于组报告文件夹中。</li></td>
  </tr>
  <tr>
    <td>我的报表</td>
    <td><li>识别并创建在<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">我的报告</a>部分中使用的所需报告。 使用此专用报表分区作为全局报表的沙盒。 它们仅适用于创建报告的用户。</li>
    <li>使用您组织的命名惯例来标识报告和用法，以便您可以协调“我的报告”中的报告与“组报告”中的报告。</li></td>
  </tr>
  <tr>
    <td>组报表</td>
    <td><li>组报告是您组织的全局报告，应报告组织的整体活动。</li>
    <li>考虑创建<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">可克隆的核心报告</a>，您希望每个业务部门最常使用，以减少提取报告所需的时间并确保数据正确。 请参阅下面<a href="#global-reports">全局报告表中的详细信息</a>。
    <ul><li>人员绩效报表（全时和基于时间），按来源、月份</li>
    <li>项目执行情况报告（按成本月份，基于时间）</li>
    <li>电子邮件性能报表（基于时间）</li></ul>
    <li><a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">在报表的“设置”选项卡中打开“全局报告”</a>，将来自您所有工作区的数据包含在电子邮件性能和电子邮件链接性能报表中。 如果您有多个工作区，则只需在默认工作区中启用它即可。</li>
    <p><img src="assets/tip-icon.png" alt="注释图标"> 提示：创建<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">智能列表</a>时，应包含要包含在数据库部分大多数报表中的筛选器。 当需要更新智能列表条件时，可以在一个位置更新它，而不是在所有全局报告中更新它。</td>
  </tr>
</tbody>
</table>

## 订阅 {#subscriptions}

<table>
<thead>
  <tr>
    <th style="width:20%">面积图</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>订阅</td>
    <td><li>与您的营销负责人保持一致，了解哪些人应该审查报告结果以及他们在实施过程中的节奏。</li> <li>使用订阅将数据分发给组织中的需要了解的人员，而不用用耗尽指定的用户许可证。</li>
    <p><img src="assets/tip-icon.png" alt="注释图标"> 提示：如果您希望用户访问实时报表数据，则需要将他们添加为用户，以便他们能够查看报表。
    <p>
    <li><a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">按照所需的节奏（每日/每周/每月）设置订阅</a>，以便每个团队持续监控。 您还可以在Analytics的“订阅”选项卡下，在一个位置<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">查看您的所有订阅</a>。</li></td>
  </tr>
</tbody>
</table>

## 全局报告 {#global-reports}

确定应与您组织内的不同用户组（例如，销售团队、营销领导层）共享的报表。 为每个团队/用户组/业务部门创建适当的文件夹结构，以便在组报表中组织克隆的报表。 请考虑设置全局报表，例如：

<table>
<thead>
  <tr>
    <th style="width:20%">报告类型</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>电子邮件性能报表</td>
    <td><li>选择正确的电子邮件以创建全局、Workspace/业务部门范围的报告。</li>
    <li>在所有可克隆的计划模板中创建本地电子邮件性能报告。</li>
    <li><a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">使用相关时间范围</a>（例如，YTD、过去90天等） ，以准确了解标准电子邮件参与度和可投放性指标。</li>
    <p><img src="assets/tip-icon.png" alt="注释图标"> 提示： <a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">在<strong>管理员&gt;电子邮件</strong></a>中打开“机器人活动”筛选以避免日志记录，或识别是否为机器人活动启用了日志记录。 包含该过滤器，以便仅允许<a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">在可克隆全局报告的智能列表中将“Is Bot Activity”约束设置为“False”的已打开/已单击活动</a>。</td>
  </tr>
  <tr>
    <td>人员绩效报表</td>
    <td><img src="assets/note-icon.png" alt="注释图标"> 注意：建议您为每个Marketo Engage实施制定适当的<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">渠道和标记策略</a>，然后才能按渠道跟踪获得的人员以及营销投资的ROI。
    <p>
    <li>确定将用于衡量商机获取计划绩效的标准，并根据这些指标创建基于时间（当前年份、最近连续12个月或180天）的标准报表： <ul><li>客户获取计划：为获取人员而贷记的Marketo Engage计划。</li>
    <li>人员Source：数据库了解记录的源类别（基于CRM中的源值列表）
    </li></ul>
    <li>按周或月衡量创建的人员。 该报告将为您提供数据库增长率的衡量标准以及您是否接近数据库大小限制。</li>
    <li>将您的智能列表作为自定义列，按<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">筛选人员绩效报表中的指标。</a></li>
    <p><img src="assets/tip-icon.png" alt="注释图标"> 提示：为要添加到数据库中的“人员绩效报表”而不是“营销活动”的自定义列创建智能列表，以便您在报表中选择智能列表后能够正确而清楚地查看智能列表名称。</td>
  </tr>
  <tr>
    <td>项目执行情况报告</td>
    <td><p><img src="assets/note-icon.png" alt="注释图标"> 注意：此报表要求您在<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong>管理员</strong> &gt; <strong>标记</strong></a>中定义渠道、进度状态和成功步骤。
    <p>
    <li><a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">在选择性项目中衡量营销策略的有效性</a>。</li>
    <li>根据营销活动中的最佳实践管理项目成员资格（使用智能营销活动更新客户获取项目、状态、成功状态）。</li>
    <li>按本年度和连续12个月的成本计量。
    <ul><li>请记住，维护<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">期间成本</a>对于利用项目性能报告至关重要。</li></ul></li>
    <p>
    <img src="assets/tip-icon.png" alt="注释图标">提示：若要汇总和查看项目性能报表中的任何<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">导入的列表</a>，请确保您的团队选择适当的客户获取项目来进行标记。 当导入的列表不适用于任何渠道时，考虑<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">创建一个要选作客户获取项目的默认项目</a>。 这可确保导入的任何人员都具备与来源、业务部门、渠道等相关的有效客户获取计划，而不是空白值。</td>
  </tr>
  <tr>
    <td>登陆页面性能报表</td>
    <td><li>将<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">登陆页面性能报表</a>创建为全局报表，以便您可以<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">在一个位置</a>筛选和查看您的所有设计工作室/营销活动登陆页面的数量。</li>
    <li>对于具有登陆页面的程序，请考虑<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">在程序模板</a>中创建专用本地报告，以便在程序级别查看性能。</li></td>
  </tr>
  <tr>
    <td>网页活动报表</td>
    <td><img src="assets/note-icon.png" alt="注释图标"> 注意：此报表中仅跟踪启用了<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">Munchkin JavaScript</a>的网页(外部和Marketo登录页面)。 考虑将JavaScript代码放在Tag Management平台中，如<a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a>，以避免对每个网页上的代码进行硬编码。
    <p>
    <li>创建<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">网页活动报告</a>作为全局报告，以便在一个位置查看所有网页的数量。 请注意，您的外部网页活动仅反映在网页活动报表中。</li></td>
  </tr>
</tbody>
</table>

## 本地报表 {#local-reports}

某些Marketo Engage报表最好作为本地资源部署在营销活动中的特定项目中，因为它们的典型用法是在一组更为有限的项目和资源中。 考虑设置基本报表，例如：

<table>
<thead>
  <tr>
    <th style="width:20%">报告类型</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>电子邮件链接性能报表</td>
    <td><li>在发送电子邮件的项目和您的滴答式促销活动中创建<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">电子邮件链接性能报表</a>，以洞察用户在电子邮件中点击的链接。</li></td>
  </tr>
  <tr>
    <td>营销活动报表</td>
    <td><li>创建<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">促销活动报表</a>，并在营销活动的操作文件夹中选择一个句点。</li>
    <li>设置报告以监视每个用例的触发器并<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank">应用促销活动过滤器</a>（例如，行为评分触发器、生命周期资格触发器、有趣的时间触发器）。</li></td>
  </tr>
  <tr>
    <td>参与流性能报表（如果适用）</td>
    <td><li>创建<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">参与流性能报告</a>以衡量在参与计划中部署的内容和流的有效性。</li>
    <li>请考虑在报表的“设置”选项卡</a>中使用<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank">“分段”筛选器，并按参与计划中使用的<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">区段</a>（例如，人员来源、行业）对报表数据进行分组。 这将有助于更深入地了解每个区段的参与模式，指导您进行战略更改以改进参与计划（内容、流、流节奏等）。</li></td>
  </tr>
</tbody>
</table>

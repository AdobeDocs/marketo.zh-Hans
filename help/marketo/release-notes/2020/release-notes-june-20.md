---
unique-page-id: 37357276
description: 发行说明 — ’20年6月 — Marketo Docs — 产品文档
title: 发行说明 — 2020年6月
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '1073'
ht-degree: 0%

---


# 发行说明：’20年6月{#release-notes-june}

’20年6月版包含以下功能。 查看您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>由星(![(star)](assets/star-yellow.svg))表示的特征可以是付费附加项。 请联系您的Marketo Engage代表以了解更多信息。

**_季_** 度版本2020年6月5日将发 **布以下功能**。

## 核心Marketo Engage{#core-marketo-engage}

* **[预测受众](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![（星形）](assets/star-yellow.svg):新的智能列表和由Adobe Sensei提供支持的智能活动过滤器使您能够为电子邮件、事件和网络研讨会营销项目创建由人工智能提供的受众细分。使用AI根据潜在客户注册受众、参加事件或取消订阅的可能性帮助您细分事件。 根据过去的项目构建相似受众，以高效复制以前的成功。 通过预测目标跟踪实现转化目标并获取有关如何针对事件项目优化受众细分的建议。
* **批量电子邮件提** ![升（星型）](assets/star-yellow.svg):增强了我们的电子邮件营销功能，使您每小时最多可发送300万封批量电子邮件。我们重新构建了批量活动和电子邮件报告处理架构，以增强电子邮件项目和批量电子邮件活动的性能。 这会缩短发送的提前期，并改善完成时间。 设置电子邮件发送，没有额外的复杂性。 此增强功能可作为产品加载项提供，其中还包括投放服务启动包、电子邮件投放工具和多个专用IP地址。
* **[受众与Adobe Experience Cloud(AEC)集成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**:新的Adobe Experience Cloud(AEC)集成允许您将Marketo Engage中已知潜在客户的静态列表与多个AEC应用程序同步，以增强现有项目、释放新用例并协调多渠道活动。此集成包括Adobe Analytics、Adobe Target、Adobe Experience Manager、Adobe Audience Manager和Adobe Advertising Cloud。
* **[项目成员自定义字段](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**:捕获并利用有关项目成员的自定义字段。在您的Marketo Engage表单中使用这些新字段，在项目成员列表中视图它们，在智能列表过滤器和触发器中利用它们，并将它们包含在新的智能活动流动操作中以增强自动化和更精细的个性化。 还可以通过UI和API导入和导出这些组件。 增强我们的自定义数据对象和字段功能。
* **描述项目成员**:检索项目成员元数据，使您能够使用REST API导入和导出项目成员自定义字段数据。增强我们的API。
* **[在Microsoft Dynamics中创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**:根据在Marketo Engage中捕获的客户行为，使用新的“流动操作”为Microsoft Dynamics中的销售创建任务。增强了我们本机的Microsoft Dynamics CRM集成。
* **获取列表 Asset API端点使用的表单**:检索依赖表单的资产列表。增强我们的API。
* **通过API设置电子邮件头**:启用电子邮件标题字段的自动翻译和本地化。增强我们的API。
* **图像和文件缓存**:我们通过从60秒的缓存中提供图像和文件资源来增强Marketo Engage服务器的稳定性。

## 基于帐户的营销{#account-based-marketing}

![（星号）](assets/star-yellow.svg)

* **通常提供新帐户发现**

   * 新帐户发现是对我们帐户分析功能的增强，使您能够根据基于人工智能的理想目标模型发现您的ABM战略的新客户帐户。 视图、选择和导入建议的新帐户及其基于AI的适应和意图数据指示器。

<br> 

**_在整个季度内发布_**

以下功能按非季度周期发布，将在未来几个月发布。

## 可见{#bizible}

![（星号）](assets/star-yellow.svg)

* **Marketo Engage项目集成**:在Bizible中直接从Marketo Engage中提取项目数据，在归因旅程中创建接触点，以便对电子邮件和互动项目进行适当的信用。增强我们的Marketo Engage集成。
* **Marketo Engage活动集成（测试版）**:将Marketo Engage活动数据直接引入Bizible，在客户旅程和所有归因模型中创建接触点。示例包括潜在客户得分变化、有趣时刻、电子邮件点击或任何自定义活动。 增强我们的Marketo Engage集成。
* **备见的B2B客户属性集成（测试版）**:这是与Adobe Analytics的Adobe Experience Cloud集成，允许您将选定的可视数据直接引入Adobe Analytics中，以进行更深入的分析。示例包括按公司名称、帐户属性、CRM机会以及由Bizible归因收入和漏斗阶段定义的高价值个人基于帐户的网站流量和内容分析。
* **备见的Discover过滤器和增强**:利用渠道、子渠道、活动和跨仪表板的细分过滤器分析数据。利用更多向下钻取属性增强数据可见性。 这是对Discover展示板的增强。
* **活动同步Microsoft Dynamics**:将Microsoft Dynamics CRM活动引入接触点旅程，跟踪与您的潜在客户或联系人关联的事件(如呼叫、约会或任务)，从而确定销售互动的属性。增强我们的Microsoft Dynamics CRM集成。

## 销售分析{#sales-insight}

![（星号）](assets/star-yellow.svg)

* **[针对Salesforce CRM的洞察仪表板](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**:我们正在重新构思销售分析功能，并对即将到来的营销事件和活动进行全新的了解，使销售者能够根据客户和潜在客户的需求和兴趣提出更相关的建议。销售商还可以在时间轴中视图联系人和帐户活动，并轻松访问其他活动详细信息。 在](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/configuration-for-existing-customers.md)此处查找有关如何升级软件包的更多详细信息。[

<br> 

## 公告{#announcements}

* **ITP 2.1+ RTP更新**:由于Safari的Cookie策略发生更改，ITP将限制RTP Cookie在同一域上跨会话跟踪用户的能力(基于访客使用的浏览器和浏览器版本)为1天或7天。为此，我们正在实施一项新的Web服务，以允许通过HTTP响应使用Set-Cookie头设置RTP Cookie。 有关详细信息，请在[此处](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603)找到。

* **批活动基础结构更改**:我们将在今年剩余时间升级批活动服务。这将是一个无缝更新，不会影响任何正在进行的批活动，也不会导致行为发生更改。 无需执行任何操作。 有关更多详细信息，请参阅此[国家/地区帖子](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374)。

## 弃用{#deprecations}

* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:从Munchkin JS的159版开始，当调用“关联潜在客户”方法时，浏览器控制台中将记录一个停用警告，指示该功能将在将来的版本中删除。 完全弃用计划将在以后的日期宣布。

**_产品发布网_** [络研讨会观](https://engage.marketo.com/June-Release-2020-On-Demand.html) 看“2020年6月产品发布创新网络研讨会”的录制内容。

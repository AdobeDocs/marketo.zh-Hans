---
unique-page-id: 37357276
description: 发行说明 — 2020年6月 — Marketo文档 — 产品文档
title: 发行说明 — 2020年6月
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# 发行说明：’20年6月 {#release-notes-june}

’20年6月版中包含以下功能。 查看您的Marketo版本以了解功能的可用性。

>[!AVAILABILITY]
>
>以星形(![](assets/yellow-star.png))表示的功能是付费的附加组件。 请联系您的Marketo Engage代表以了解更多信息。

**_季_** 度版本以下功能将于2020年6 **月5日发布**。

## 核心Marketo Engage {#core-marketo-engage}

* **[预测受众](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![（星形）](assets/yellow-star.png):通过由Adobe Sensei提供支持的新智能列表和智能营销活动过滤器，您可以为电子邮件、事件和网络研讨会营销计划创建AI支持的受众区段。使用AI帮助您根据潜在客户注册事件、参加活动或退订的可能性对受众进行细分。 根据过去的计划构建相似人群拓展受众，以高效复制先前的成功。 通过预测目标跟踪实现转化目标，并获取有关如何为事件程序优化受众区段的建议。
* **批量电子邮件提升** ![（星形）](assets/yellow-star.png):增强了我们的电子邮件营销功能，允许您每小时发送多达300万封批量电子邮件。我们重新构建了批量营销活动和电子邮件报表处理架构，以提升电子邮件项目和批量电子邮件营销活动的性能。 这会缩短发送的前置时间，并缩短完成时间。 按常规方式设置电子邮件发送，这不会增加任何复杂性。 此增强功能可作为产品加载项使用，其中还包括Delivery Services Launch Pack、电子邮件投放工具和多个专用IP地址。
* **[受众与Adobe Experience Cloud集成(AEC)](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**:新的Adobe Experience Cloud(AEC)集成允许您将来自Marketo Engage的已知潜在客户静态列表与多个AEC应用程序同步，以增强现有项目、解锁新用例和编排多渠道活动。此集成包括Adobe Analytics、Adobe Target、Adobe Experience Manager、Adobe Audience Manager和Adobe Advertising Cloud。
* **[程序成员自定义字段](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**:捕获和利用有关项目成员的自定义字段。在您的Marketo Engage表单中使用这些新字段，在项目的成员列表中查看这些字段，在智能列表过滤器和触发器中利用它们，并将它们包含在新的智能促销活动流程操作中，以增强自动化和更精细的个性化。 这些配置文件也可以通过UI和API导入和导出。 增强了自定义数据对象和字段功能。
* **描述项目成员**:检索程序成员元数据，让您能够使用REST API导入和导出程序成员自定义字段数据。增强了我们的API。
* **[在Microsoft Dynamics中创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**:根据在Microsoft Dynamics中捕获的客户行为使用新的“流量操作”为Sales创建任务。增强我们的本机Microsoft Dynamics CRM集成。
* **获取列表资产API端点使用的表单**:检索依赖于表单的资产列表。增强了我们的API。
* **通过API设置电子邮件预标头**:启用电子邮件预标题字段的自动翻译和本地化。增强了我们的API。
* **图像和文件缓存**:我们通过从60秒的缓存中提供图像和文件资产来增强Marketo Engage服务器的稳定性。

## 基于帐户的营销 {#account-based-marketing}

![（星号）](assets/yellow-star.png)

* **新帐户发现功能通常可用**

   * 新帐户发现是对“帐户分析”功能的增强，让您能够根据AI支持的理想客户配置模型，为您的ABM战略发现新的目标帐户。 查看、选择和导入推荐的新帐户，以及其基于AI的拟合和意图数据指标。

<br> 

**_在整个季度发布_**

以下功能处于非季度周期，将在未来几个月内发布。

## Bizible {#bizible}

![（星号）](assets/yellow-star.png)

* **Marketo Engage程序集成**:直接从Marketo Engage中提取项目数据，以在Bizible的归因历程中创建接触点，从而对电子邮件和参与项目进行适当信用。增强了我们的Marketo Engage集成。
* **Marketo Engage活动集成（测试版）**:将Marketo Engage活动数据直接引入Bizible，以在客户历程和所有归因模型中创建接触点。示例包括潜在客户分数更改、有趣时刻、电子邮件点击或任何自定义活动。 增强了我们的Marketo Engage集成。
* **Bizible B2B客户属性集成（测试版）**:这是与Adobe Analytics的Adobe Experience Cloud集成，允许您将选定的Bizible数据直接引入Adobe Analytics中，以便进行更深入的分析。示例包括按公司名称、帐户属性、CRM机会和由Bizible归因收入和漏斗阶段定义的高价值个人，基于帐户的网站流量和内容分析。
* **Bizible Discover过滤器和增强功能**:通过功能板中的渠道、子渠道、营销活动和客户群细分分析数据。使用更多深入分析属性增强数据可见性。 这是对Discover展示板的增强。
* **Microsoft Dynamics的活动同步**:将Microsoft Dynamics CRM活动引入接触点历程，并跟踪与您的潜在客户或联系人关联的呼叫、约会或任务等事件，从而确定销售交互的属性。增强Microsoft Dynamics CRM集成。

## 销售分析 {#sales-insight}

![（星号）](assets/yellow-star.png)

* **[适用于Salesforce CRM的分析功能板](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**:我们正在重新构想我们的销售分析功能，以便能够全面了解即将发生的营销活动和促销活动，从而让销售者能够根据其需求和兴趣，向客户和潜在客户提出更相关的推荐。卖家还可以在时间线内查看联系人和帐户活动，并轻松访问其他活动详细信息。 在[此处](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md)查找有关如何升级包的更多详细信息。

<br> 

## 公告 {#announcements}

* **ITP 2.1+ RTP更新**:由于Safari的Cookie策略发生更改，RTP Cookie在同一域上跨会话跟踪用户的功能将因访客使用的浏览器和浏览器版本而受ITP限制为1天或7天。为此，我们实施了新的Web服务，以允许通过HTTP响应使用Set-Cookie标头来设置RTP Cookie。 有关更多信息，请参见[此处](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603)。

* **批量营销活动基础架构更改**:我们将在今年剩余时间升级批量营销活动服务。这将是一个无缝更新，不会影响任何正在进行的批量营销活动，也不会导致行为发生更改。 无需执行任何操作。 有关更多详细信息，请参阅此[国家帖子](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374)。

## 弃用 {#deprecations}

* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:从Munchkin JS版本159开始，当调用关联潜在客户方法时，浏览器控制台中将记录一个弃用警告，指示该功能将在将来的版本中删除。 完整的弃用计划将在以后的日期公布。

**_产品发布网_** [络研讨会](https://engage.marketo.com/June-Release-2020-On-Demand.html) 观看我们“2020年6月产品发布创新”网络研讨会的录像。

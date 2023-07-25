---
unique-page-id: 37357276
description: 发行说明 — 2020年6月 — Marketo文档 — 产品文档
title: 发行说明 — 2020年6月
exl-id: ffc39c9f-8c0c-45af-8ee6-f58971e230b9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# 发行说明： 2020年6月 {#release-notes-june}

2020年6月版中包含以下功能。 查看Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_** 以下功能将发布于 **2020年6月5日**.

## 核心Marketo Engage {#core-marketo-engage}

* **[预测受众](https://experienceleague.adobe.com/docs/marketo/sky/predictive-audiences/getting-started-with-predictive-audiences.html?lang=en#predictive-audiences)** ![(star)](assets/yellow-star.png)：由Adobe Sensei提供支持的新智能列表和智能营销活动过滤器允许您为电子邮件、事件和网络研讨会营销计划创建AI支持的受众区段。 使用AI可帮助您根据潜在客户注册事件、参加事件或取消订阅的可能性来细分受众。 根据过去的计划构建相似受众以有效地复制以前的成功案例。 通过预测目标跟踪实现转化目标，并获得有关如何优化事件项目的受众区段的建议。
* **批量电子邮件提升** ![(star)](assets/yellow-star.png)：增强了我们的电子邮件营销功能，允许您每小时最多发送300万封批量电子邮件。 我们重新设计了批量营销活动和电子邮件报告处理，以增强电子邮件项目和批量电子邮件营销活动的性能。 这可以缩短发送的前置时间，并缩短完成时间。 按照常规方式设置电子邮件发送，不会增加复杂性。 此增强功能作为产品加载项提供，它还包含一个投放服务启动包、电子邮件投放工具和多个专用IP地址。
* **[Audience与Adobe Experience Cloud (AEC)的集成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**：新的Adobe Experience Cloud (AEC)集成，允许您将Marketo Engage中已知商机的静态列表与多个AEC应用程序同步，以增强现有计划、解锁新用例并编排多渠道营销活动。 此集成包括Adobe Analytics、Adobe Target、Adobe Experience Manager、Adobe Audience Manager和Adobe Advertising Cloud。
* **[项目群成员自定义字段](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md)**：捕获和利用有关项目群成员的自定义字段。 在Marketo Engage表单中使用这些新字段，在项目的成员列表中查看它们，在智能列表过滤器和触发器中使用它们，并将它们包含在新的智能营销活动流量操作中，以增强自动化和更精细的个性化。 这些内容也可以通过UI和API导入和导出。 增强了自定义数据对象和字段功能。
* **描述计划成员**：检索项目群成员元数据，使您能够使用REST API导入和导出项目群成员自定义字段数据。 API的增强功能。
* **[在Microsoft Dynamics中创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/create-task-in-microsoft.md)**：使用基于Marketo Engage中捕获的客户行为的新流量操作，在Microsoft Dynamics中为销售人员创建Task。 增强了我们的本机Microsoft Dynamics CRM集成。
* **获取由列表资源API端点使用的表单**：检索依赖于表单的资源列表。 API的增强功能。
* **通过API设置电子邮件标头**：启用电子邮件标头字段的自动翻译和本地化。 API的增强功能。
* **图像和文件缓存**：我们通过从60秒的缓存中提供图像和文件资源来增强Marketo Engage服务器的稳定性。

## Account-Based Marketing {#account-based-marketing}

![(star)](assets/yellow-star.png)

* **新帐户发现功能现已正式推出**

   * 新帐户发现是对我们的帐户分析功能的增强，使您能够根据AI支持的理想客户配置文件模型为ABM策略发现新的净目标帐户。 查看、选择和导入推荐的新帐户，以及这些帐户基于人工智能的拟合和意图数据指示器。

<br> 

**_整个季度发布_**

以下功能属于非季度周期，将在未来几个月发布。

## Bizible {#bizible}

![(star)](assets/yellow-star.png)

* **Marketo Engage程序集成**：直接从Marketo Engage中提取程序数据，沿Bizible中的归因历程创建接触点，以适当地点数电子邮件和参与程序。 增强了Marketo Engage集成。
* **Marketo Engage活动集成（测试版）**：将Marketo Engage活动数据直接引入Bizible以在客户历程和所有归因模型中创建接触点。 示例包括商机得分更改、有趣的时刻、电子邮件点击或任何自定义活动。 增强了Marketo Engage集成。
* **Bizible B2B客户属性集成（测试版）**：这是与Adobe Analytics的Adobe Experience Cloud集成，可让您将选定的Bizible数据直接引入Adobe Analytics以进行更深入的分析。 示例包括基于帐户的网站流量和按公司名称、帐户属性、CRM机会以及Bizible归因收入和漏斗阶段定义的高价值个人的内容分析。
* **Bizible Discover过滤器和增强功能**：使用各个功能板中的渠道、子渠道、营销活动和区段过滤器分析您的数据。 使用更多深入分析属性增强数据可见性。 这是对我们的Discover Boards的增强。
* **Microsoft Dynamics的活动同步**：通过将Microsoft Dynamics CRM活动引入接触点历程来归因销售互动，并跟踪事件，例如与潜在客户或联系人关联的电话、约会或任务。 增强了Microsoft Dynamics CRM集成。

## 销售分析 {#sales-insight}

![(star)](assets/yellow-star.png)

* **[Salesforce CRM的分析仪表板](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)**：我们通过新的对即将发生的营销活动和营销活动的了解，重新构想了我们的销售洞察功能，使销售商能够根据客户和潜在客户的需求和兴趣提供更相关的推荐。 卖家还可以在时间轴中查看联系人和帐户活动，并轻松访问其他活动详细信息。 查找有关如何升级包的更多详细信息 [此处](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

<br> 

## 公告 {#announcements}

* **ITP 2.1+ RTP更新**：由于对Safari的Cookie策略进行了更改，ITP将根据访客使用的浏览器和浏览器版本，将RTP Cookie在同一域上跨会话跟踪用户的能力限制为1或7天。 为此，我们正在实施一项新的Web服务，以允许通过HTTP响应使用Set-Cookie标头设置RTP Cookie。 可找到更多信息 [此处](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603).

* **批量活动基础架构更改**：我们将在今年剩余时间升级批处理Campaign服务。 这将是一种无缝更新，不会影响任何正在进行的批量活动，也不会导致行为更改。 无需执行任何操作。 在此查找更多详细信息 [国家帖子](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374).

## 弃用 {#deprecations}

* **[Munchkin关联潜在客户](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**：从Munchkin JS版本159版本开始，当调用Associate Lead方法时，浏览器控制台中将记录弃用警告，这表示将在未来版本中删除该功能。  之后将宣布完整的弃用计划。

**_产品发布网络研讨会_** [观看录制](https://engage.marketo.com/June-Release-2020-On-Demand.html) 2020年6月产品发布创新网络研讨会的一个成员。

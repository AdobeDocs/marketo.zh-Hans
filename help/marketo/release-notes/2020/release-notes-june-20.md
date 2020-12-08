---
unique-page-id: 37357276
description: 发行说明- 2020年6月- Marketo Docs —— 产品文档
title: 发行说明- 2020年6月
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 0%

---


# 发行说明：2020年6月 {#release-notes-june}

2020年6月版包含以下功能。 检查您的Marketo版本以了解功能可用性。

>[!NOTE]
>
>**可用性**
>
>由星(（星） ![)表示的特](assets/star-yellow.svg)征可以是付费附加项。 请联系您的Marketo Engage代表以了解更多信息。

***季度版本*** 2020年6月5日将发 **布以下功能**。

## 核心Marketo Engage {#core-marketo-engage}

* **预 [测受众](https://help.marketo.com/hc/en-us/articles/360045746253)![（星形）](assets/star-yellow.svg)

   **:新的智能列表和由Adobe Sensei提供支持的智能活动过滤器使您能够为电子邮件、事件和网络研讨会营销项目创建由人工智能提供支持的受众细分。 使用AI根据潜在客户注册受众、参加事件或取消订阅的可能性帮助您对事件进行细分。 根据过去的受众构建相似项目，以有效复制以前的成功。 通过预测目标跟踪实现转化目标，并获取有关如何为事件项目优化受众细分的建议。
* **批量电子邮件 ![提升（星型）](assets/star-yellow.svg):**增强我们的电子邮件营销功能，使您每小时最多可发送300万封批量电子邮件。 我们重新构建了批量活动和电子邮件报告处理架构，以增强电子邮件项目和批量电子邮件活动的性能。 这会缩短发送的提前期，并改善完成时间。 按照正常方式设置电子邮件发送，不会增加复杂性。 此增强功能可作为产品附加项提供，其中还包括投放服务启动包、电子邮件投放工具和多个专用IP地址。
* **与 [Adobe Experience Cloud(AEC)受众集成](https://docs.marketo.com/x/ogI6Ag):**新的Adobe Experience Cloud(AEC)集成，可让您将Marketo Engage的已知销售线索静态列表与多个AEC应用程序同步，以增强现有项目、释放新用例和编排多渠道活动。 这一整合包括Adobe Analytics、Adobe Target、Adobe Experience Manager、Adobe Audience Manager和Adobe Advertising Cloud。
* **项目 [成员自定义字段](https://docs.marketo.com/x/MQA6Ag)**:捕获并利用有关项目成员的自定义字段。 在您的Marketo Engage表单中使用这些新字段，在项目的成员列表中视图它们，在智能列表过滤器和触发器中利用它们，并将它们纳入新的智能活动流动操作中，以增强自动化和更精细的个性化。 还可以通过UI和API导入和导出这些组件。 增强我们的自定义数据对象和字段功能。
* **描述项目成员**:检索项目成员元数据，使您能够使用REST API导入和导出项目成员自定义字段数据。 增强我们的API*。*

* **在 [Microsoft Dynamics中创建任务](https://docs.marketo.com/x/jQM6Ag)**:根据Marketo Engage中捕获的客户行为，使用新的“流动操作”为Microsoft Dynamics内的销售人员创建任务。 增强我们本机Microsoft Dynamics CRM集成*。*

* **获取列表资产API端点使用的表单**:检索依赖表单的资产列表。 增强我们的API*.*

* **通过API设置电子邮件预头**:启用电子邮件预头字段的自动翻译和本地化。 增强我们的API*.*

* **图像和文件缓存**:我们通过从60秒的缓存提供图像和文件资源来增强Marketo Engage服务器的稳定性。

**基于帐户的营 ![销（星型）](assets/star-yellow.svg)

**

* **通常提供新帐户发现**

   * 新帐户发现是对我们帐户分析功能的增强，使您能够根据基于AI的理想客户目标模型发现ABM战略的新客户帐户。 视图、选择和导入推荐的新帐户，以及基于AI的适应和意图数据指示器。

<br> 

**

***整季度发布***

以下功能在非季度周期中发布，并将在未来几个月中发布。
**可 ![比（星）](assets/star-yellow.svg)

**

* **Marketo Engage项目集成**:直接从Marketo Engage中提取项目数据，在Bizible的归因旅程中创建接触点，为电子邮件和互动项目提供适当信用。 增强我们的Marketo Engage集成。
* **Marketo Engage活动集成`<sup>BETA</sup>`**:将Marketo Engage活动数据直接引入Bizible，在客户旅程和所有归因模型中创建接触点。 示例包括潜在客户得分变化、有趣时刻、电子邮件点击或任何自定义活动。 增强我们的Marketo Engage集成。
* **备见B2B客户属性集成`<sup>BETA</sup>`**:这是Adobe Experience Cloud与Adobe Analytics的集成，允许您将选定的Bizible数据直接引入Adobe Analytics，以进行更深入的分析。 示例包括按公司名称、帐户属性、CRM机会以及由Bizbile归属的收入和漏斗阶段定义的高价值个人，基于帐户的网站流量和内容分析。
* **奇怪的发现过滤器和增强功能：** 利用渠道、子渠道、活动和跨仪表板的细分过滤器分析数据。 利用更多向下钻取属性增强数据可见性。 这是对Discover展示板的增强。
* **活动同步Microsoft Dynamics**:通过将Microsoft Dynamics CRM活动引入接触点旅程并跟踪与您的潜在客户或联系人关联的事件(如呼叫、约会或任务)，确定销售互动的属性。 增强我们的Microsoft Dynamics CRM集成。

**销售 ![分析（星型）](assets/star-yellow.svg)

**

* **针 [对Salesforce CRM的洞察仪表板](https://docs.marketo.com/x/EoGMAg)**:我们正在重新构思销售分析功能，对即将到来的营销事件和活动进行全面了解，使销售者能够根据客户和潜在客户的需求和兴趣提供更具相关性的建议。 销售者还可以在时间轴中视图联系人和帐户活动，并轻松访问其他活动详细信息。 在此处查找有关如何升级包的更多详 [细信息](https://docs.marketo.com/x/F4GMAg)。

<br> 

## 公告 {#announcements}

* **ITP 2.1+ RTP更新**:由于Safari的Cookie策略发生更改，RTP Cookies在同一域上跨会话跟踪用户的能力将受ITP限制为1天或7天，这取决于访客使用的浏览器和浏览器版本。 为此，我们实施了新的Web服务，以允许通过HTTP响应使用Set-Cookie头设置RTP Cookie。 更多信息可在此 [找到](https://nation.marketo.com/t5/Knowledgebase/Browser-Cookie-Updates-How-Marketo-RTP-Is-Affected/ta-p/299603)。

* **批活动基础结构更改**:我们将在今年剩余时间升级批活动服务。 这将是一个无缝更新，不会影响任何正在进行的批活动，不会导致行为发生更改。 无需执行任何操作。 在此国家／地区帖子中查 [找更多详细信息](https://nation.marketo.com/t5/Product-Documents/Batch-Campaign-Processing-Infrastructure-Update/ta-p/301374)。

## 弃用 {#deprecations}

* ** [Munchkin关联潜在客户](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/):**从Munchkin JS的版本159开始，当调用关联潜在客户方法时，浏览器控制台中将记录一个停用警告，表明该功能将在将来的版本中删除。  完全弃用计划将在以后的日期公布。

***产品发布网络研讨会***[观看我们](https://engage.marketo.com/June-Release-2020-On-Demand.html) “2020年6月产品发布创新”网络研讨会的录制。

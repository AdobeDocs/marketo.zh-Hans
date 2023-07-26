---
description: 发行说明 — 2021年5月 — Marketo文档 — 产品文档
title: 发行说明 — 2021年5月
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 0%

---

# 发行说明： 2021年5月 {#release-notes-may-21}

2021年5月版本中包含以下功能。 检查您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_**

以下功能将发布于 **2021年5月7日**.

## 基于帐户的体验 {#Account-based-eaperiences}

* **帐户智能列表（正式发布）** ![](assets/yellow-star.png)：通过跨渠道营销活动中定位所需的帐户和人员属性，动态确定客户并确定其资格，并及时向销售人员发送警报，以便更快地完成交易。 这项新功能允许对基于帐户的营销策略实现强大的自动化功能。 帐户智能列表适用于具有新一代用户体验中的Target帐户管理的客户。

## 新一代用户体验 {#next-generation-user-experience}

通过全局搜索预览，营销人员可以快速查看共享资产在其实例中的位置。 浏览器选项卡显示位置以改进营销活动或设计工作室中的导航。 其他树和全局搜索筛选器有助于优化您的搜索条件。 树中的拖放功能已恢复，允许您在主应用程序区域中快速高效地移动文件夹和资产。 最新更新的图标(符合Adobe的辅助功能标准)和状态徽章允许营销人员在树中快速轻松地区分文件夹和资源，并识别项目和资源的状态。

## 体验自动化 {#experience-automation}

* **执行Campaign流程步骤**：通过“智能营销活动”的新流程步骤，简化营销活动创建工作流并提高营销活动效果。 为工作区中的重复任务（如国家/地区代码标准化）创建和保存集中式模板营销活动，以便通过新的“执行营销活动”流程步骤从任何Smart Campaign调用和运行。 链接的营销活动将以指定顺序运行，并确保任务在进入下一个流程步骤之前完成。 在一个集中式活动中快速编辑流，以更新使用它的每个Smart Campaign来简化数据管理、领导评分和路由工作流。

## 跨渠道编排 {#cross-channel-orchestration}

* **Forms中的敏感数据字段**：通过将数据字段定义为敏感字段并限制这些字段的表单预填充，Protect客户的个人身份信息(PII)不会显示在Adobe Marketo Engage表单中。 每当访客在登陆页面上查看表单时，定义为敏感的字段将不显示任何预填数据。

* **阻止垃圾邮件表单提交**：Protect您的Adobe Marketo Engage数据库，防止垃圾数据向销售人员发送无效警报、触发促销活动积压并创建不需要的活动。 新的验证机制会拒绝无效的表单提交并阻止机器人攻击。 您的数据更干净，营销活动按预期运行，从而最大限度地降低将不合格的潜在客户推向销售的风险。

* **电子邮件程序审批警告**：防止在对之前批准的程序进行新编辑时发送错误的电子邮件。  当营销人员将更改应用于已批准的电子邮件，但随后忘记批准最新更改时，警告充当护栏，并向没有内容、不良内容或旧内容的大型受众发送电子邮件。

* **过滤掉电子邮件机器人活动**：通过新的电子邮件机器人活动过滤功能防止意外销售警报和不准确的电子邮件报告。 识别并过滤掉可能与电子邮件机器人相关的打开次数和点击次数，检查导致错误触发器和销售警报，或报告不正确的链接。

## API增强功能 {#api-enhancements}

对Bulk API和Lead API进行了几项关键更新，包括能够批量导出自定义对象数据，将公司与潜在客户批量关联，能够根据主要属性筛选批量活动提取，以及能够创建和更新计划成员资格。

* **嵌套事件程序**：在Adobe Marketo Engage中，您可以创建、克隆或移动其他程序类型下的事件程序。 现在允许在assets API中使用此功能。

* **增强删除程序API**：允许集成应用程序删除包含其他类型资源的程序，而无需用户从Adobe Marketo Engage手动执行此操作。

* **计划会员资格**：营销人员可以根据不同的条件（如项目成员状态）查询选定项目的所有项目成员记录。 与外部应用程序、商业智能工具或Adobe Experience Cloud共享此信息，以改进细分并创建更有针对性的参与。

* **批量自定义对象提取**：批量数据导出补充了数据分析师在Adobe Marketo Engage中已有的导入功能。 现在，他们可以批量提取存储在第一级Adobe Marketo Engage自定义对象中的数据，并将该数据加载到其他应用程序、data warehouse或BI(Business Intelligence)工具中，以便更好地了解Adobe Marketo Engage实例中的数据。  自定义对象批量数据移动是双向的，可以在方便的时间进行调度。

* **自定义字段元数据API**：在设置您的Adobe Marketo Engage与第三方应用程序的集成时，通过自动创建自定义字段来节省时间。 这种自动化尤其使具有多个Adobe Marketo Engage实例的客户受益，现在这些客户能够简化自定义字段创建，以前这些字段在每个实例中都需要手动工作。 简化自定义字段创建并节省此资源消耗活动的时间。

* **批量活动提取API**：执行批量提取时，获得对数据量和类型的控制。 过滤掉不必要的数据点并控制批量提取活动数据所需的API调用数。  例如，选择打开的电子邮件、访问网页或更改潜在客户得分，并保留您不希望分析的值中的其他更改。 简化流程，减少API调用和数据清理的次数。

* **潜在客户API**：识别Adobe Marketo Engage中具有AdobeECID(Experience CloudID)的潜在客户。  Adobe Marketo Engage客户可以通过选定的营销活动创建潜在客户列表，并使用ECID(Experience CloudID)在Adobe Analytics中为该特定列表创建报表。 Adobe Marketo Engage与Adobe Experience Cloud之间的集成为分段、定位和报表带来了无限商机。

* **批量商机导入API**：控制批量商机导入及其占用的资源。 此增强功能在批量商机导入过程中在商机与公司之间创建了关联。 如果API调用，则提高处理数据的效率和效率，并减少用量。

* **面向Microsoft Dynamics Online客户的基于Web API的集成**：MS Dynamics Web API随8.0版REST协议引入，实现了OData（开放数据协议）v4。 OData是OASIS （结构化信息标准促进组织）标准，用于在富数据上构建和使用RESTful服务。 需要使用此方法与Microsoft Dynamics集成的Adobe Marketo Engage客户当前正在从SOAP（简单对象访问协议）迁移到基于Web API的连接。

## 营销数据环境 {#marketing-data-environment}

* **XLSX导出**：我们升级了整个产品的导出功能，以支持XLSX而不是XLS。 这意味着在产品中当前支持XLS导出的任何位置，此选项将被替换为导出到XLSX的选项。 此更改将影响Adobe Marketo Engage中报表和其他数据的所有Excel导出的文件名。

* **按潜在客户ID搜索**：快速访问潜在客户数据库或静态列表中按Adobe Marketo Engage潜在客户ID搜索的潜在客户记录。 在“快速查找”窗口中，只需键入 `[id]` ，则将显示潜在客户信息。 用户可以快速查看潜在客户、公司或商机的详细信息。

## Bizible {#bizible}

![](assets/yellow-star.png)

* **与LinkedIn Lead Gen Forms（测试版）集成**：使用Bizible Premium归因解决方案深入了解您的LinkedIn渠道支出和ROI。 通过与LinkedIn的Lead Gen Forms的最新集成，Bizible可深入了解在LinkedIn平台中提交的表单。 这些表单填写会根据您的CRM（客户关系管理）或Adobe Marketo Engage实例中的潜在客户进行匹配，以便他们符合归因条件，并且可以根据您的其他营销参与进行跟踪。

## 公告 {#announcements}

* **Marketo产品文档切换平台**：我们很高兴地宣布，自5月7日星期五起，Marketo产品文档已加入Adobe Experience League。 您仍可以使用URL： docs.marketo.com，如果您有任何已添加书签的现有文章，您将被重定向。 新平台上提供了所有产品文档，并计划在今年晚些时候进行增强。

* **由AdobeIdentity System提供支持的简化用户管理和单点登录**：从2021年7月开始，将使用Adobe用户凭据载入新的Adobe Marketo Engage客户。 在2022年年中之前不会将当前客户迁移到集成的Identity System，在进一步通知之前，无需客户采取任何行动。 通过单点登录，IT/安全管理员可以管理多个Adobe Marketo Engage产品实例及其他Experience Cloud解决方案，并通过通用控制台配置SSO (Shared Services Organization)。 管理员可以通过公共Admin Console方便地管理用户组和用户权限。

**_产品发布网络研讨会_**

[2021年5月Marketo Engage发布网络研讨会](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)

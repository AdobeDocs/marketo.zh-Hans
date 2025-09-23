---
description: 发行说明 — 2021年5月 — Marketo文档 — 产品文档
title: 发行说明 - 2021 年 5 月
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1436'
ht-degree: 1%

---

# 发行说明：2021 年 5 月 {#release-notes-may-21}

2021年5月版本中包含以下功能。 检查您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![](assets/yellow-star.png))表示的功能是付费加载项。 请联系您的 Marketo Engage 代表了解更多信息。

**_季度发布_**

以下功能将于&#x200B;**2021年5月7日发布**。

## 基于帐户的体验 {#Account-based-eaperiences}

* **帐户智能列表（正式发布）** ![](assets/yellow-star.png)：通过跨渠道营销活动中定位的所需帐户和人员属性，动态识别并限定帐户，并及时向销售人员发送警报，以更快地完成交易。 这项新功能允许对基于帐户的营销策略实现强大的自动化功能。 帐户智能列表适用于具有新一代用户体验中的Target帐户管理的客户。

## 新一代用户体验 {#next-generation-user-experience}

通过全局搜索预览，营销人员可以快速查看共享资产在其实例中的位置。 浏览器选项卡显示位置以改进[!UICONTROL Marketing Activities]或[!UICONTROL Design Studio]中的导航。 其他树和全局搜索筛选器有助于优化您的搜索条件。 树中的拖放功能已恢复，允许您在主应用程序区域中快速高效地移动文件夹和资产。 最新更新的图标(符合Adobe的辅助功能标准)和状态徽章允许营销人员在树中快速轻松地区分文件夹和资源，并识别项目和资源的状态。

## 体验自动化 {#experience-automation}

* **执行营销活动流程步骤**：通过智能营销活动的新流程步骤，简化营销活动创建工作流并提高营销活动效果。 为工作区中的重复任务（如国家/地区代码标准化）创建和保存集中式模板营销活动，以便通过新的“执行营销活动”流程步骤从任何Smart Campaign调用和运行。 链接的营销活动将以指定顺序运行，并确保任务在进入下一个流程步骤之前完成。 在一个集中式活动中快速编辑流，以更新使用它的每个Smart Campaign来简化数据管理、领导评分和路由工作流。

## 跨渠道编排 {#cross-channel-orchestration}

* **Forms中的敏感数据字段**：通过将数据字段定义为敏感字段，并限制这些字段的表单预填充，保护客户的个人身份信息(PII)不显示在Adobe Marketo Engage表单中。 每当访客在登陆页面上查看表单时，定义为敏感的字段将不显示任何预填数据。

* **阻止垃圾邮件表单提交**：保护您的Adobe Marketo Engage数据库，使其免受垃圾数据的攻击，这些垃圾数据可能会导致向销售人员发出无效警报、触发营销活动积压并创建不需要的活动。 新的验证机制会拒绝无效的表单提交并阻止机器人攻击。 您的数据更干净，营销活动按预期运行，从而最大限度地降低将不合格的潜在客户推向销售的风险。

* **电子邮件项目批准警告**：在对先前批准的项目进行新编辑时，阻止发送错误的电子邮件。  当营销人员将更改应用于已批准的电子邮件，但随后忘记批准最新更改时，警告充当护栏，并向没有内容、不良内容或旧内容的大型受众发送电子邮件。

* **过滤掉电子邮件机器人活动**：通过新的电子邮件机器人活动过滤功能防止意外销售警报和不准确的电子邮件报告。 识别并过滤掉可能与电子邮件机器人相关的打开次数和点击次数，检查导致错误触发器和销售警报，或报告不正确的链接。

## API增强功能 {#api-enhancements}

对Bulk API和Lead API进行了几项关键更新，包括能够批量导出自定义对象数据，将公司与潜在客户批量关联，能够根据主要属性筛选批量活动提取，以及能够创建和更新计划成员资格。

* **嵌套事件程序**：在Adobe Marketo Engage中，可以在其他程序类型下创建、克隆或移动事件程序。 现在允许在assets API中使用此功能。

* **增强删除程序API**：允许集成应用程序删除包含其他资源类型的程序，而无需用户从Adobe Marketo Engage手动执行此操作。

* **计划成员资格**：营销人员可以根据不同的条件（如计划成员状态）查询选定计划的所有计划成员记录。 与外部应用程序、商业智能工具或Adobe Experience Cloud共享此信息，以改进细分并创建更有针对性的参与。

* **批量自定义对象提取**：批量数据导出补充了数据分析人员在Adobe Marketo Engage中已有的导入功能。 现在，他们可以批量提取存储在第一级Adobe Marketo Engage自定义对象中的数据，并将该数据加载到其他应用程序、数据仓库或BI (Business Intelligence)工具中，以便更好地了解Adobe Marketo Engage实例中的数据。  自定义对象批量数据移动是双向的，可以在方便的时间进行调度。

* **自定义字段元数据API**：在设置您的Adobe Marketo Engage与第三方应用程序的集成时，通过自动创建自定义字段来节省时间。 这种自动化尤其使具有多个Adobe Marketo Engage实例的客户受益，现在这些客户能够简化自定义字段创建，以前这些字段在每个实例中都需要手动工作。 简化自定义字段创建并节省此资源消耗活动的时间。

* **批量活动提取API**：在执行批量提取时获得对数据量和类型的控制。 过滤掉不必要的数据点并控制批量提取活动数据所需的API调用数。  例如，选择打开的电子邮件、访问网页或更改潜在客户得分，并保留您不希望分析的值中的其他更改。 简化流程，减少API调用和数据清理的次数。

* **潜在客户API**：识别Adobe Marketo Engage中与Adobe ECID (Experience Cloud ID)关联的潜在客户。  Adobe Marketo Engage客户可以通过选定的营销活动创建潜在客户列表，并使用ECID (Experience Cloud ID)在Adobe Analytics中为该特定列表创建报表。 Adobe Marketo Engage与Adobe Experience Cloud之间的集成为分段、定位和报表带来了无限商机。

* **批量潜在客户导入API**：控制批量潜在客户导入及其使用的资源。 此增强功能在批量商机导入过程中在商机与公司之间创建了关联。 如果API调用，则提高处理数据的效率和效率，并减少用量。

* 针对&#x200B;**客户的[!DNL Microsoft Dynamics Online]基于Web API的集成**： [!DNL MS Dynamics] Web API是通过8.0 REST协议引入的，并且实现了OData（开放数据协议）v4。 OData是OASIS （结构化信息标准促进组织）标准，用于在富数据上构建和使用RESTful服务。 需要使用此方法与[!DNL Microsoft Dynamics]集成的Adobe Marketo Engage客户当前正在从SOAP (Simple Object Access Protocol)迁移到基于Web API的连接。

## 营销数据环境 {#marketing-data-environment}

* **XLSX导出**：我们升级了整个产品的导出功能，以支持XLSX而不是XLS。 这意味着在产品中当前支持XLS导出的任何位置，此选项将被替换为导出到XLSX的选项。 此更改将影响Adobe Marketo Engage中报表和其他数据的所有Excel导出的文件名。

* **按潜在客户ID搜索**：快速访问在潜在客户数据库或静态列表中按Adobe Marketo Engage潜在客户ID搜索的潜在客户记录。 在“快速查找”窗口中，只需键入具有相应编号的`[id]`即可，然后将显示潜在客户信息。 用户可以快速查看潜在客户、公司或商机的详细信息。

## Bizible {#bizible}

![](assets/yellow-star.png)

* **与[!DNL LinkedIn] Lead Gen Forms (Beta)集成**：通过Bizible Premium归因解决方案深入了解您的[!DNL LinkedIn]渠道支出和ROI。 通过与[!DNL LinkedIn]的Lead Gen Forms的最新集成，Bizible将insight纳入已在[!DNL LinkedIn]平台中提交的表单中。 这些表单填写会根据您的CRM（客户关系管理）或Adobe Marketo Engage实例中的潜在客户进行匹配，以便他们符合归因条件，并且可以根据您的其他营销参与进行跟踪。

## 公告 {#announcements}

* **Marketo产品文档切换平台**：我们很高兴地宣布，从5月7日星期五起，Marketo产品文档已加入Adobe Experience League。 您仍可以使用URL： docs.marketo.com，如果您有任何已添加书签的现有文章，您将被重定向。 新平台上提供了所有产品文档，并计划在今年晚些时候进行增强。

* **由Adobe Identity System提供支持的简化用户管理和单点登录**：从2021年7月开始，将使用Adobe Marketo Engage用户凭据登记新的Adobe客户。 在2022年年中之前不会将当前客户迁移到集成的Identity System，在进一步通知之前，无需客户采取任何行动。 通过单点登录，IT/安全管理员可以管理多个Adobe Marketo Engage产品实例及其他Experience Cloud解决方案，并通过通用控制台配置SSO (Shared Services Organization)。 管理员可以通过公共Admin Console方便地管理用户组和用户权限。

**_产品发布网络研讨会_**

[2021年5月Marketo Engage发布网络研讨会](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)

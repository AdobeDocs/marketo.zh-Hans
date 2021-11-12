---
description: 发行说明 — 2021年5月 — Marketo文档 — 产品文档
title: 发行说明 — 2021年5月
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
source-git-commit: 115b6e97978778a1d1e13478adf6fee625aa5257
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 0%

---

# 发行说明：2021年5月 {#release-notes-may-21}

’21年5月版中包含以下功能。 查看您的Marketo版本以了解功能的可用性。

>[!AVAILABILITY]
>
>由星(![](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_**

将在 **2021年5月7日**.

## 基于帐户的体验 {#Account-based-eaperiences}

* **帐户智能列表（正式发布）** ![](assets/yellow-star.png):动态识别具有所需帐户和人员属性的帐户并确定其资格，以便在跨渠道营销活动中进行定位，并及时向销售人员发送警报，以便更快地完成交易。 这项新功能可实现基于帐户的营销策略的强大自动化。 具有Target帐户管理的客户在下一代用户体验中可以使用帐户智能列表。

## 新一代用户体验 {#next-generation-user-experience}

通过全局搜索预览，营销人员可以快速查看共享资产在其实例中的位置。 浏览器选项卡会显示相应位置，以改进营销活动或Design Studio中的导航。 其他树和全局搜索过滤器有助于优化搜索标准。 恢复了树中的拖放功能，允许您在主应用程序区域内快速高效地移动文件夹和资产。 新更新的图标(符合Adobe的辅助功能标准)和状态徽章允许营销人员在树中快速轻松地区分文件夹和资产，并识别程序和资产的状态。

## 体验自动化 {#experience-automation}

* **执行营销活动流程步骤**:通过智能营销活动的新流程步骤，简化营销活动创建工作流程并提高营销活动性能。 在工作区中为重复任务创建并保存集中的模板营销活动（如国家/地区代码标准化），以便通过新的“执行营销活动”流程步骤从任何智能营销活动中调用和运行。 链接的营销活动将按指定顺序运行，并确保任务在进入下一个流程步骤之前完成。 在一个集中的营销活动中快速编辑流程，以更新每个使用该流程的智能营销活动，从而简化数据管理、商机评分和路由工作流程。

## 跨渠道编排 {#cross-channel-orchestration}

* **Forms中的敏感数据字段**:Protect客户的个人身份信息(PII)无法在AdobeMarketo Engage表单中显示，方法是将数据字段定义为敏感字段，并限制对这些字段进行表单预填。 每当访客在登陆页面上查看表单时，定义为敏感字段将不会显示任何预填充数据。

* **阻止垃圾邮件表单提交**:Protect您的AdobeMarketo Engage数据库会从垃圾数据中删除，这些数据可能会导致销售人员收到无效警报、触发营销活动积压，以及创建不需要的活动。 新的验证机制拒绝无效的表单提交并停止机器人攻击。 您的数据更简洁，并且您的营销活动按预期运行，从而最大限度地降低向销售发送不合格销售线索的风险。

* **电子邮件程序批准警告**:在对之前批准的程序进行新编辑时，请防止发送错误的电子邮件。  当营销人员对已批准但随后忘记批准最新更改的电子邮件进行更改，并将电子邮件发送给没有内容、内容不正确或内容不为旧的大量受众时，此警告将充当护栏。

* **过滤掉电子邮件机器人活动**:通过新的电子邮件机器人活动过滤功能，防止意外的销售警报和不准确的电子邮件报告。 识别并过滤掉可能与电子邮件机器人关联的打开数和点击数，这些机器人会检查导致虚假触发器和销售警报或报表不正确的链接。

## API增强功能 {#api-enhancements}

对批量API和潜在客户API进行了几项重要更新，包括能够批量导出自定义对象数据，将公司与潜在客户批量关联，能够根据主属性过滤批量活动提取，以及能够创建和更新程序成员资格。

* **嵌套事件程序**:在“Adobe”Marketo Engage中，您可以在其他程序类型下创建、克隆或移动事件程序。 现在，资产API中允许使用此功能。

* **增强的删除程序API**:允许集成应用程序删除包含其他类型资产的程序，而无需用户从AdobeMarketo Engage中手动删除。

* **计划会员资格**:营销人员可以查询给定不同标准（如项目成员状态）的选定项目的所有项目成员记录。 与外部应用程序、业务智能工具或Adobe Experience Cloud共享此信息，以改进客户细分并创建更具针对性的参与。

* **批量自定义对象提取**:批量数据导出补充了数据分析人员在AdobeMarketo Engage中已经享受的导入功能。 现在，他们可以批量提取存储在第1级AdobeMarketo Engage自定义对象中的数据，将此数据加载到其他应用程序、data warehouse或BI(Business Intelligence)工具中，以便更好地分析AdobeMarketo Engage实例中的数据。  自定义对象批量数据移动是双向的，并且可以在方便的时间安排。

* **自定义字段元数据API**:在设置与第三方应用程序的AdobeMarketo Engage集成时，通过自动创建自定义字段来节省时间。 此自动化尤其使具有多个AdobeMarketo Engage实例的客户受益，这些客户现在能够简化自定义字段的创建过程，这些自定义字段过去要求在每个实例中进行手动工作。 简化自定义字段的创建过程，并节省此资源消耗活动的时间。

* **批量活动提取API**:执行批量提取时，获取对数据量和类型的控制。 过滤掉不必要的数据点，并控制批量提取活动数据所需的API调用数量。  例如，选择打开的电子邮件、访问网页或更改潜在客户分数，并保留您不希望分析的其他值更改。 简化该流程，以减少API调用和数据清理的数量。

* **潜在客户API**:识别AdobeMarketo Engage中与AdobeECID(Experience CloudID)关联的潜在客户。  AdobeMarketo Engage客户可以从选定的促销活动中创建潜在客户列表，并使用ECID(Experience CloudID)在Adobe Analytics中为该特定列表创建报表。 AdobeMarketo Engage与Adobe Experience Cloud之间的集成，为细分、定位和报告提供了无限的机会。

* **批量潜在客户导入API**:控制批量潜在客户导入和所需资源。 此增强功能可在批量潜在客户导入过程中创建潜在客户与公司之间的关联。 在API调用中提高处理数据的效率并减少使用。

* **面向Microsoft Dynamics Online客户的基于Web API的集成**:MS Dynamics Web API是在8.0版REST协议中引入的，实现了OData(Open Data Protocol)v4。 OData是OASIS（提高结构化信息标准组织）标准，用于通过丰富数据构建和消费RESTful服务。 需要使用此方法与Microsoft Dynamics集成的AdobeMarketo Engage客户当前正从SOAP（简单对象访问协议）迁移到基于Web API的连接。

## 营销数据环境 {#marketing-data-environment}

* **XLSX导出**:我们升级了整个产品的导出功能，以支持XLSX而不是XLS。 这意味着当前支持XLS导出的产品中的任何位置，此选项将替换为导出到XLSX的选项。 此更改将影响所有Excel导出的报表及AdobeMarketo Engage中的其他数据的文件名。

* **按潜在客户ID搜索**:通过潜在客户数据库或静态列表中的AdobeMarketo Engage潜在客户ID快速访问潜在客户记录搜索。 在“快速查找”窗口中，只需键入 `[id]` 并显示相应的数字，则显示潜在客户信息。 用户可以快速查看潜在客户、公司或商机详细信息。

## Bizible {#bizible}

![](assets/yellow-star.png)

* **与LinkedIn Lead Gen Forms（测试版）集成**:通过Bizible高级归因解决方案，深入了解您的LinkedIn渠道支出和ROI。 通过与LinkedIn的Lead Gen Forms的最新集成，Bizible对LinkedIn平台内已提交的表单有了深入的了解。 这些表单填充会与您的CRM（客户关系管理）或AdobeMarketo Engage实例中的潜在客户进行匹配，以便他们有资格进行归因，并且可以根据您的其他营销活动进行跟踪。

## 公告 {#announcements}

* **Marketo产品文档切换平台**:我们很高兴地宣布，Marketo产品文档已从5月7日星期五起加入Adobe Experience League。 您仍然能够使用URL:docs.marketo.com中，如果您有任何现有文章添加了书签，您将被重定向。 所有产品文档都在新平台上提供，并计划在今年晚些时候进行增强。

* **由Adobe身份系统提供支持的简化的用户管理和单点登录**:从2021年7月起，将使用Adobe用户凭据载入新的AdobeMarketo Engage客户。 到2022年年中，才会将当前客户迁移到集成身份系统，在进一步通知之前，无需客户采取任何操作。 通过单点登录，IT/安全管理员可以管理多个AdobeMarketo Engage产品实例以及其他Experience Cloud解决方案，并通过通用控制台配置单点登录（Shared Services组织）。 管理员可以通过通用Admin Console方便地管理用户组和用户权限。

**_产品发行网络研讨会_**

[2021年5月版Marketo Engage网络研讨会](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)

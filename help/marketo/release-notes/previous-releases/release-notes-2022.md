---
title: "2022"
description: 2022 - Marketo文档 — 产品文档
feature: Release Information
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
  - id: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 1e70b9383bf3a1cd30715df4379d440c4efb1abd
workflow-type: tm+mt
source-wordcount: 4254
ht-degree: 6%

---

# 2022

## 2022 年 1 月 {#january}

2022年1月版中包含以下功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。 请联系您的 Marketo Engage 代表了解更多信息。

**_季度发布_**

以下功能将于&#x200B;**2022年1月21日**&#x200B;开始发布，并在接下来的几周内分阶段推出每个功能（除非另有说明）。

## 新一代体验

* **更新了新一代体验中的Screens**：我们将在新一代体验中提供其他更新的屏幕，这些屏幕提供了可通过切换开关访问的最新设计和可用性增强功能：

   * [!UICONTROL Design Studio]中的登陆页面资产详细信息
   * [!UICONTROL Marketing Activities]中的登陆页面资产详细信息

## [!DNL Microsoft Dynamics]集成 {#microsoft-dynamics-integration}

* **多选选项集字段类型的同步功能一般可用**：同步来自[!DNL Microsoft Dynamics]的多选选项集字段类型，以便在智能列表和智能营销活动中利用它们，以实现更精细的受众定位。 示例包括：主题/感兴趣的产品、首选通信模式等。 此新同步可用于[!DNL Microsoft Dynamics]版本9.X（包括Dynamics 365 Online）。

* **用于[!DNL Microsoft Dynamics 365 Online]**&#x200B;的Server to Server身份验证：为了提高安全性，我们现在将支持Server to Server (S2S)作为Azure Active Directory上Marketo Engage同步用户的附加身份验证模式，以便以非交互方式访问[!DNL Microsoft Dynamics 365 Online]。 这允许您采用多重身份验证，因为所有身份验证和登录都将基于OAuth（仅客户端ID和客户端密码）。

>[!NOTE]
>
>S2S模式基于“应用程序用户”而非“许可用户”，这节省了使用额外的许可证。

## 管理 {#administration}

* **[表单验证规则](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**：保持数据库的运行状况，能够阻止有问题或不适当的电子邮件域提交Marketo Engage表单。 “全局表单验证规则”面板允许管理员定义阻止列表或启用要阻止表单的免费使用者域的预定义列表。

* **[登陆页面标头安全性](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**：管理员可以管理其登陆页面域上的严格传输安全性和X-Frame Options标头，以强制实施严格的安全要求。

**_在整个季度中发布_**

以下功能采用非季度周期，并将在未来几个月发布。

## AEP Marketo Engage目标连接器 — 创建全新潜在客户 {#aep-marketo-engage-destination-connector}

同时使用Adobe Experience Platform (AEP)的Marketo Engage客户可以最大限度地利用其数据库，通过AEP目标连接器将全新人员记录从AEP推送到Marketo Engage。 将受众区段从AEP发送到Marketo Engage时，区段中尚不存在于Marketo Engage数据库[中的人员会自动添加到该区段中](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md)。

## [!DNL Sales Insight]

![（星形）](assets/yellow-star.png)

[!DNL Salesforce] CRM **的**&#x200B;[!DNL Sales Insight]

* **适用于[!UICONTROL Best Bets]**&#x200B;的新类型列：销售商将通过标记为“类型”的新列快速获得见解，以区分[!UICONTROL Best Bets]页面上的潜在客户和联系人。

* **[!DNL Salesforce]平台API更新**：为响应[!DNL Salesforce]弃用[!DNL Salesforce]平台API版本21.0到30.0，[!DNL Sales Insight]包已更新为最新的API。

* **已更新品牌**：正在更新所有[!DNL Sales Insight]页面，以与Adobe品牌保持一致。

[!DNL Microsoft Dynamics]&#x200B;**的**&#x200B;[!DNL Sales Insight]

* **更新了帐户布局**：销售人员可以获取热门活动的集体视图，例如：电子邮件活动、Web活动、有趣的时刻以及帐户中所有联系人的得分更改。

## [!DNL Sales Connect]

![（星形）](assets/yellow-star.png)

* **致电结果和原因**：通过新的、完全自定义的致电结果和致电原因选项，更详细地了解和跟踪您的销售团队的出站努力。 除了这些新字段外，我们还将引入新的治理功能以强制在销售者进行呼叫时选择呼叫原因和结果，引入新的治理功能以启用或禁用呼叫原因和结果，并引入新的呼叫原因和呼叫结果[!DNL Salesforce]活动自定义字段以将数据记录到[!DNL Salesforce]。 [单击此处](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812)了解更多信息。

* **[!DNL Salesforce]活动详细信息自定义**：当销售活动从[!DNL Sales Connect]登录到[!DNL Salesforce]时，通过自定义添加到[!DNL Salesforce]任务主题字段中的信息，在[!DNL Salesforce]中捕获更多销售活动和任务数据。 [单击此处](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819)了解更多信息。

## 公告

* **弃用Marketo Sky**：在3月，Marketo Sky将不再可用，因为我们的资源侧重于提供新一代用户体验。 为了保持对Marketo Sky目前独有的功能的访问权限，我们将在3月份将资产到期和智能营销活动优先级覆盖引入主流体验。 [单击此处](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33)了解更多信息。

* **表单端点弃用**：Marketo Engage表单将拒绝不支持的对leadCapture/save2端点的程序化表单POST。 [单击此处](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631)了解更多信息。

* **在“邀请用户”对话框中登录**：在3月份，将弃用现有的可选“在“邀请用户”对话框中登录”功能。 功能“[!UICONTROL Login in Invite User Dialog]”被通用ID功能覆盖，即将推出的Adobe Identity Management系统集成需要该功能，并且已于2021年8月在所有订阅中启用。 作为弃用的结果，Marketo Engage将强制在订阅中每个电子邮件地址仅关联一个用户。

**Marketo Engage域 — [!DNL Sales Insight]配置**：对于未配置SSL证书和https://的Marketo Engage域，调用将失败，并出现SSL握手错误。 因此，这些领域将会被淘汰。 因此，使用指向这些域中任何域的旧配置的[!DNL Sales Insight]用户可能在其Lead、Contact、Account、Opportunity Panels或Marketo Global页面上遇到系统标注错误。 如果您遇到此错误，我们建议您在[!DNL Salesforce]中更新[Marketo Engage配置](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)。 您只需要更新文档中突出显示“[!DNL Marketo Sales Insight]配置”部分的Marketo Engage凭据。

**_产品发布网络研讨会_**

[2022年1月Marketo Engage发布网络研讨会](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)

## 2022 年 3 月 {#march}

2022年3月版中包含以下功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。 请联系您的 Marketo Engage 代表了解更多信息。

**_季度发布_**

以下功能将于&#x200B;**2022年3月11日**&#x200B;开始发布，并在接下来的几周内分阶段推出每个功能（除非另有说明）。

## 跨渠道编排

* **[!DNL Dynamic Chat]**：通过主动、主动和1:1次个性化对话，将潜在客户和客户都定位到一起，从而最大限度地利用您网站上的每一个机会。 [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}允许Marketo Engage用户开始将聊天用作B2B营销和销售用例的集成式跨渠道体验的关键部分。 功能包括：直接在聊天中预约会议、潜在客户路由、入门模板、拖放式对话创建等。 Dynamic Chat包含在所有Marketo Engage包中，并将于今年向所有Marketo Engage用户推出。

* **电子邮件机器人活动筛选增强功能**：作为以前发布的[电子邮件机器人活动筛选](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}功能的增强功能，您现在可以选择加入标识为机器人的日志记录活动。 然后，您可以根据被识别为机器人正在执行的活动过滤和触发操作。

## 新一代体验

* **更新了新一代体验中的Screens**：我们将在新一代体验中提供其他更新的屏幕，这些屏幕提供了可通过切换开关访问的最新设计和可用性增强功能：

   * [!UICONTROL Design Studio]中的表单列表视图（包括新的批量操作）

* **导入程序工作流更新**：导入程序工作流将在下一代体验中交付，并包含更新的设计和可用性增强功能。 这将是一个无需切换开关的自动更改。

* **下一代体验切换开关的管理员控制**：以适合用户的方式管理下一代体验的推出，管理员能够选择哪些用户类型可以访问切换开关。

## 体验自动化

* **自助流程步骤(Beta)**：扩展Marketo Engage与栈栈其他部分之间的连接，能够创作自定义的流程步骤以用于Smart Campaigns。 Marketo用户和合作伙伴都可以利用此功能，允许以批量方式使用外部Web服务并执行营销活动，而不使用Webhook，后者只能用于触发营销活动。

* **资产到期**：保持对时间敏感资产和营销活动的控制，并能够在经典用户体验中的指定日期和时间计划其自动停用。

* **智能营销活动优先级覆盖**：确保高优先级触发器智能营销活动尽快执行，并能够覆盖标准营销活动优先级排名。 低优先级触发器智能营销活动也可以优先级降低，以便为其他高优先级任务释放处理资源。

## API增强功能

* **返回禁用电子邮件的打开跟踪状态**：允许通过API读取电子邮件的打开跟踪状态
* **从电子邮件检索动态内容主题行**：允许营销人员在BI工具中执行动态主题行分析
* **项目群成员自定义字段CRUD**：允许营销人员以编程方式创建项目群成员自定义字段
* **批量自定义对象导出更新于Filter**：允许营销人员以编程方式同步自定义对象
* **公开电子邮件程序的“抢先计划”设置**：允许营销人员通过API配置具有抢先计划的电子邮件程序
* **选择性项目标签更新**：允许营销人员推送选择性标签更新，而无需同时推送所有标签
* **批量活动提取actionResult字段**：允许营销人员识别哪些活动被跳过或失败

**_在整个季度中发布_**

以下功能采用非季度周期，并将在未来几个月发布。

## [!DNL Bizible] {#bizible}

![（星形）](assets/yellow-star.png)

* **BI模板**： [!DNL Bizible]现在将为Tableau和Power BI提供可下载的基础报表工件和示例报表，以便快速开发针对您的特定业务需求定制的自定义报表。

## [!DNL Sales Connect]

![（星形）](assets/yellow-star.png)

* **电子邮件连接限制(GA)**：电子邮件连接限制允许[!DNL Sales Connect]管理员在使用Gmail或[!DNL Exchange]作为投放渠道时配置电子邮件的发送速率，以便将电子邮件传递给投放渠道提供商的速率不超过强制的限制。

## 公告

* **弃用Marketo Sky**：在3月，Marketo Sky将不再可用，因为我们的资源侧重于提供新一代用户体验。 为了保持对Marketo Sky目前独有的功能的访问权限，我们在Classic体验中引入了资产到期和智能营销活动优先级覆盖。 [单击此处](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33)了解更多信息。

**_产品发布网络研讨会_**

[2022年3月和5月Marketo Engage发布网络研讨会](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## 2022 年 5 月 {#may}

在下方，您会找到2022年5月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。 请联系您的 Marketo Engage 代表了解更多信息。

**_季度发布_**

以下功能将于&#x200B;**2022年5月6日**&#x200B;开始发布，并在接下来的几周内分阶段推出剩余功能（除非另有说明）。

## 本机CRM集成 {#native-crm-integration}

**[本机Veeva CRM集成](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} （限量发布）**：通过本机集成在Veeva CRM和Marketo Engage之间同步活动，从而改善与医疗保健专业人员的互动。 此集成允许营销人员为医疗保健专业人员创建更加个性化且无缝的跨渠道体验。 如果您有兴趣参与，请联系您的客户成功经理。

## 跨渠道编排

**针对[!DNL Dynamic Chat]**&#x200B;的聊天机器人事件：利用更详细的Web访客行为数据（如页面逗留时间、网站逗留时间和页面滚动百分比）来定义何时应显示聊天对话框。

**PDF为[!DNL Dynamic Chat]**&#x200B;嵌入：通过将PDF嵌入聊天对话框以及通过参与活动跟踪衡量内容性能，提高参与度并共享有意义的内容。

**针对[!DNL Dynamic Chat]**&#x200B;的扩展语言支持： [!DNL Dynamic Chat]用户界面现在还将提供法语、德语、日语、葡萄牙语和西班牙语版本。 也可以用这些语言配置聊天对话框。

**排除[!DNL Dynamic Chat]**&#x200B;的URL：控制您的网页[!DNL Dynamic Chat]中的哪些网页能够排除定位条件中的特定URL。

**[电子邮件机器人活动过滤增强功能](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**：除了现有的IAB列表匹配标识之外，还能够基于隐藏链接用户代理或IP和邻近关系模式来识别机器人行为，继续保护数据库的运行状况。 查看机器人活动统计信息，以便您了解针对每种类型标识的机器人活动数。

电子邮件跟踪链接的&#x200B;**[STS标头](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**：符合安全最佳实践，能够应用Secure Transport Security标头，以确保跟踪链接的流量始终安全。

## 新一代体验

**切换开关默认为新一代体验**：切换开关将在所有可用屏幕中都默认为新体验，使用户更容易发现更新的设计和可用性增强功能。

**更新了下一代体验中的屏幕**：

我们在[!UICONTROL Design Studio]内提供了新一代体验中的电子邮件模板详细信息视图，提供了更新的设计和可用性增强功能，可通过切换开关访问。

## 体验自动化

**自助服务流程步骤（继续测试版）**：扩展Marketo Engage与栈栈其他部分之间的连接，并能够创作自定义流程步骤以用于Smart Campaigns。 Marketo Engage用户和合作伙伴都可以利用此功能，允许在触发、批量和可执行的营销活动中使用外部Web服务（与只能在触发营销活动中使用的Webhook不同）。

## API增强功能

* **为启用了CRM的订阅扩展API访问**：我们正在为启用了CRM同步的订阅扩展API访问，以允许用户从Marketo Engage检索公司、商机和销售人员。
* **支持Forms中的“隐藏”数据类型**：提供通过API管理隐藏表单字段的功能。
* **通过Rules支持isNot表单的多个比较值**：根据另一个字段的值是否不是给定列表中的值之一来管理表单字段的可见性。
* **允许单独设置选择列表中的显示值和提交值**：单独设置字段中的显示值和提交值。 例如，显示酒店的名称，但向后端提交内部ID。
* **允许在“创建或更新电子邮件”时禁用“打开跟踪”设置**：创建禁用了打开跟踪的电子邮件。

## 公告

**电子邮件验证和唯一性**：从4月开始，将开始推出电子邮件验证。 届时，Marketo Engage用户电子邮件地址将需要验证和唯一性（这不适用于仅API用户）。 当目录服务认证用户的订阅启用了电子邮件验证时，该用户将自动验证其电子邮件。

使用&quot;[!UICONTROL Login in Invite User Dialog]&quot;功能订阅的电子邮件验证或只有一封电子邮件与多个用户关联的订阅的电子邮件验证将与5月版本一致。 如果订阅只有一个与多个用户关联的电子邮件，则会启用电子邮件验证，并将要求这些用户解决冲突并为每个用户使用唯一的电子邮件。 启用“在邀请用户对话框中登录”功能后，通过此功能邀请的用户将需要具有唯一的电子邮件地址。 对于通过此功能邀请的仅API用户，电子邮件地址不需要是唯一的。

**存档文件夹行为更改**：在此版本中，将无法再从树上下文菜单中使用在存档文件夹中创建新资源的功能。 用于创建新资产的菜单选项将对所有资产隐藏。 [在此处了解详情](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}。

**_产品发布网络研讨会_**

[2022年3月和5月Marketo Engage发布网络研讨会](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## 2022 年 6 月 {#june}

在下方，您会找到2022年6月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。 请联系您的 Marketo Engage 代表了解更多信息。

以下功能将于&#x200B;**2022年6月24日**&#x200B;开始发布，并在接下来的几周内分阶段推出剩余功能（除非另有说明）。

## 营销数据环境

* **公开自定义对象的CreatedAt/UpdatedAt字段**：让您能够在“人员详细信息”屏幕中检查这些字段，以获取额外的insight。

## 跨渠道编排

* **已改进[!DNL Dynamic Chat]**&#x200B;的流Designer可用性：无需拖放，即可直接从Designer流画布添加信息卡。 [!DNL Dynamic Chat]界面也已得到改进，可更好地显示各个信息卡中的内容。

* [!DNL Dynamic Chat]&#x200B;**的**&#x200B;高级约会路由规则： [!DNL Dynamic Chat]为目标约会路由提供了更多选项。 指定应根据Marketo Engage属性路由哪些座席约会，确保将潜在客户路由到适当的座席。

* **适用于[!DNL Dynamic Chat]**&#x200B;的高级对话框报表：使用参与和转化量度的全新数据可视化图表，更详细地查看[!DNL Dynamic Chat]营销活动的性能。

* **取消同步[!DNL Dynamic Chat]**&#x200B;的未使用Marketo Engage属性：取消同步未使用的[!DNL Dynamic Chat]订阅中的Marketo Engage属性，这有助于促进数据清理，并可以根据需要同步替代属性。

## 下一代体验

**新的切换开关视图**：以下视图现在可在下一代体验中使用：

* [电子邮件详情视图](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [电子邮件列表视图](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## 体验自动化

* **全局表单字段验证规则排除**：从全局表单验证规则中排除特定表单，以便订阅中心和其他关键业务工作流可以接受所有值。

* **自助流程步骤**：扩展Marketo Engage与栈栈其他部分之间的连接，并能够创作自定义流程步骤以用于Smart Campaigns。 Marketo Engage用户和合作伙伴都可以利用此功能，允许在“触发器”、“批处理”和“可执行”营销活动中使用外部Web服务，而相比之下，Webhook只能在“触发器”营销活动中使用。

* **与Munchkin协议无关的链接跟踪**：通过Munchkin扩展对`tel`和`mailto`链接的跟踪支持，以跟踪扩展的Web行为集。

* **Webhook的其他HTTP方法**：将PUT、PATCH和DELETE指定为与Web服务交互的请求类型。

## [!DNL Sales Insight]

![（星形）](assets/yellow-star.png)

* **[!DNL Sales Insight]在[!DNL Salesforce]**&#x200B;中设置的权限：管理员可以通过Marketo应用程序权限集向用户级别上的有限用户集合提供[!DNL Sales Insight]访问权限，而不是配置文件级别上的有限用户集合，该权限集是[!DNL Sales Insight] [!DNL Salesforce]包的一部分。

* **我的Marketo拼贴更新 — [!DNL Sales Insight]操作**： Marketo管理员（以及他们指定的用户）现在可以通过位于“我的Marketo”页面上的新[!DNL Sales Insight]操作拼贴快速导航到他们的[!DNL Sales Insight]操作实例。

## [!DNL Sales Connect]

![（星形）](assets/yellow-star.png)

* **[!DNL Salesforce]API更新**：在[!DNL Salesforce]夏季&#39;22版本中，[!DNL Salesforce]将不再支持API旧版本21 -30。 在此Marketo Engage版本中，使用旧版API的所有[!DNL Sales Connect]请求都已更新，以保持在支持的版本中。 有关[!DNL Salesforce] API弃用计划的完整详细信息，请单击[此处](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}。

## API增强功能

* **批量程序成员提取API的新筛选功能**：按程序成员资格状态、updatedAt、cadence或用完的内容进行筛选，以优化提取的数据集。

* **批量程序成员提取API改进**：在创建作业期间指定最多10个程序以提高吞吐量。

## 公告

* **Forms弃用 — Forms 1.0、潜在客户捕获/保存端点以及Forms**&#x200B;的无脚本版本：到2022年10月，将从Marketo Engage中完全移除对Forms 1.0资源的支持。 所有现有的Forms 1.0资源都将停止运行。 Marketo Engage表单将要求在登陆页面和网站上加载JavaScript。

**_产品发布网络研讨会_**

[2022年6月和8月Marketo Engage发布网络研讨会](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## 2022 年 8 月 {#august}

在下方，您会找到2022年8月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。 请联系您的 Marketo Engage 代表了解更多信息。

以下功能已于&#x200B;**2022年8月26日**&#x200B;开始分阶段推出。

## 跨渠道编排

* 一次启用/禁用[!DNL Dynamic Chat]的所有已发布对话框**：通过按按钮从“配置”页面一次全局启用/禁用所有已发布对话框。

* **[!DNL Dynamic Chat]**&#x200B;的自定义头像：上传自定义聊天机器人头像，以便根据您的品牌对其进行个性化。

* **[!DNL Dynamic Chat]**&#x200B;的聊天记录：查看每个对话的聊天记录，以深入了解insight中每个Web访客感兴趣的内容。

## 下一代体验

* **Adobe品牌**：更新了编辑和人员详细信息页面的外观，并新增了Adobe Experience Cloud品牌。

* **在移动对话框中显示目标文件夹的文件夹层次结构**：查看每个文件夹的文件夹层次结构可简化移动资产的过程，并降低将资产放入错误文件夹的可能性。

* **[更新了新一代体验中的Screens](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md){target="_blank"}**：我们将在新一代体验中提供其他更新的屏幕，这些屏幕提供了可通过切换开关访问的最新设计和可用性增强功能：

   * 代码片段详细信息
   * “图像和文件”详细信息

>[!NOTE]
>
>在营销活动中，将资产移动到项目中的文件夹是一个例外。 此移动操作不会显示文件夹层次结构，因为项目中的文件夹不能具有重复名称。

## 体验自动化

* **[自助服务流程步骤 — 程序导入增强功能](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/flow-step-service.md){target="_blank"}**：改进了对导入具有自定义流程步骤的程序的支持，在该程序中，您现在可以使用同一服务提供程序的多个实例，并导入具有与这些服务提供程序兼容的流程步骤的程序。

* **[!DNL Munchkin]— 扩展的链接跟踪**：通过Munchkin扩展对`tel`和`mailto`链接的跟踪支持，以跟踪扩展的Web行为集。

* **Webhook自定义标头可见性**： Webhook自定义标头现在显示在[!UICONTROL Admin] > [!UICONTROL Webhooks]选项卡中，可见性更高。

* **CAPTCHA**：使用reCAPTCHA v3[&#128279;](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}评估表单提交的有效性以对传入的表单流量进行评分。 构建营销工作流以自动排除、隔离或删除可疑的机器人流量。

* **批准表单的权限**：新权限可控制哪些设计人员可以批准对表单的更改，这些更改与其他[!UICONTROL Design Studio]资源一致。 这可以防止其他设计人员在没有获得批准权限的其他人审阅表单的情况下，将更改推送到表单中。

* **在匿名合并后始终执行促销活动重播**：在促销活动重播之前进行匿名潜在客户合并，这样当匿名促销活动重播完成时，自定义字段筛选器可以可靠地工作。

## 营销数据环境

* **修复自定义对象“[!UICONTROL Used By]”字段的UI截断**：现在可以更轻松地识别“正在使用”的自定义对象字段，以便在必要时可以从自定义对象中删除字段。

## API增强功能

* **批量程序成员提取API的新筛选功能**：按程序成员资格状态、updatedAt、cadence或用完的内容进行筛选，以优化提取的数据集。

## [!DNL Sales Insight]

![（星形）](assets/yellow-star.png)

* **[[!DNL Sales Insight] 与 [!DNL Dynamic Chat]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}**&#x200B;集成：在[!DNL Sales Insight]面板中查看来自[!DNL Dynamic Chat]的活动，并在您的潜在客户工作中利用此新数据点。

## 公告

**_产品发布网络研讨会_**

[2022年6月和8月Marketo Engage发布网络研讨会](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## 2022 年 10 月 {#october}

在下方，您会找到2022年10月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。 请联系您的 Marketo Engage 代表了解更多信息。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2022年10月14日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。 请检查每个功能下方的状态。

### 营销数据环境

</br>

* **项目群成员自定义字段同步**：能够双向同步为项目群成员捕获的可扩展字段（例如，在活动注册期间与会者首选项，如食物、会话、曲目等） Salesforce中的促销活动成员字段。

<table>
  <tr>
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr>
   <td>已发布</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">项目成员自定义字段同步</a></td>
  </tr>
  </tbody>
</table>

* **Adobe Privacy Service集成**：与Privacy Service协调以自动遵守Experience Cloud产品中的数据隐私法规。 目前，此服务仅适用于已载入Adobe Identity Management System的Marketo Engage客户。

<table>
  <tr>
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr>
   <td>已发布</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### 下一代体验

</br>

* **更新了新一代体验中的Screens**：我们将在新一代体验中提供其他更新的屏幕，这些屏幕提供了可通过切换开关访问的最新设计和可用性增强功能：

   * 登录页面模板详情
   * 电子邮件模板列表

<table>
  <tr>
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr>
   <td>已发布</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">切换开关</a></td>
  </tr>
  </tbody>
</table>

* **电子邮件模板详细信息中的用于选项卡的增强功能**：在新Experience中，您将看到与使用电子邮件模板的资源相关的其他信息，包括资源状态、上次修改时间和上次修改者。 您还可以搜索、排序和筛选资源使用的列表。

<table>
  <tr>
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
  </tbody>
</table>

* **报表资产筛选器模型**：报表配置模型的新设计在配置菜单中显示新的资产树以及创建和修改日期的筛选器。

<table>
  <tr>
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
  </tbody>
</table>

### API增强功能

</br>

* **批量潜在客户导入：销售人员关联**：与潜在客户REST API存在对等关系，以便在批量潜在客户导入过程中将潜在客户与销售人员关联，从而减少所需的复杂性和调用API的次数。

<table>
  <tr>
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr>
   <td>已发布</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">批量商机导入</a></td>
  </tr>
  </tbody>
</table>

### 销售Insight

</br>

![（星形）](assets/yellow-star.png)

* **Sales Insight与Dynamic Chat的集成**： Insights Dashboard现在包括智能网格中的Dynamic Chat活动以及每周摘要和详细信息卡。

<table>
  <tr>
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr>
   <td>已发布</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Dynamic Chat 集成</a></td>
  </tr>
  </tbody>
</table>

## Agile版本功能

以下功能遵循Agile格式，并在标准发布日期之前或之后的各种日期发布。 请检查每个功能下方的状态。

* **自动排列Dynamic Chat的对话框流**：通过按按钮通过“自动排列”，将画布上的所有内容整理为简洁易读的格式，从而改善您拥挤的对话框画布。

<table>
  <tr>
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr>
   <td>已发布</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">流式传输Designer图标</a></td>
  </tr>
  </tbody>
</table>

* **Dynamic Chat的会议链接**：在发送给访客的每个日历邀请中自动包含Google和Outlook的“团队”或“会议”链接的选项。

<table>
  <tr>
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr>
   <td>已发布</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">日程表</a></td>
  </tr>
  </tbody>
</table>

* **支持Dynamic Chat的其他数据类型**：三种新数据类型（布尔值、整数、浮点数）允许您在Dynamic Chat中利用更多现有的Marketo Engage字段来诸如根据得分定位或询问访客是/否问题。

<table>
  <tr>
   <td><b>状态</b></td>
   <td><b>文档更新</b></td>
  </tr>
  <tr>
   <td>已发布</td>
   <td>不适用</td>
  </tr>
  </tbody>
</table>

## 公告

* **Forms 1.0**：将在10月版本中完成Forms 1.0的弃用。 Forms 1.0资源将不再能够向Marketo Engage提交数据，如果尝试，则将返回错误。

* **无脚本Forms**：在浏览器中禁用Javascript后，Forms将不再正常运行。 提交表单需要启用Javascript。

---
unique-page-id: 42762322
description: Salesforce中的“Marketo Sales Insight配置”选项卡 — Marketo文档 — 产品文档
title: Salesforce中的“Marketo Sales Insight配置”选项卡
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# Salesforce中的“Marketo Sales Insight配置”选项卡 {#marketo-sales-insight-configuration-tab-in-salesforce}

## 操作设置 {#operational-settings}

您需要设置此项才能开始在SFDC中使用Sales Insight。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI同时使用Soap和Rest API
* 您的Marketo帐户中的“销售分析”页面将有两个具有Soap和Rest API凭据的相应面板，您可以在此处复制并粘贴它们
* Soap和Rest API具有单独的超时，您可以根据组织的需求设置这些超时。 允许的最长时间为120秒
* 禁用分析功能板：您可以删除Rest API凭据，而仅使用Soap API。 这样做将禁用所有MSI Visualforce面板中的“分析功能板”选项卡

## MSI配置 {#msi-configuration}

配置适用于所有MSI用户，而不是特定于配置文件。

**Visualforce页面设置**

* “启用操作”下拉列表：
   * 能够从潜在客户和联系MSI布局的下拉列表中隐藏“发送Marketo电子邮件”
   * 能够从潜在客户和联系人MSI布局的下拉列表中隐藏“添加到Marketo Campaign”选项
* 即将举行的活动：能够向用户显示受邀的活动、所有活动或完全隐藏此选项卡
* 即将推出的营销活动：能够显示所有电子邮件营销活动或完全隐藏此选项卡
* 加载即将到来的活动和事件：通过将活动和活动选项卡置于按需“加载即将到来的项目”按钮的后面，能够减少用户发出的Rest API调用数
* 选项卡设置：默认情况下，所有五个选项卡都可用。 您可以在“销售分析”面板中选择选项卡的顺序。 相同的顺序将适用于所有布局(Lead、Contact、Account、Opportunity)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**“Marketo全局”选项卡**

* 启用RSS馈送：启用后，MSI用户可以在RSS馈送中查看其潜在客户馈送（除了Salesforce中的潜在客户馈送之外）。 只有在禁用“令牌过期”功能的情况下，RSS馈送才能正常工作。 此设置可在Marketo Sales Insight Admin页面中控制。
* 最佳调试模式
* 默认隐藏：您在此处选择的选项将是单击“隐藏”图标时最佳匹配在Marketo的“最佳匹配”选项卡中隐藏的天数
* 联系人状态字段：您在此处选择的选项将是一个值，该值填充到Marketo“最佳匹配”选项卡的“状态标题”列中
* 实时信息源设置：用于选择仅显示实时信息源的选项(在“销售线索”、“联系人”、“客户”和“业务机会”面板以及“全局Marketo”页面中)，仅显示销售线索信息源(在“Marketo全局”页面中)，或者同时显示实时信息和销售线索信息源
* 选项卡设置：默认情况下，所有五个选项卡都可用。 您可以在Marketo全局页面中选择选项卡的顺序

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**限制**

* 默认情况下，活动（有趣的时刻、Web活动、电子邮件）设置为1000。 电子邮件营销活动和事件默认设置为200
* 如果您注意到组织中存在超时问题，则可以减少限制

**操作设置**

* 发送Marketo电子邮件：启用此项将为所有Sales Insight用户授予从Lead 、 Contact 、 Account 、 Opportunity面板和Best Bets选项卡（批量操作和内联参与）发送电子邮件的访问权限
* 添加到Marketo Campaign：启用此项将使所有Sales Insight用户都有权从Lead 、 Contact 、 Account 、 Opportunity面板和Best Bets选项卡（批量操作和内联参与）添加到营销活动

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## 重置Marketo Sales Insight {#reset-marketo-sales-insight}

选择此操作将擦除SFDC中的所有配置，并且无法恢复它们。 您将必须重新配置所有内容。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

>[!IMPORTANT]
>
>除非您正在使用Sales Insights Actions功能，否则请不要选中“启用MSI操作”复选框。

>[!MORELIKETHIS]
>
>[添加对用户档案的销售分析访问权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}

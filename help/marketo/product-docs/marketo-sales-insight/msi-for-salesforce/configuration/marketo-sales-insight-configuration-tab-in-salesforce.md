---
unique-page-id: 42762322
description: Salesforce中的Marketo Sales Insight Configuration选项卡 — Marketo文档 — 产品文档
title: Salesforce 中的 Marketo Sales Insight 配置选项卡
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 1%

---

# [!DNL Marketo Sales Insight]中的[!DNL Salesforce]配置选项卡 {#marketo-sales-insight-configuration-tab-in-salesforce}

## 操作设置 {#operational-settings}

您需要设置此设置，才能开始在SFDC中使用[!DNL Sales Insight]。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI同时使用Soap和Rest API
* Marketo帐户中的Sales Insight页面将具有两个带Soap和Rest API凭据的相应面板，您可以在此处复制并粘贴这些面板
* Soap和Rest API具有单独的超时，您可以根据组织的需求设置这些超时。 允许的最长时间为120秒
* 禁用分析功能板：您可以删除Rest API凭据，而仅使用Soap API。 这样做将禁用所有MSI Visualforce面板中的分析功能板选项卡

## MSI配置 {#msi-configuration}

配置适用于所有MSI用户，而不是特定于配置文件。

**Visualforce页面设置**

* “启用操作”下拉列表：
   * 能够隐藏潜在客户和联系MSI布局中的发送Marketo电子邮件下拉列表
   * 能够从“潜在客户”和“联系人MSI布局”的下拉列表中隐藏“添加到Marketo促销活动”选项
* 即将发生的事件：能够向用户显示受邀事件、所有事件或完全隐藏此选项卡
* 即将推出的营销活动：可显示所有电子邮件营销活动或完全隐藏此选项卡
* 加载即将开始的营销活动和事件：通过将事件和营销活动选项卡置于按需“加载即将发生的项目”按钮的后面，能够减少用户发出的Rest API调用数
* 选项卡设置：默认情况下，所有五个选项卡均可用。 您可以在Sales Insight面板中选择选项卡的顺序。 相同的顺序将适用于所有布局(Lead、Contact、Account、Opportunity)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**Marketo全局选项卡**

* 启用RSS信息源：启用后，MSI用户可以在RSS信息源中查看其潜在客户信息源(除Salesforce中的潜在客户信息源之外)。 仅当“令牌过期”功能被禁用时，RSS馈送才能正常工作。 此设置可在您的Marketo Sales Insight Admin页面中进行控制。
* 最佳调试模式
* 默认隐藏：您在此处选择的选项是单击“隐藏”图标时最佳匹配在Marketo的“最佳匹配”选项卡中隐藏的天数
* 联系人状态字段：您在此处选择的选项将是在Marketo的“最佳匹配”选项卡的“状态标题”列中填充的值
* 实时信息源设置：用于选择仅显示实时信息源的选项(在“销售线索”、“联系人”、“客户”和“业务机会”面板以及“全局Marketo”页面中)，仅显示销售线索信息源(在“Marketo全局”页面中)，或同时显示实时信息和销售线索信息源
* 选项卡设置：默认情况下，所有五个选项卡均可用。 您可以在Marketo全局页面中选择选项卡的顺序

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**限制**

* 默认情况下，活动（有趣的时刻、Web活动、电子邮件）设置为1000。 电子邮件营销活动和事件默认设置为200
* 如果您注意到组织中存在超时问题，则可以降低限制

**操作设置**

* 发送Marketo电子邮件：如果启用此选项，将允许所有Sales Insight用户从Lead 、 Contact 、 Account 、 Opportunity面板和Best Bets选项卡（批量操作和内联参与）发送电子邮件
* 添加到Marketo Campaign：启用此项可为所有Sales Insight用户授予从Lead、Contact、Account、Opportunity面板和Best Bets选项卡（批量操作和内联参与）添加到营销活动的权限

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## 支持设置 {#support-settings}

选中此复选框将在您的Salesforce实例中启用Debug Logging 。 它可以帮助您排除问题。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

## 重置Marketo Sales Insight {#reset-marketo-sales-insight}

选择这样做将擦除SFDC中的所有配置，并且无法恢复它们。 您将必须重新配置所有内容。

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-6.png)

>[!IMPORTANT]
>
>除非您正在使用Sales Insights Actions功能，否则请不要选中“启用MSI操作”复选框。

>[!MORELIKETHIS]
>
>[添加Sales Insight访问用户档案的权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}

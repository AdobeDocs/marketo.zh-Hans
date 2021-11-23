---
unique-page-id: 37356893
description: MSI功能概述 — Marketo文档 — 产品文档
title: MSI功能概述
exl-id: e6cd988c-afba-44e3-b240-68258236f344
source-git-commit: 5f2967fb56daa8c3f86f6d9577626928f1e5bbd6
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 0%

---

# MSI功能概述 {#msi-feature-overview}

MSI在Salesforce Lightning和Classic中具有以下功能。

## Visualforce面板 {#visualforce-panel}

MSI Visualforce面板包含以下功能：

* 选项卡

   * [分析功能板](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/insights-dashboard-feature-overview.md)
   * 有趣的时刻
   * Web活动
   * 电子邮件
   * 得分

* 操作

   * 添加到Marketo Campaign
   * 发送Marketo电子邮件
   * 从监视列表添加/删除

* 星与火焰

## 潜在客户布局 {#lead-layout}

可视化强制页面：

* 潜在客户 — 包含单击超级“转至完整列表”的选项，您将被发送到Salesforce中的新选项卡，在该选项卡中，MSI面板将以全页布局显示
* 潜在客户完整列表 — 不包括“转至完整列表”选项
* 潜在客户移动设备 — 在Salesforce移动设备应用程序中可见
* 潜在客户联系人桥 — 显示您在MSI联系人ID字段中添加的联系人的MSI面板

字段：

* 最后一个有趣的时刻
* 最后有趣的时刻日期
* 最后一个有趣的时刻
* 最后有趣的时刻来源
* 最后有趣的时刻类型
* 上次Marketo活动（按销售）
* 上次按销售额划分的Marketo参与度
* 相对分数
* 相对分数值
* 紧急
* 紧急价值
* 在Marketo中查看 — 单击此字段可打开Marketo中潜在客户的不可编辑视图。 包括：潜在客户信息、公司信息、SFDC潜在客户信息、SFDC自定义字段、活动日志
* MSI联系人ID — 将Salesforce联系人添加到此字段，并在潜在客户布局中包含“潜在客户联系人桥”面板，以查看联系人的MSI面板

## 联系人布局 {#contact-layout}

可视化强制页面：

* 联系人 — 包含单击超级“转至完整列表”的选项，您将被发送到Salesforce中的新选项卡，在该选项卡中，MSI面板将以全页布局显示
* 联系人完整列表 — 不包括“转至完整列表”选项
* 联系移动设备 — 在Salesforce移动应用程序中可见
* 添加到Marketo Campaign联系人页面 — 此面板中提供了添加到Marketo Campaign功能

字段：

* 最后一个有趣的时刻
* 最后有趣的时刻日期
* 最后一个有趣的时刻
* 最后有趣的时刻来源
* 最后有趣的时刻类型
* 上次Marketo活动（按销售）
* 相对分数
* 相对分数值
* 紧急
* 紧急价值
* 在Marketo中查看 — 单击此字段可打开Marketo中潜在客户的不可编辑视图。 包括：潜在客户信息、公司信息、SFDC潜在客户信息、SFDC自定义字段、活动日志
* Mkto潜在客户得分
* 销售分析 — 打开联系人完整列表页面

## 帐户布局 {#account-layout}

可视化强制页面：

* 帐户 — 包含单击超级“转至完整列表”的选项，您将被发送到Salesforce中的新选项卡，在该选项卡中，MSI面板将以全页布局显示
* 帐户完整列表 — 不包括“转至完整列表”选项
* 帐户移动 — 在Salesforce移动应用程序中可见

字段：

* 销售分析 — 打开联系人完整列表页面

操作：

* 添加到Marketo Campaign
* 发送Marketo电子邮件
* 从监视列表添加/删除

以下功能包括 **不可用** 在“帐户布局”页面中：

* 星与火焰

## 机会布局 {#opportunity-layout}

可视化强制页面：

* 机会 — 包含单击超级“转到完整列表”的选项，您将被发送到Salesforce中的新选项卡，在该选项卡中，MSI面板将以全页布局显示
* Opportunity Full List — 不包括“转至Full List”选项
* Opportunity Mobile — 在Salesforce移动应用程序中可见

字段：

* 销售分析 — 打开联系人完整列表页面
* Marketo Opportunity Analysis — 在Marketo打开Opportunity Inflect Analyzer

操作：

* 添加到Marketo Campaign
* 发送Marketo电子邮件
* 从监视列表添加/删除

以下功能包括 **不可用** 在Opportunity Layout页面中：

* 星与火焰

## 潜在客户和联系人列表视图（批量操作） {#lead-and-contact-list-view-bulk-actions}

Salesforce闪电：在“潜在客户”和“联系人”列表视图中，将添加到观看列表、添加到Marketo Campaign和发送Marketo电子邮件批量操作按钮。

Salesforce Classic:在“潜在客户”和“联系人”列表视图中，“添加到观看列表”、“添加到Marketo Campaign”和“发送Marketo电子邮件”批量操作按钮。

## Marketo选项卡 {#marketo-tab}

* 最佳下注

   * 包括创建和编辑视图的功能。 能够根据“Marketo配置”页面中“默认隐藏”选项的配置来隐藏最佳结果
   * 列 — 名称、帐户、最后关注时刻、状态标题、参与度（星星和火焰）、隐藏

* 我的监视列表

   * 包括创建和编辑视图的功能
   * 列 — 名称、帐户、最后关注时刻、状态标题、参与度（星星和火焰），删除

* Web活动

   * 包括创建和编辑视图、时间范围过滤器功能的功能
   * 列 — 页面查看、名称、帐户、上次访问

* 匿名Web活动

   * 包括创建和编辑视图、时间范围过滤器功能的功能
   * 列 — 页面查看、公司、上次访问、研究(打开公司的LinkedIn页面)

* 我的电子邮件

   * 包括创建和编辑视图的功能
   * 列 — 名称、帐户、主题、日期、打开、单击

* 潜在客户馈送 — 包括订阅相关时刻的功能，必须启用“配置”页面上的RSS馈送才能使用此功能

   * 具有此有趣时刻的领导/联系人
   * 有趣的时刻类型（Web、电子邮件或里程碑）和描述
   * 帐户名称
   * 这个有趣的时刻发生的时间
   * 用于接收此类事件的电子邮件通知的订阅选项
   * 显示此人是最佳人选的高优先级图标

## Marketo Sales Insight“配置”选项卡 {#marketo-sales-insight-configuration-tab}

* 操作设置：包括在SFDC中设置MSI所需的Soap和Rest API凭据
* MSI配置：包括配置Marketo选项卡和MSI可视化力面板
* 重置Marketo销售分析：包括清除所有配置的功能

>[!MORELIKETHIS]
>
>[Marketo Sales Insight的“配置”选项卡](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md)

## 销售分析绩效报表 {#sales-insight-performance-reports}

查看通过Salesforce、Microsoft Dynamics或Gmail或Outlook插件发送的电子邮件的性能

## 适用于移动设备的MSI {#msi-for-mobile}

Salesforce移动应用程序支持MSI功能

## 语言支持 {#language-support}

Marketo Sales Insight按语言进行存储。 因此，如果您希望它适用于多种语言，则必须分别输入每种语言的凭据。

>[!NOTE]
>
>* 联系人/潜在客户需要位于默认分区中才能添加到监视列表。
>
>* MSI Salesforce包不支持具有相关字段的自定义视图。


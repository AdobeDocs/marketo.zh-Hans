---
unique-page-id: 37356893
description: MSI功能概述- Marketo Docs —— 产品文档
title: MSI功能概述
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---


# MSI功能概述 {#msi-feature-overview}

MSI在Salesforce Lightning和Classic中提供以下功能。

## Visualforce面板 {#visualforce-panel}

MSI Visualforce面板包含以下功能：

* 选项卡

   * [洞察仪表板](http://docs.marketo.com/x/EoGMAg)
   * 有趣的时刻
   * Web活动
   * 电子邮件
   * 得分

* 操作

   * 添加到营销活动
   * 发送Marketo电子邮件
   * 添加／从监视列表

* 星与火焰

## 潜在客户布局 {#lead-layout}

Visualforce页面：

* 潜在客户——包含单击超级“转至完整列表”的选项，您将被发送到Salesforce中的新选项卡，在该选项卡中，MSI面板将在整个页面布局中显示
* 潜在客户完整列表-不包括“转至完整列表”选项
* 潜在客户移动——在Salesforce移动应用程序中可见
* 潜在客户联系人桥接器——显示您在MSI联系人ID字段中添加的联系人的MSI面板

字段：

* 最后一个有趣的时刻
* 最后一个有趣的时刻日期
* 《最后有趣的时刻》
* 最后有趣的时刻源
* 最后有趣的时刻类型
* 上一个按销售活动的营销人员
* 按销售人员列出的最后一个营销人员参与情况
* 相对得分
* 相对得分值
* 紧急
* 紧急值
* 视图在Marketo中——单击此字段可打开Marketo中不可编辑的潜在客户视图。 包括：潜在客户信息、公司信息、SFDC潜在客户信息、SFDC自定义字段、活动日志
* MSI联系人ID —— 将Salesforce联系人添加到此字段，并在潜在客户布局中加入“潜在客户联系人桥接器”面板，以查看联系人的MSI面板

## 联系人布局 {#contact-layout}

Visualforce页面：

* 联系人——包含单击超级“转至完整列表”选项，您将被发送到Salesforce中的新选项卡，在该选项卡中，MSI面板将在整个页面布局中显示
* 联系完整列表-不包括“转到完整列表”选项
* 联系移动——在Salesforce移动应用程序中可见
* 添加到Marketo活动联系人页——添加到Marketo活动功能在此面板中可用

字段：

* 最后一个有趣的时刻
* 最后一个有趣的时刻日期
* 《最后有趣的时刻》
* 最后有趣的时刻源
* 最后有趣的时刻类型
* 上一个按销售活动的营销人员
* 相对得分
* 相对得分值
* 紧急
* 紧急值
* 视图在Marketo中——单击此字段可打开Marketo中不可编辑的潜在客户视图。 包括：潜在客户信息、公司信息、SFDC潜在客户信息、SFDC自定义字段、活动日志
* Mkto潜在客户得分
* 销售分析——打开联系人完整列表页

## 帐户布局 {#account-layout}

Visualforce页面：

* 帐户——包含单击超级“转至完整列表”的选项，您将被发送到Salesforce中的新选项卡，在该选项卡中，MSI面板将在整个页面布局中显示
* 帐户完整列表-不包括“转到完整列表”选项
* 帐户移动——在Salesforce移动应用程序中可见

字段：

* 销售分析——打开联系人完整列表页

“帐户布局” **页面中** 不提供以下功能：

* 操作：添加到Marketo活动、发送Marketo电子邮件、添加／从观察列表
* 星与火焰

## 机会布局 {#opportunity-layout}

Visualforce页面：

* Opportunity —— 包含单击超级“转到完整列表”选项，您将被发送到Salesforce中的新选项卡，在该选项卡中，MSI面板将在整个页面布局中显示
* 机会完整列表-不包括“转到完整列表”选项
* Opportunity Mobile —— 在Salesforce移动应用程序中可见

字段：

* 销售分析——打开联系人完整列表页
* Marketo机会分析-在Marketo中打开机会影响分析器

以下功能 **在Opportunity** Layout页面中不可用：

* 操作：添加到Marketo活动、发送Marketo电子邮件、添加／从观察列表
* 星与火焰

## 潜在客户和联系人列表视图（批量操作） {#lead-and-contact-list-view-bulk-actions}

Salesforce闪电：添加到观察列表、添加到营销活动和发送Marketo电子邮件批量操作按钮，在潜在客户和联系列表视图中。

Salesforce经典：添加到“观察列表”、“添加到营销人员”和“发送Marketo电子邮件”批量操作按钮，并在“潜在客户”和“联系人”活动视图中执行列表操作。

## Marketo选项卡 {#marketo-tab}

* 最佳赌注

   * 包括创建和编辑视图的功能。 根据“Marketo配置”页中“默认隐藏”选项的配置隐藏最佳赌注的能力
   * 列——名称、帐户、最后有趣的时刻、状态标题、参与（星星和火焰）、隐藏

* 我的手表列表

   * 包括创建和编辑视图的功能
   * 列——名称、帐户、最后感兴趣的时刻、状态标题、参与（星星和火焰）、删除

* Web活动

   * 包括创建和编辑视图、时间帧过滤器功能
   * 列——页面视图、名称、帐户、上次访问

* 匿名Web活动

   * 包括创建和编辑视图、时间帧过滤器功能
   * 列——页面视图、公司、上次访问、研究(打开公司的LinkedIn页面)

* 我的电子邮件

   * 包括创建和编辑视图的功能
   * 列——名称、帐户、主题、日期、打开，单击

* 潜在客户源——包括订阅有趣时刻的功能，必须启用“配置”页上的RSS源才能使用此功能

   * 具有此有趣时刻的主管／联系人
   * 有趣的时刻类型（Web、电子邮件或里程碑）和描述
   * 帐户名称
   * 这个有趣的时刻发生的时间
   * 用于接收此类事件的电子邮件通知的“订阅”选项
   * 显示此人的高优先级图标是最佳选择

## Marketo Sales Insight配置选项卡 {#marketo-sales-insight-configuration-tab}

* 操作设置：包括在SFDC中设置MSI所需的Soap和Rest API凭据
* MSI配置：包括配置Marketo选项卡和MSI Visualforce面板
* 重置Marketto Sales Insight:包括清除所有配置的功能

>[!NOTE]
>
>**相关文章**
>
>[Salesforce中的“Marketo Sales Insight配置”选项卡](http://docs.marketo.com/x/UoCMAg)

## Sales Insight Performance Reports {#sales-insight-performance-reports}

视图通过Salesforce、Microsoft Dynamics或Gmail或Outlook插件发送的电子邮件的性能

## 移动MSI {#msi-for-mobile}

Salesforce移动应用程序支持MSI功能

## 语言支持 {#language-support}

Marketo Sales Insight按语言存储。 因此，如果希望它适用于多种语言，您必须分别为每种语言输入凭据。

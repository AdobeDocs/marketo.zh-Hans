---
unique-page-id: 6848747
description: 角色权限描述 — Marketo文档 — 产品文档
title: 角色权限描述
exl-id: 00963cd9-2d53-455f-bc6f-42a573468ff9
feature: Users and Roles
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 0%

---

# 角色权限描述 {#descriptions-of-role-permissions}

以下是您可以分配给角色的所有可用权限列表。 权限通常与Marketo中的特定功能区域相关联，可以帮助您控制不同用户有权访问的区域和功能。

有关权限的一些其他信息：

* “访问”权限授予角色查看并编辑应用程序该部分的权限。
* 要使角色具有子权限（“创建”、“删除”等）的访问权限，该角色必须具有应用程序该部分的“访问权限”权限。 例如，如果您要授予某人“编辑营销活动”的权限，则他们必须拥有访问营销活动的整体权限。
* 您可能会看到没有权限使用的操作或资源。 但是，如果您尝试访问它们，将会看到一条消息，警告您访问受限。

## 可用权限 {#available-permissions}

当您[创建或编辑角色](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md)时，可以通过选中相应的框来选择允许该角色使用的以下权限之一。

![](assets/descriptions-of-role-permissions-1.png)

## 访问管理员  {#access-admin}

查看管理员的“我的帐户”部分中的设置并进行更改。

* 访问Adobe Connect — 允许用户访问Adobe Connect屏幕
* 访问Adobe Experience Manager&#42; — 允许用户访问Adobe Experience Manager屏幕
* 访问Adobe组织映射&#42; — 授予用户访问Adobe组织映射屏幕的权限
* 访问管理员审核记录&#42; — 授予用户访问管理员审核记录屏幕的权限
* 访问审核记录&#42; — 授予用户访问审核记录的权限
* 访问审核记录 — 让用户可以访问资产审核记录和管理员审核记录
* 访问CAPTCHA — 访问CAPTCHA屏幕
* 访问渠道 — 仅授予用户修改渠道标记的权限，而不授予其他自定义标记的权限
* 访问通信限制 — 授予用户在管理员中启用通信限制的权限
* 访问CRM — 授予用户在管理员中访问CRM （如[!DNL Salesforce]或[!DNL Microsoft Dynamics]）的权限
* 访问`Data.com` — 授予用户访问Data.com流操作的权限
* 访问电子邮件管理员 — 赋予用户访问电子邮件管理员的权限，以更改默认设置，如取消订阅和品牌化域
* 访问事件合作伙伴 — 以管理员身份授予用户访问LaunchPoint的权限
* 访问Experience Cloud受众共享 — 通过受众，用户可以将受众从Adobe Experience Cloud同步到Marketo Engage
* 访问字段管理 — 允许用户访问管理员中的字段管理
* 访问文件上传 — 使用户能够将图像和文件上传到Design Studio
* 访问登陆页面 — 允许用户在Admin中访问登陆页面
* 访问位置 — 允许用户访问管理员中的位置，以设置默认语言、区域设置、时区和货币
* 访问登录历史记录 — 允许用户访问审核记录中的用户登录历史记录
* 访问登录设置 — 允许用户访问“管理员”中的“登录设置”，以获取安全性、IP限制和智能列表报表设置
* 访问新体验&#42; — 允许用户访问新体验屏幕
* 访问Marketo自定义活动 — 允许用户在“管理员”中访问Marketo自定义活动
* 访问Marketo自定义对象 — 允许用户在管理员中访问Marketo自定义对象
* 访问[!DNL Munchkin] — 授予用户在管理员中访问[!DNL Munchkin]的权限，以设置跟踪代码、人员跟踪和启用API配置
* 访问Predictive Audiences&#42; — 允许用户访问Predictive Audiences屏幕
* 访问Revenue Cycle Analytics — 让用户可以访问Admin中的Revenue Cycle Analytics，以设置同步摘要和归因
* 访问角色 — 授予用户管理和编辑角色的权限，但不授予用户
* 访问Sales Insight — 授予用户在管理员中管理Sales Insight的权限，用于设置状态、API配置、人员评分和其他设置
* 访问单点登录 — 让用户可以在Admin中管理单点登录，以便启用SAML并使用SAML设置和重定向页面URL
* 访问Smart Campaign — 让用户在管理员中访问Smart Campaign，以限制对合格人员的限制
* 访问SOAP API — 允许用户在Admin中管理Web服务中的SOAP API
* 访问标记 — 允许用户访问除渠道标记以外的所有自定义标记
* 访问Treasure Check — 让用户能够在Admin中访问Treasure Check中的实验功能
* 访问用户 — 授予用户在管理员中编辑和管理用户（而非角色）的权限
* 访问Webhook — 为用户提供Admin中的Webhook，用于设置详细信息和响应映射
* 访问工作区和分区 — 使用户可以在Admin中创建、编辑和删除工作区和分区

_&#42;为避免现有用户中断，此权限将在被动模式下引入，此时可见但不可访问。 我们将传达该工具在2024年年中成为活动状态时如何实施该工具。_

## 访问API  {#access-api}

授予具有&#x200B;**仅API** **角色**&#x200B;的用户访问下面列出的各个API的权限。

* 批准Assets
* 执行营销活动
* 只读活动
* 只读活动元数据
* 只读Assets
* 只读营销活动
* 只读公司
* 只读自定义对象
* 只读人员
* 只读指定帐户
* 只读机会
* 只读销售人员
* 读写活动
* 读写活动元数据
* 读写Assets
* 读写营销活动
* 读写公司
* 读写自定义对象
* 读写人员
* 读写指定帐户
* 读写机会
* 读写销售人员

## 访问Analytics {#access-analytics}

允许用户访问Analytics选项卡、电子邮件分析、报表以及下面的三个项目，除非未选中它们。

* 访问Revenue Explorer — 取消选中将删除用户对Revenue Explorer的访问权限
* 创建报表&#42; — 赋予用户在Analytics和Marketing Activities以及Revenue Cycle Modeler资产中创建、克隆、读取、更新和移动报表资产的权限
* 删除报告 — 取消选中此项将删除用户删除报告的能力
* 导出Analytics数据 — 取消选中此项会删除用户导出Analytics数据的能力

_&#42;为避免现有用户中断，此权限将在被动模式下引入，此时可见但不可访问。 我们将传达该工具在2024年年中成为活动状态时如何实施该工具。_

## 访问日历演示 {#access-calendar-presentations}

使用户能够访问“日历”演示文稿 — 允许显示在底部的“演示文稿”按钮。

* 编辑日历演示文稿 — 允许用户编辑日历中的演示文稿

## 访问Design Studio {#access-design-studio}

允许用户访问Design Studio选项卡和树视图，但不能访问详细信息。

* 访问电子邮件
   * 编辑电子邮件 — 授予用户编辑、创建和克隆电子邮件的权限
      * 使电子邮件可操作 — 授予用户使电子邮件可操作的权限。 请参阅：[使电子邮件正常运行](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)

      * 批准电子邮件 — 允许用户批准电子邮件。
      * 删除电子邮件 — 允许用户删除电子邮件。
      * 设置品牌域 — 使用户能够使用品牌域。 请参阅：[添加附加品牌推广域](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/add-an-additional-branding-domain.md)

* 访问电子邮件模板

   * 批准电子邮件模板
   * 删除电子邮件模板
   * 编辑电子邮件模板 — 编辑、创建和克隆电子邮件模板

* 访问表单

   * 批准表单
   * 删除表单
   * 编辑表单 — 编辑、创建和克隆表单

* 访问图像

   * 删除图像
   * 上传图像

* 访问登陆页面

   * 批准登陆页面
   * 删除登陆页面
   * 编辑登陆页面 — 编辑、创建和克隆登陆页面

* 访问登陆页面模板

   * 批准登陆页面模板
   * 删除登陆页面模板
   * 编辑登陆页面模板 — 编辑、创建和克隆登陆页面模板

* 访问代码片段

   * 批准代码片段
   * 删除代码片段
   * 编辑代码片段

* 访问社交应用程序

   * 批准社交应用程序
   * 删除社交应用程序
   * 编辑社交应用程序

## Access数据库 {#access-database}

查看数据库以及查看和编辑智能/静态列表。

* 访问分段

   * 批准分段
   * 删除分段
   * 编辑分段

* 删除人员
* 创建列表&#42;
   * 在数据库和营销活动中创建列表资产的权限
   * 在数据库和营销活动中创建智能列表资产的权限
* 删除列表
* 编辑人员 — 阻止手动编辑和运行单个流程步骤；您仍然可以通过针对人员运行营销活动来编辑人员
* 导出人员 — 从数据库列表中导出带有的电子表格
* 导入自定义对象
* 导入列表
* 合并人员
* 运行单流操作 — 使用户能够对数据库中的人员运行&#x200B;**更改数据值**&#x200B;流步骤

* 查看机会数据 — 在人员详细信息页面上隐藏机会信息

_&#42;为避免现有用户中断，此权限将在被动模式下引入，此时可见但不可访问。 我们将传达该工具在2024年年中成为活动状态时如何实施该工具。_

## 访问营销活动 {#access-marketing-activities}

查看营销活动选项卡、营销活动和营销活动文件夹。

* 访问短信消息

   * 批准短信消息
   * 删除短信消息
   * 编辑短信消息

* 访问推送通知

   * 批准推送通知
   * 删除推送通知
   * 编辑推送通知

* 访问奖
* 激活触发器营销活动
* 批准电子邮件项目
* 克隆营销资产
* 删除营销资产
* 编辑营销活动限制
* 编辑营销资产
* 导出营销活动活动&#42;
* 导入项目群
* 列表导入
* 计划批处理活动

访问SEO

* 管理SEO
* 标准SEO

_&#42;为避免现有用户中断，此权限将在被动模式下引入，此时可见但不可访问。 我们将传达该工具在2024年年中成为活动状态时如何实施该工具。_

## 定位和Personalization {#targeting-and-personalization}

* 管理Web Personalization
* CRE营销活动编辑器
* CRE Campaign启动器
* Web营销活动编辑器
* Web营销活动启动器

Workspace管理

* 特定Workspace的管理员访问权限（仅当启用了工作区时）
* 在工作区之间移动资产（仅在启用了工作区的情况下）

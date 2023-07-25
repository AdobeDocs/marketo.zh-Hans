---
unique-page-id: 6848747
description: 角色权限描述 — Marketo文档 — 产品文档
title: 角色权限描述
exl-id: 00963cd9-2d53-455f-bc6f-42a573468ff9
feature: Users and Roles
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# 角色权限描述 {#descriptions-of-role-permissions}

以下是您可以分配给角色的所有可用权限的列表。 权限通常与Marketo中的特定功能区域相关联，并可帮助您控制不同用户有权访问的区域和功能。

有关权限的一些其他信息：

* “访问”权限授予角色查看并编辑应用程序该部分的权限。
* 要使角色具有子权限（“创建”、“删除”等）的访问权限，该角色必须具有应用程序该部分的“访问权限”权限。 例如，如果要授予某人“编辑营销活动”的权限，此人必须拥有访问营销活动的整体权限。
* 您可能会看到没有权限使用的操作或资源。 但是，如果您尝试访问它们，则会看到一条消息，警告您访问受限。

## 可用权限 {#available-permissions}

当您 [创建或编辑角色](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md)，您可以通过选中相应的框来选择允许该角色使用的以下权限之一。

![](assets/descriptions-of-role-permissions-1.png)

## 访问管理员  {#access-admin}

查看管理员的“我的帐户”部分中的设置并进行更改。

* 访问审核记录 — 让用户可以访问资产审核记录和管理审核记录
* 访问渠道 — 仅授予用户修改渠道标记（而非其他自定义标记）的访问权限
* 访问通信限制 — 授予用户在“管理员”中启用通信限制的访问权限
* 访问CRM — 授予用户访问CRM的权限，例如 [!DNL Salesforce] 或 [!DNL Microsoft Dynamics]，在管理员中
* 访问 [[!DNL Data.com]](https://Data.com)  — 授予用户访问Data.com流操作的权限
* 访问电子邮件管理员 — 允许用户使用电子邮件管理员更改默认设置，如取消订阅和品牌推广域
* 访问事件合作伙伴 — 让用户以管理员身份访问LaunchPoint
* 访问字段管理 — 允许用户访问管理员中的字段管理
* 访问文件上传 — 使用户能够将图像和文件上传到Design Studio
* 访问登陆页面 — 让用户有权访问管理员中的登陆页面
* 访问位置 — 允许用户访问管理员中的位置，以设置默认语言、区域设置、时区和货币
* 访问登录历史记录 — 允许用户访问审核记录中的用户登录历史记录
* 访问登录设置 — 允许用户访问“管理员”中的“登录设置”以获得安全性、IP限制和智能列表报表设置
* 访问Marketo自定义活动 — 允许用户在“管理员”中访问Marketo自定义活动
* 访问Marketo自定义对象 — 让用户可以访问管理员中的Marketo自定义对象
* 访问 [!DNL Munchkin]  — 允许用户访问 [!DNL Munchkin] 用于设置跟踪代码、人员跟踪和启用API配置
* 访问Revenue Cycle Analytics — 让用户可以访问Admin中的Revenue Cycle Analytics，以设置同步摘要和归因
* 访问角色 — 赋予用户管理和编辑角色的访问权限，但不赋予用户管理和编辑角色的权限
* 访问Sales Insight — 让用户有权在“管理员”中管理Sales Insight，以便设置Status、API配置、人员评分和其他设置
* 访问单点登录 — 让用户可以在“管理员”中管理单点登录，以便启用SAML并处理SAML设置和重定向页面URL
* 访问Smart Campaign — 让用户在管理员中访问Smart Campaign，以限制对合格人员的限制
* 访问SOAP API — 让用户有权在Admin中管理Web服务中的SOAP API
* 访问标记 — 允许用户访问除渠道标记以外的所有自定义标记
* 访问Treasure Check — 让用户可以访问Admin中的Treasure Check中的实验功能
* 访问用户 — 授予用户在“管理员”中编辑和管理用户（但不管理角色）的权限
* 访问Webhook — 让用户在“管理员”中访问Webhook，以设置详细信息和响应映射
* 访问工作区和分区 — 赋予用户在Admin中创建、编辑和删除工作区和分区的权限

## 访问API  {#access-api}

为用户提供以下功能 **仅API** **角色** 访问下面列出的单个API。

* 批准资产
* 执行营销活动
* 只读活动
* 只读活动元数据
* 只读资产
* 只读营销活动
* 只读公司
* 只读自定义对象
* 只读人员
* 只读指定帐户
* 只读机会
* 只读销售人员
* 读写活动
* 读写活动元数据
* 读写资产
* 读写营销活动
* 读写公司
* 读写自定义对象
* 读写人员
* 读写指定帐户
* 读写机会
* 读写销售人员

## 访问Analytics {#access-analytics}

允许用户访问Analytics选项卡、电子邮件分析、报表以及下面的三个项目，除非未选中这些项。

* 访问Revenue Explorer — 取消选中将删除用户对Revenue Explorer的访问权限
* 删除报告 — 取消选中此项会删除用户删除报告的能力
* 导出Analytics数据 — 取消选中将删除用户导出Analytics数据的能力

## 访问日历Presentations {#access-calendar-presentations}

允许用户访问“日历”演示文稿 — 允许显示在底部的“Presentations”按钮。

* 编辑日历Presentations — 允许用户在日历中编辑演示文稿

## 访问Design Studio {#access-design-studio}

允许用户访问Design Studio选项卡和树视图，但不能访问详细信息。

* 访问电子邮件
   * 编辑电子邮件 — 授予用户编辑、创建和克隆电子邮件的权限
      * 使电子邮件可操作 — 授予用户使电子邮件可操作的权限。 请参阅： [使电子邮件可运行](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)

      * 批准电子邮件 — 允许用户批准电子邮件。
      * 删除电子邮件 — 允许用户删除电子邮件。
      * 设置品牌域 — 使用户能够使用品牌域。 请参阅： [添加附加品牌推广域](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/add-an-additional-branding-domain.md)

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
* 删除列表
* 编辑人员 — 阻止手动编辑和运行单个流程步骤；您仍然可以通过针对人员运行营销活动来编辑人员
* 导出人员 — 从数据库列表中导出电子表格和
* 导入自定义对象
* 导入列表
* 合并人员
* 运行单流操作 — 使用户能够运行 **更改数据值** 对数据库中的人员执行流程步骤

* 查看Opportunity数据 — 在人员详细信息页面上隐藏Opportunity信息

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

* 访问奖励
* 激活触发器营销活动
* 批准电子邮件项目
* 克隆营销资产
* 删除营销资产
* 编辑营销活动限制
* 编辑营销资产
* 导入程序
* 列表导入
* 计划批处理活动

访问SEO

* 管理SEO
* 标准SEO

## 定位和个性化 {#targeting-and-personalization}

* 管理Web个性化
* CRE营销活动编辑器
* CRE Campaign启动器
* Web营销活动编辑器
* Web营销活动启动器

工作区管理

* 特定工作区的管理员访问权限（仅当启用了工作区时）
* 在工作区之间移动资产（仅当启用了工作区时）

---
description: 第2步（共3步） — 为Marketo创建Salesforce用户(Enterprise/Unlimited) - Marketo文档 — 产品文档
title: 第2步（共3步） — 为Marketo创建Salesforce用户(Enterprise/Unlimited)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 1%

---

# 第2步（共3步）：为Marketo创建Salesforce用户(Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>这些步骤必须由Salesforce管理员完成

>[!PREREQUISITES]
>
>[第1步（共3步）：将Marketo字段添加到Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

在本篇文章中，您将在Salesforce配置文件中设置用户权限，并创建一个Marketo-Salesforce集成帐户。

## 创建配置文件 {#create-a-profile}

1. 单击&#x200B;**[!UICONTROL 设置]**。

   屏幕快照

1. 在导航搜索栏中键入“profiles”，然后单击“Profiles”链接。

   屏幕快照

1. 单击新建配置文件。

   屏幕快照

1. 选择“标准用户”，将配置文件命名为“Marketo-Salesforce同步”，然后单击“保存”。

   屏幕快照

## 设置配置文件权限 {#set-profile-permissions}

1. 单击“编辑”以设置安全权限。

   屏幕快照

1. 在“管理权限”部分下，确保选中以下复选框：

   * API已启用
   * 编辑HTML模板
   * 管理公共文档
   * 管理公共模板

   >[!TIP]
   >
   >确保选中“密码永不过期”框。

1. 在“常规用户权限”部分下，确保选中以下复选框：

   * 转换潜在客户
   * 编辑事件
   * 编辑任务

1. 在“标准对象权限”部分下，确保检查读取、创建、编辑和删除权限：

   * 帐户
   * 营销活动
   * 联系人
   * 潜在客户
   * 机会

   >[!NOTE]
   >
   >如果您计划使用Campaign同步，请向促销活动授予权限。

   屏幕快照

1. 完成后，单击页面底部的Save 。

   屏幕快照

## 设置字段权限 {#set-field-permissions}

1. 与您的营销人员讨论，了解哪些自定义字段是同步所必需的。

   >[!NOTE]
   >
   >此步骤将阻止您不需要的字段显示在Marketo中，这将减少杂乱并加快同步速度。

1. 在用户档案详细信息页面中，转到字段级安全性部分。 单击查看可编辑对象的辅助功能：

   * 潜在客户
   * 联系人
   * 帐户
   * 机会

   >[!TIP]
   >
   >您可以根据组织的需求配置其他对象。

1. 对于每个对象，单击“编辑”。

   屏幕快照

1. 找到不需要的字段，确保未选中“读取权限”和“编辑权限”。 完成后单击保存。

   >[!NOTE]
   >
   >仅编辑自定义字段的辅助功能。

   屏幕快照

1. 禁用完所有不需要的字段后，必须选中以下对象字段的读取访问和编辑访问。 完成后单击保存。

   表

   屏幕快照

## 创建Marketo-Salesforce同步帐户 {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>创建专用的Salesforce帐户（例如`marketo@yourcompany.com`），以区分Marketo用户与其他Salesforce用户所做的更改。

1. 在导航搜索栏中键入“Manage users”（管理用户），然后单击Users（用户）。 单击“新建用户”。

   屏幕快照

   屏幕快照

1. 填写必填字段。 然后，选择用户许可证：Salesforce以及您之前创建的配置文件。 完成后，单击保存。

   屏幕快照

第2步（共3步）已完成。

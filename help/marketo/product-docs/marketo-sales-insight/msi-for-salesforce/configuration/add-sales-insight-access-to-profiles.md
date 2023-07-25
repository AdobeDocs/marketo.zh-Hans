---
description: 对配置文件添加销售分析访问权限 — Marketo文档 — 产品文档
title: 添加对用户档案的销售分析访问权限
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# 添加对用户档案的销售分析访问权限 {#add-sales-insight-access-to-profiles}

下面是如何创建有权访问Sales Insight的用户档案，同时删除其他用户档案的访问权限。 这适用于已经安装了 [Sales InsightAppExchange包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>如果您以前授予了所有用户档案的销售分析访问权限，则您必须 [删除配置文件级别访问权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} 以使用此权限集。

## 为Sales Insight创建新的配置文件 {#create-a-new-profile-for-sales-insight}

如果您有专门的Sales Insight用户档案，则可以跳过此步骤。

1. 在Salesforce中，转到“设置”页面。

1. 在快速查找中搜索用户档案并选择 **个人资料** 选项。

1. 单击 **新建配置文件** 按钮进行修改。

1. 选取要克隆的配置文件并为其命名（例如： Sales Insight User）。

1. 单击 **保存** 完成时。

## 添加Sales Insight权限 {#add-sales-insight-permissions}

1. 返回您的“配置文件”列表。

1. 单击 **编辑** 您刚刚创建的新用户档案的链接（或者您希望授予Sales Insight访问权限的任何其他现有用户档案的链接）。

1. 在编辑页面上，您需要更改一些设置。

   **对于允许访问销售分析的用户档案**：

   * 在选项卡设置中，将Marketo选项卡更改为默认开启
   * 在“自定义对象权限”中，选中Marketo Sales Insight Config上的读取、创建、编辑和删除（如果用户应有权访问配置设置 — 通常用于管理员）

   **对于不允许访问销售分析的用户档案**：

   * 在选项卡设置中，将Marketo选项卡更改为隐藏选项卡
   * 在“自定义对象权限”中，取消选中Marketo Sales Insight Config中的“读取”、“创建”、“编辑”和“删除”

1. 单击 **保存** 完成时。

## 为销售分析创建布局 {#create-layout-for-sales-insight}

1. 转到“设置”页面，然后单击 **应用程序设置** > **自定义** > **潜在客户** > **页面布局**. 然后单击 **新** 按钮。

1. 克隆您选择的布局，并为该布局提供一个适当的名称（例如： Sales Insight Layout ）。

1. 单击 **保存** 完成时。

1. 对您的Contacts 、 Opportunity和Accounts页面布局重复这些步骤。

## 将配置文件分配给布局 {#assign-profile-to-layout}

1. 返回页面布局部分，然后单击 **页面布局分配** 按钮。

1. 选择 **编辑分配**.

1. 从列表中选择您的Sales Insight配置文件，然后从“选择页面布局”下拉列表中选择您的Sales Insight布局。

1. 单击 **保存** 完成时。

1. 对您的Contacts 、 Opportunity和Accounts页面布局重复这些步骤。

## 其他更改 {#other-changes}

下面是其他可能会显示销售分析项目的位置。 由于无法使用用户档案限制其访问，因此您必须直接删除这些用户档案：

* 从“搜索布局”中删除“销售分析”按钮，以查找联系人、潜在客户和客户
* 从联系人和潜在客户列表中删除Sales Insight列

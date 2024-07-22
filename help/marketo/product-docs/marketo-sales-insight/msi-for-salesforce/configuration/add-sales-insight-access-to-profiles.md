---
description: 添加对用户档案的销售分析访问权限 — Marketo文档 — 产品文档
title: 添加对用户档案的销售分析访问权限
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# 添加对用户档案的销售分析访问权限 {#add-sales-insight-access-to-profiles}

下面是如何创建有权访问Sales Insight的用户档案，同时删除对其他用户档案的访问权限。 适用于已安装[Sales InsightAppExchange包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}的用户。

>[!IMPORTANT]
>
>如果您以前授予了销售分析访问所有配置文件的权限，则您必须[删除配置文件级访问权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"}才能使用此权限集。

## 为Sales Insight创建新配置文件 {#create-a-new-profile-for-sales-insight}

如果您有专门针对Sales Insight用户的用户档案，则可以跳过此步骤。

1. 在Salesforce中，转到“设置”页面。

1. 在“快速查找”中搜索配置文件，并选择&#x200B;**配置文件**&#x200B;选项。

1. 单击页面顶部的&#x200B;**新建配置文件**&#x200B;按钮。

1. 选取要克隆的配置文件并为其命名（例如： Sales Insight User）。

1. 完成后单击&#x200B;**保存**。

## 添加Sales Insight权限 {#add-sales-insight-permissions}

1. 返回您的“配置文件”列表。

1. 单击您刚刚创建的新配置文件（或要授予Sales Insight访问权限的任何其他现有配置文件）的&#x200B;**编辑**&#x200B;链接。

1. 在编辑页面上，您需要更改一些设置。

   **对于允许访问Sales Insight**&#x200B;的用户档案：

   * 在选项卡设置中，将Marketo选项卡更改为默认开启
   * 在“自定义对象权限”中，选中Marketo Sales Insight Config上的“读取”、“创建”、“编辑”和“删除”（如果用户应有权访问配置设置，通常用于管理员）

   **对于不允许访问Sales Insight**&#x200B;的用户档案：

   * 在选项卡设置中，将Marketo选项卡更改为选项卡隐藏
   * 在“自定义对象权限”中，取消选中“Marketo销售分析配置”中的“读取”、“创建”、“编辑”和“删除”

1. 完成后单击&#x200B;**保存**。

## 创建销售分析布局 {#create-layout-for-sales-insight}

1. 转到“设置”页面，然后单击&#x200B;**应用程序设置** > **自定义** > **潜在客户** > **页面布局**。 然后单击&#x200B;**新建**&#x200B;按钮。

1. 克隆您选择的布局，并为该布局提供一个适当的名称（例如： Sales Insight Layout ）。

1. 完成后单击&#x200B;**保存**。

1. 对您的Contacts 、 Opportunity和Accounts页面布局重复这些步骤。

## 将配置文件分配给布局 {#assign-profile-to-layout}

1. 返回页面布局部分，然后单击&#x200B;**页面布局分配**&#x200B;按钮。

1. 选择&#x200B;**编辑分配**。

1. 从列表中选择您的Sales Insight配置文件，然后从“选择页面布局”下拉列表中选择您的Sales Insight布局。

1. 完成后单击&#x200B;**保存**。

1. 对您的Contacts 、 Opportunity和Accounts页面布局重复这些步骤。

## 其他更改 {#other-changes}

下面是其他可能会显示销售分析项目的位置。 您将必须彻底删除它们，因为无法使用配置文件限制其访问权限：

* 从“搜索布局”中删除“销售分析”按钮，以查找联系人、潜在客户和帐户
* 从联系人和潜在客户列表中删除Sales Insight列

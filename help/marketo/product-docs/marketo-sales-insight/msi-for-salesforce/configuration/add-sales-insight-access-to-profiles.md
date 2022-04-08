---
description: 向用户档案添加Sales Insight访问权限 — Marketo文档 — 产品文档
title: 向用户档案添加Sales Insight访问权限
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 向用户档案添加Sales Insight访问权限 {#add-sales-insight-access-to-profiles}

以下是如何在删除其他用户档案的访问权限时，创建具有Sales Insight访问权限的用户档案。 这适用于已安装 [Sales InsightAppExchange包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target=&quot;_blank&quot;}。

>[!IMPORTANT]
>
>如果您之前已授予Sales Insight对所有配置文件的访问权限，则必须 [删除配置文件级别访问权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target=&quot;_blank&quot;}使用此权限集。

## 为Sales Insight创建新配置文件 {#create-a-new-profile-for-sales-insight}

如果您的Sales Insight用户具有专用配置文件，则可以跳过此步骤。

1. 在Salesforce中，转到“设置”页面。

1. 在快速查找中搜索用户档案，然后选择 **用户档案** 选项。

1. 单击 **新建用户档案** 按钮。

1. 选择要克隆的配置文件并为其指定名称(例如：Sales Insight用户)。

1. 单击 **保存** 完成时。

## 添加销售分析权限 {#add-sales-insight-permissions}

1. 返回至用户档案列表。

1. 单击 **编辑** 链接，以获取您刚刚创建的新配置文件（或您要授予Sales Insight访问权限的任何其他现有配置文件）。

1. 在编辑页面上，您需要更改一些设置。

   **对于允许访问Sales Insight的用户档案**:

   * 在“选项卡设置”中，将“Marketo”选项卡更改为“默认启用”
   * 在“自定义对象权限”中，选中Marketo Sales Insight配置中的读取、创建、编辑和删除（如果用户应有权访问配置设置 — 通常用于管理员）

   **对于不允许访问Sales Insight的用户档案**:

   * 在“选项卡设置”中，将“Marketo”选项卡更改为“隐藏的选项卡”
   * 在“自定义对象权限”中，取消选中“在Marketo Sales Insight配置中读取、创建、编辑和删除”


1. 单击 **保存** 完成时。

## 为销售分析创建布局 {#create-layout-for-sales-insight}

1. 转到“设置”页面，然后单击 **应用程序设置** > **自定义** > **潜在客户** > **页面布局**. 然后，单击 **新建** 按钮。

1. 克隆所选布局并为布局指定适当的名称(例如：销售分析布局)。

1. 单击 **保存** 完成时。

1. 为您的“联系人”、“机会”和“帐户”的页面布局重复这些步骤。

## 将配置文件分配给布局 {#assign-profile-to-layout}

1. 返回到“页面布局”部分，然后单击 **页面布局分配** 按钮。

1. 选择 **编辑分配**.

1. 从列表中选择您的销售分析配置文件，然后从“选择页面布局”下拉列表中选择您的销售分析布局。

1. 单击 **保存** 完成时。

1. 为您的“联系人”、“机会”和“帐户”的页面布局重复这些步骤。

## 其他更改 {#other-changes}

以下是可能显示销售分析项目的其他一些位置。 由于无法使用用户档案限制其访问，因此您必须直接删除这些用户档案：

* 从“联系人”、“潜在客户”和“帐户”的“搜索布局”中删除“销售分析”按钮
* 从“联系人”和“潜在客户”列中删除“销售分析”列

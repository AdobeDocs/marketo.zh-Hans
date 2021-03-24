---
description: 为团队 — Marketo Docs — 产品文档设置Sales Insight
title: 为团队设置销售分析
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# 为您的团队{#setting-up-sales-insight-for-your-team}设置销售分析

下面介绍如何在删除对其他用户档案的访问权限时创建具有Sales Insight访问权限的用户档案。 这适用于已安装[Sales InsightAppExchange包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)的用户。

## 为Sales Insight创建新用户档案{#create-a-new-profile-for-sales-insight}

如果您有专门的Sales Insight用户用户档案，您可以跳过此步骤。

1. 在Salesforce中，转到设置页面。

1. 在“快速查找”中搜索用户档案，然后选择&#x200B;**用户档案**&#x200B;选项。

1. 单击页面顶部的&#x200B;**新建用户档案**&#x200B;按钮。

1. 选择要克隆的用户档案，并为其命名(例如：Sales Insight用户)。

1. 完成后，单击&#x200B;**保存**。

## 添加Sales Insight权限{#add-sales-insight-permissions}

1. 返回用户档案列表。

1. 单击您刚刚创建的新用户档案(或您要授予Sales Insight Access权限的任何其他现有用户档案)的&#x200B;**Edit**&#x200B;链接。

1. 在编辑页面上，您需要更改一些设置。

   **对于允许访问Sales Insight的用户档案**:

   * 在“自定义应用程序设置”中，选中Marketo以使Marketo应用程序可见
   * 在“选项卡设置”中，将“市场营销”选项卡更改为“默认开启”
   * 在“自定义对象权限”中，选中“在Marketo Sales Insight配置上读取、创建、编辑和删除”（如果用户应有权访问配置设置 — 通常用于管理员）

   **对于不允许访问Sales Insight的用户档案**:

   * 在“自定义应用程序设置”中，取消选中“营销”以隐藏Marketo应用程序
   * 在“选项卡设置”中，将“标记”选项卡更改为“选项卡隐藏”
   * 在“自定义对象权限”中，取消选中“在Marketo Sales Insight配置上读取、创建、编辑和删除”


1. 完成后，单击&#x200B;**保存**。

## 为Sales Insight {#create-layout-for-sales-insight}创建布局

1. 转到“设置”页，然后单击&#x200B;**应用程序设置** > **自定义** > **潜在客户** > **页面布局**。 然后单击&#x200B;**新建**&#x200B;按钮。

1. 仿制所选布局，并为布局指定适当的名称(例如：Sales Insight Layout)。

1. 完成后，单击&#x200B;**保存**。

1. 为您的“联系人”、“业务机会”和“帐户”页面布局重复这些步骤。

## 将用户档案分配给布局{#assign-profile-to-layout}

1. 返回“页面布局”部分并单击&#x200B;**“页面布局分配”**&#x200B;按钮。

1. 选择&#x200B;**编辑分配**。

1. 从列表中选择您的销售分析用户档案，然后从“选择页面布局”下拉菜单中选择您的销售分析布局。

1. 完成后，单击&#x200B;**保存**。

1. 为您的“联系人”、“业务机会”和“帐户”页面布局重复这些步骤。

## 其他更改{#other-changes}

以下是Sales Insight项目可能显示的其他位置。 您必须直接删除它们，因为您不能使用用户档案限制它们的访问：

* 从联系人、潜在客户和帐户的搜索布局中删除“销售分析”按钮
* 从“联系人”和“潜在客户”列表中删除“销售分析”列

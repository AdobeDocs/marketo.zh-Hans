---
description: 添加Insight销售人员对配置文件的访问权限 — Marketo文档 — 产品文档
title: 添加Sales Insight对配置文件的访问权限
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 添加[!DNL Sales Insight]对配置文件的访问权限 {#add-sales-insight-access-to-profiles}

下面说明了如何在删除其他配置文件的访问权限的同时创建具有[!DNL Sales Insight]访问权限的配置文件。 适用于已安装[[!DNL Sales Insight] AppExchange包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}的用户。

>[!IMPORTANT]
>
>如果您之前授予[!DNL Sales Insight]对所有配置文件的访问权限，则您必须[移除配置文件级别访问权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"}才能使用此权限集。

## 为[!DNL Sales Insight]创建新配置文件 {#create-a-new-profile-for-sales-insight}

如果您有[!DNL Sales Insight]个用户的专用配置文件，则可以跳过此步骤。

1. 在[!DNL Salesforce]中，转到“设置”页面。

1. 在快速查找中搜索配置文件并选择&#x200B;**[!UICONTROL Profile]**&#x200B;选项。

1. 单击页面顶部的&#x200B;**[!UICONTROL New Profile]**&#x200B;按钮。

1. 选取要克隆的配置文件并为其命名(例如： Sales Insight User)。

1. 完成后单击&#x200B;**[!UICONTROL Save]**。

## 添加[!DNL Sales Insight]权限 {#add-sales-insight-permissions}

1. 返回您的“配置文件”列表。

1. 单击刚刚创建的新配置文件（或要授予&#x200B;**[!UICONTROL Edit]**&#x200B;访问权限的任何其他现有配置文件）的[!DNL Sales Insight]链接。

1. 在编辑页面上，您需要更改一些设置。

   **对于允许访问[!DNL Sales Insight]**&#x200B;的配置文件：

   * 在选项卡设置中，将Marketo选项卡更改为默认开启
   * 在自定义对象权限中，选中[!DNL Marketo Sales Insight]配置中的读取、创建、编辑和删除（如果用户应有权访问配置设置 — 通常用于管理员）

   **对于不允许访问[!DNL Sales Insight]**&#x200B;的配置文件：

   * 在选项卡设置中，将Marketo选项卡更改为选项卡隐藏
   * 在“自定义对象权限”中，取消选中[!DNL Marketo Sales Insight]配置上的读取、创建、编辑和删除

1. 完成后单击&#x200B;**[!UICONTROL Save]**。

## 为[!DNL Sales Insight]创建布局 {#create-layout-for-sales-insight}

1. 转到设置页面，然后单击&#x200B;**[!UICONTROL App Setup]** > **[!UICONTROL Customize]** > **[!UICONTROL Leads]** > **[!UICONTROL Page Layouts]**。 然后单击&#x200B;**[!UICONTROL New]**&#x200B;按钮。

1. 克隆您选择的布局，并为该布局提供一个适当的名称(例如： Sales Insight Layout)。

1. 完成后单击&#x200B;**[!UICONTROL Save]**。

1. 对您的[!UICONTROL Contacts]、[!UICONTROL Opportunities]和[!UICONTROL Accounts]页面布局重复这些步骤。

## 将配置文件分配给布局 {#assign-profile-to-layout}

1. 返回页面布局部分，然后单击&#x200B;**[!UICONTROL Page Layout Assignment]**&#x200B;按钮。

1. 选择 **[!UICONTROL Edit Assignment]**。

1. 从列表中选择您的[!DNL Sales Insight]配置文件，然后从“[!DNL Sales insight]”下拉列表中选择您的[!UICONTROL Select Page Layout]布局。

1. 完成后单击&#x200B;**[!UICONTROL Save]**。

1. 对您的[!UICONTROL Contacts]、[!UICONTROL Opportunities]和[!UICONTROL Accounts]页面布局重复这些步骤。

## 其他更改 {#other-changes}

以下是可能显示[!DNL Sales Insight]个项目的其他位置。 您将必须彻底删除它们，因为无法使用配置文件限制其访问权限：

* 从[!DNL Sales Insight]、[!UICONTROL Contacts]和[!UICONTROL Leads]的搜索布局中删除[!UICONTROL Accounts]按钮
* 从联系人和潜在客户列表中删除[!DNL Sales Insight]列

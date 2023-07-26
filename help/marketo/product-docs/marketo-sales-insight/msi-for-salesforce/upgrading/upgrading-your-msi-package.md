---
unique-page-id: 37357050
description: 升级MSI包 — Marketo文档 — 产品文档
title: 升级MSI包
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 升级MSI包 {#upgrading-your-msi-package}

1. 导航到 [appexchange中的此页面](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target="_blank"}.

1. 从步骤一的页面右上角登录Salesforce实例(连接到Marketo实例的实例，可以是沙盒或生产实例)。 您必须具有管理员权限才能在Salesforce中安装/升级托管包。

1. 单击 **立即获取** 按钮。 系统将要求您选择要安装的位置。 您将可以选择升级，因为您已经拥有以前版本的MSI。 根据您在第一步中登录的帐户选择一个选项。

   >[!TIP]
   >
   >我们建议您在升级生产实例之前，在沙盒实例上测试此设置。

1. 您可以通过选择“仅为管理员安装”（并在以后提供对特定配置文件的MSI访问）、“为所有用户安装”或“为特定配置文件安装”来升级包。 在此示例中，我们选择“仅限管理员”。 作出选择后，单击 **升级**.

   ![](assets/four.png)

>[!NOTE]
>
>建议您仅更新管理员包，然后 [提供对特定用户的访问权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"} 基于购买的MSI名额。 或者，您也可以为MSI用户创建特定的Salesforce配置文件，并仅为这些用户安装或升级包。

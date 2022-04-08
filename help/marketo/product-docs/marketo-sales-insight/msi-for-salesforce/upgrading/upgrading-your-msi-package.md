---
unique-page-id: 37357050
description: 升级MSI包 — Marketo文档 — 产品文档
title: 升级MSI包
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# 升级MSI包 {#upgrading-your-msi-package}

1. 导航到 [appexchange中的此页面](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target=&quot;_blank&quot;}。

1. 从步骤1的页面右上角登录到Salesforce实例(与Marketo实例连接的实例可以是沙盒或生产实例)。 您必须具有管理员权限才能在Salesforce中安装/升级托管包。

1. 单击 **立即获取** 按钮。 系统将要求您选择要安装的位置。 由于您之前已拥有MSI版本，因此将可选择升级。 根据您在步骤1中登录的帐户选择一个选项。

   >[!TIP]
   >
   >我们建议您在升级生产实例之前，在沙盒实例上测试此实例。

1. 您可以通过选择“仅为管理员安装”（稍后为特定配置文件提供MSI访问权限）、“为所有用户安装”或“为特定配置文件安装”来升级包。 在本例中，我们选择“仅管理员”。 进行选择后，单击 **升级**.

   ![](assets/four.png)

>[!NOTE]
>
>建议您仅为管理员更新包，然后 [提供对特定用户的访问权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;}，基于购买的MSI席位数。 或者，您可以为MSI用户创建特定的Salesforce配置文件，并仅为这些用户安装或升级包。

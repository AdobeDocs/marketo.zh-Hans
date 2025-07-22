---
unique-page-id: 37357050
description: 升级MSI包 — Marketo文档 — 产品文档
title: 升级MSI包
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 升级MSI包 {#upgrading-your-msi-package}

>[!IMPORTANT]
>
>由于Salesforce进行了安全增强，Sales Insight包无法再向标准对象授予权限。 今后，Sales Insight用户的Salesforce配置文件需要具有以下标准对象的读取权限：潜在客户、联系人、客户和机会。 [在此了解如何进行配置](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#grant-sales-insight-users-profile-access){target="_blank"}。

1. 在appexchange[中导航到](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target="_blank"}此页面。

1. 从步骤一的页面右上角登录[!DNL Salesforce]实例(连接到Marketo实例的实例，可以是沙盒或生产实例)。 您必须具有管理员权限才能在[!DNL Salesforce]中安装/升级托管包。

1. 单击&#x200B;**立即获取**&#x200B;按钮。 系统将要求您选择要安装的位置。 您将可以选择升级，因为您已经拥有以前版本的MSI。 根据您在第一步中登录的帐户选择一个选项。

   >[!TIP]
   >
   >我们建议您在升级生产实例之前，在沙盒实例上测试此设置。

1. 您可以通过选择“仅为管理员安装”（并在以后提供对特定配置文件的MSI访问）、“为所有用户安装”或“为特定配置文件安装”来升级包。 在此示例中，我们选择“仅限管理员”。 选择完毕后，单击&#x200B;**升级**。

   ![](assets/four.png)

>[!NOTE]
>
>建议仅更新管理员程序包，然后[根据购买的MSI名额向特定用户提供访问权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}。 或者，您也可以为MSI用户创建特定的Salesforce配置文件，并仅为这些用户安装或升级包。

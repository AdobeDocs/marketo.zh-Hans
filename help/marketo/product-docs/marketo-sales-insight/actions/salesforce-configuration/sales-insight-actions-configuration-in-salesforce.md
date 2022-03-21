---
description: Salesforce中的Sales Insight Actions配置 — Marketo文档 — 产品文档
title: Salesforce中的Sales Insight操作配置
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: f2f81167066c2f170f81308b2deec52d19efafb3
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Salesforce中的Sales Insight操作配置 {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [安装](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) 或 [升级](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Salesforce实例中的Sales Insight包
>* [在Salesforce企业/无限制中配置Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)


## 在Salesforce中添加新的远程站点 {#add-new-remote-site-in-salesforce}

1. 在Salesforce中，单击 **设置**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. 搜索“远程站点”并选择 **远程站点设置**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. 单击 **新建远程站点**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. 输入远程站点名称（可以是类似于“MarketoSalesInsight”的内容）。 输入远程站点URL(https://ims-na1-stg1.adobelogin.com)，然后单击 **保存**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

## 在CRM中启用Sales Insight操作 {#enabling-sales-insight-actions-across-the-crm}

1. 在Salesforce中，单击 **Marketo Sales Insight配置** 选项卡。

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >如果您在顶部栏中未看到“Marketo Sales Insight配置”，请单击 **+** 在“All Tabs（所有选项卡）”下标记并查找。

1. 选择 **启用MSI操作** 复选框。

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. 输入API密钥。

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >如果您的API密钥不方便使用，则可以按照 [本文](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. 单击 **保存** 完成时。

这将自动启用功能概述文章中概述的所有MSI操作功能。

>[!NOTE]
>
>只需取消选中“启用MSI操作”复选框，即可禁用所有MSI操作功能。

## MSI-Actions管理 {#msi-actions-governance}

1. 您可以禁用“销售促销活动”和/或即将发布的部分中的任务选项卡。 这将适用于潜在客户、联系人、帐户和机会面板。

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. 您可以通过取消选中“操作”设置下的相应功能来禁用MSI操作。

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>管理设置适用于所有MSI用户。

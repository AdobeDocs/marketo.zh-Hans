---
description: Salesforce中的Sales Insight Actions配置 — Marketo文档 — 产品文档
title: Salesforce中的Sales Insight操作配置
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Salesforce中的Sales Insight操作配置 {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [安装](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) 或 [升级](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Salesforce实例中的Sales Insight包
>* [在Salesforce Enterprise/Unlimited中配置Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

## 在Salesforce中添加新的远程站点 {#add-new-remote-site-in-salesforce}

1. 在Salesforce中，单击 **设置**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. 搜索“远程站点”并选择 **远程站点设置**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. 单击 **新建远程站点**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. 输入远程站点名称（可以类似于“MarketoSalesInsight1”）。 输入远程站点URL `https://ims-na1.adobelogin.com` 并单击 **保存**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. 单击 **新建远程站点** 再来一次。

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. 输入远程站点名称（可以是“MarketoSalesInsight2”）。 输入远程站点URL `https://mkto-sales-connect.adobe.io` 并单击 **保存**.

## 在整个CRM中启用销售分析操作 {#enabling-sales-insight-actions-across-the-crm}

1. 在Salesforce中，单击 **Marketo销售分析配置** 选项卡。

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >如果您在顶部栏中未看到“Marketo销售分析配置”，请单击 **+** 在所有选项卡下签名并找到它。

1. 选择 **启用MSI操作** 复选框。

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. 输入API密钥。

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >如果您没有可用的API密钥，可以按照中的步骤找到它 [本文](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. 单击 **保存** 完成时。

这将自动启用功能概述文章中概述的所有MSI Actions功能。

>[!NOTE]
>
>只需取消选中“启用MSI操作”复选框，即可禁用所有MSI操作功能。

## MSI操作管理 {#msi-actions-governance}

1. 您可以禁用即将到来的部分中的销售促销活动和/或任务选项卡。 这将适用于潜在客户、联系人、客户和机会面板。

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. 通过取消选中“操作”设置下的相应功能，可以禁用MSI操作。

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>治理设置适用于所有MSI用户。

---
unique-page-id: 7511512
description: 在Salesforce1中安装和配置Marketo Sales Insight - Marketo文档 — 产品文档
title: 在Salesforce1中安装和配置Marketo Sales Insight
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 1%

---

# 在Salesforce1中安装和配置Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>现有客户，请[升级MSI包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md)，然后再继续！

>[!PREREQUISITES]
>
>如果您拥有Salesforce Enterprise/Unlimited：
>
>* [第1步（共3步）：将Marketo字段添加到Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [第2步（共3步）：为Marketo (Enterprise/Unlimited)创建Salesforce用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [第3步（共3步）：连接Marketo和Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [在Salesforce Enterprise/Unlimited中配置Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>如果您拥有Salesforce Professional：
>
>* [在Salesforce Professional Edition中配置Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>Salesforce1中的Marketo Sales Insight包括：最佳匹配、潜在客户源、有趣的时刻和添加到Marketo Campaign。

## 启用Salesforce1移动设备应用程序 {#enable-the-salesforce1-mobile-app}

1. 单击&#x200B;**设置**，然后单击&#x200B;**移动设备管理**。

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. 单击&#x200B;**Salesforce1**。

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. 单击&#x200B;**Salesforce1设置**。

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. 单击&#x200B;**启用Salesforce1移动浏览器应用程序**。

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. 单击&#x200B;**保存**。

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. 选择&#x200B;**移动设备管理**。

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. 单击&#x200B;**管理移动导航菜单**。

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. 选择&#x200B;**Marketo**&#x200B;和&#x200B;**将其添加到**&#x200B;选定的&#x200B;**菜单项**。

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. 选择&#x200B;**Marketo**，将其&#x200B;**向上**&#x200B;移动到所需区域，然后单击&#x200B;**保存**。

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## 隐藏过期的Marketo自定义对象 {#hide-outdated-marketo-custom-object}

1. 单击&#x200B;**设置**。

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. 选择&#x200B;**管理用户**。

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. 选择&#x200B;**配置文件**。

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. 单击以&#x200B;**编辑**&#x200B;任何所需的配置文件。

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. 在&#x200B;**选项卡设置**&#x200B;下，选择&#x200B;_第一个_ **Marketo**。

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. 选择&#x200B;**隐藏的选项卡**。

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >请确保为所有所需的配置文件隐藏Marketo选项卡！

## 自定义选项卡 {#customize-tabs}

1. 单击&#x200B;**+**。

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. 单击&#x200B;**自定义我的选项卡**。

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. 选择&#x200B;**Marketo**&#x200B;和&#x200B;**将其添加到所选选项卡**。

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. 选择&#x200B;**Marketo**，将其&#x200B;**向上**&#x200B;移动到所需区域，然后单击&#x200B;**保存**。

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## 自定义页面布局 {#customize-page-layouts}

1. 单击&#x200B;**设置**。

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. 单击“**设置**”，键入&#x200B;**页面布局**，然后单击“潜在客户”下的&#x200B;**页面布局**。

   >[!NOTE]
   >
   >对您的组织使用的每个页面布局（营销、销售等）重复这些步骤 对于Contact 、 Account和Opportunity对象。

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. 单击&#x200B;**编辑**&#x200B;以更改潜在客户布局。

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. 单击&#x200B;**Visualforce Pages**，然后将&#x200B;**潜在移动设备**&#x200B;拖到移动设备卡部分。

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. 将高度更改为66，然后单击&#x200B;**确定**。

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. 单击&#x200B;**字段**&#x200B;并将&#x200B;**添加到Marketo促销活动**&#x200B;拖到&#x200B;**Marketo销售分析**&#x200B;部分。

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >在快速查找中键入“Add to”，以便轻松查找添加到Marketo Campaign的内容。

1. 单击&#x200B;**保存**。

   ![](assets/image2015-4-22-18-3a1-3a56.png)

噢！ 您终于完成了Marketo Sales Insight for Salesforce1的安装！ 请拍拍自己的后背。

>[!MORELIKETHIS]
>
>* [Salesforce中的最佳匹配1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* Salesforce中的[有趣时刻1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [在Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)中发送Marketo电子邮件和Campaign及监视列表操作

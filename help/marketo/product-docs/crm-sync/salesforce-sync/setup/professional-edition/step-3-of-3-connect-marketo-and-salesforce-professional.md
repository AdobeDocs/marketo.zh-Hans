---
unique-page-id: 3571800
description: 第3步（共3步） — Connect Marketo和Salesforce(Professional)- Marketo文档 — 产品文档
title: 第3步（共3步） — 连接Marketo和Salesforce(Professional)
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# 第3步，共3步：连接Marketo和Salesforce(Professional){#step-of-connect-marketo-and-salesforce-professional}

在本文中，您将配置Marketo以与已配置的Salesforce实例同步。

>[!PREREQUISITES]
>
>* [第1步，共3步：将Marketo字段添加到Salesforce(Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [第2步，共3步：为Marketo(Professional)创建Salesforce用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)


## 检索同步用户安全令牌{#retrieve-sync-user-security-token}

>[!TIP]
>
>如果您已经拥有安全令牌，请直接继续设置同步用户凭据和备份！

1. 使用Marketo Sync用户登录Salesforce，单击同步用户的名称，然后单击&#x200B;**我的设置**。

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. 在Nav搜索栏中，键入“reset”并单击&#x200B;**重置我的安全令牌**。

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. 单击&#x200B;**重置安全令牌**。

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   安全令牌将通过电子邮件发送给您。

## 设置同步用户凭据{#set-sync-user-credentials}

1. 在Marketo中，转至&#x200B;**Admin**，选择&#x200B;**CRM**，然后单击&#x200B;**与[Salesforce.com](https://Salesforce.com)**&#x200B;同步。

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >在单击&#x200B;**同步字段**&#x200B;之前，请务必从同步用户中隐藏Marketo中不需要](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md)的所有字段。 [单击“同步字段”后，用户可以看到的所有字段都将在Marketo中永久创建，并且无法删除。

1. 输入在Salesforce配置的第2部分([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)、[Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md))中创建的Salesforce同步用户凭据，然后单击&#x200B;**同步字段**。

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >如果要将Marketo沙箱同步到Salesforce沙箱，请检查&#x200B;**沙箱**。

1. 阅读警告，然后单击&#x200B;**确认凭据**。

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >如果要查看[映射并自定义它们](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)，这是您唯一这样做的机会！ 单击“开始 Salesforce同步”后，即可完成。

## 开始Salesforce同步{#start-salesforce-sync}

1. 单击&#x200B;**开始Salesforce同步**&#x200B;以开始永久的Marketo-Salesforce同步。

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo不会针对Salesforce同步或在您手动输入潜在客户时自动进行重复数据消除。

1. 单击&#x200B;**开始同步**。

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >完成初始同步的时间因数据库的大小和复杂性而异。

## 验证同步{#verify-sync}

Marketo在“管理”区域中为Salesforce同步提供状态消息。 您可以按照以下步骤验证同步是否正常工作。

1. 在Marketo中，单击&#x200B;**Admin**，然后单击&#x200B;**Salesforce**。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同步状态显示在右上角。 它将显示以下三个信息之一：**上次同步**、**正在同步**&#x200B;或&#x200B;**失败**。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

哇，您刚刚完成了Marketo最强大功能之一的配置，开始吧！

>[!MORELIKETHIS]
>
>* [在SalesforceAppExchange中安装Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [在Salesforce专业版中配置Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)


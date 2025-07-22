---
unique-page-id: 2360366
description: 第3步（共3步） — 连接Marketo和Salesforce (Enterprise/Unlimited) - Marketo文档 — 产品文档
title: 第3步（共3步） — 连接Marketo和Salesforce (Enterprise/Unlimited)
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# 第3步（共3步）：连接Marketo和[!DNL Salesforce] (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

在本文中，您将将Marketo配置为与配置的[!DNL Salesforce]实例同步。

>[!PREREQUISITES]
>
>* [第1步（共3步）：将Marketo字段添加到 [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [第2步（共3步）：为Marketo (Enterprise/Unlimited)创建 [!DNL Salesforce] 用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)

## 检索同步用户安全令牌 {#retrieve-sync-user-security-token}

>[!TIP]
>
>如果您已经具有安全令牌，请直接进入“设置同步用户凭据”和“称号”以进行准备！

1. 使用Marketo同步用户登录[!DNL Salesforce]，单击同步用户的名称，然后单击&#x200B;**[!UICONTROL My Settings]**。

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. 在快速查找中，键入“reset”并单击&#x200B;**[!UICONTROL Reset My Security Token]**。

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. 单击 **[!UICONTROL Reset Security Token]**。

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   安全令牌将通过电子邮件发送给您。

## 设置同步用户凭据 {#set-sync-user-credentials}

1. 在Marketo中，转到&#x200B;**[!UICONTROL Admin]**，选择&#x200B;**CRM**，然后单击&#x200B;**[!UICONTROL Sync with Salesforce.com]**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >在单击[之前，请确保向同步用户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md)隐藏Marketo中所有不需要的字段&#x200B;**[!UICONTROL Sync Fields]**。 单击[!UICONTROL Sync Fields]后，将在Marketo中永久创建该用户可以查看的所有字段且无法将其删除。

1. 输入在[!DNL Salesforce]配置的第2部分中创建的[!DNL Salesforce]同步用户凭据（[Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)或[Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)），然后单击&#x200B;**[!UICONTROL Sync Fields]**(仅当您将Marketo沙盒同步到&#x200B;**[!UICONTROL Sandbox]**&#x200B;沙盒时才选中[!DNL Salesforce])。

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >如果您看到“登录到[!DNL Salesforce]”按钮而不是用户名/密码/令牌字段，则会为OAuth启用您的Marketo订阅。 请[参阅此文章](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md)。 使用一组凭据开始同步后，**不会切换[!DNL Salesforce]凭据或订阅**。 如果您希望使用基本身份验证，请联系您的客户成功经理。

1. 阅读警告，然后单击&#x200B;**[!UICONTROL Confirm Credentials]**。

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >如果要查看[映射并自定义它们](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)，这是您唯一的选择！ 单击[!UICONTROL Start  Salesforce Sync]后，操作即完成。

## 启动[!DNL Salesforce]同步 {#start-salesforce-sync}

1. 单击&#x200B;**[!UICONTROL Start  Salesforce Sync]**&#x200B;开始永久性Marketo-[!DNL Salesforce]同步。

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo不会针对[!DNL Salesforce]同步或手动输入潜在客户时自动执行重复数据删除。

1. 单击 **[!UICONTROL Start Sync]**。

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >完成初始同步的时间因数据库的大小和复杂性而异。

## 验证同步 {#verify-sync}

Marketo在管理区域为[!DNL Salesforce]同步提供状态消息。 您可以按照以下步骤验证同步是否正常工作。

1. 在Marketo中，单击&#x200B;**[!UICONTROL Admin]**，然后单击&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同步状态将显示在右上角。 它将显示以下三条消息之一：**[!UICONTROL Last Synced]**、**[!UICONTROL Sync in Progress]**&#x200B;或&#x200B;**[!UICONTROL Failed]**。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

您刚刚完成了Marketo最强大功能的配置，现在就开始！

>[!MORELIKETHIS]
>
>* [第1步（共3步）：将Marketo字段添加到 [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [第2步（共3步）：为Marketo (Enterprise/Unlimited)创建 [!DNL Salesforce] 用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [在 [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)中安装Marketo Sales Insight包
>* [在 [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)中配置Marketo Sales Insight

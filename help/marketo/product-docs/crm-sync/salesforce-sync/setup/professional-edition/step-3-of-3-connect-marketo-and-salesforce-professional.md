---
unique-page-id: 3571800
description: 第3步（共3步） — 连接Marketo和Salesforce（专业） - Marketo文档 — 产品文档
title: 第3步（共3步） — 连接Marketo和Salesforce（专业）
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# 第3步（共3步）：连接Marketo和[!DNL Salesforce] （专业） {#step-of-connect-marketo-and-salesforce-professional}

在本文中，您将配置Marketo Engage以与配置的Salesforce实例同步。

>[!PREREQUISITES]
>
>* [第1步（共3步）：将Marketo字段添加到Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}
>* [第2步（共3步）：为Marketo (Professional)创建Salesforce用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"}

## 检索同步用户安全令牌 {#retrieve-sync-user-security-token}

>[!TIP]
>
>如果您已经具有安全令牌，请直接进入“设置同步用户凭据”和“称号”以进行准备！

1. 使用Marketo同步用户登录Salesforce，单击同步用户的名称，然后单击&#x200B;**[!UICONTROL My Settings]**。

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. 在导航搜索栏中，键入“reset”并单击&#x200B;**[!UICONTROL Reset My Security Token]**。

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. 单击 **[!UICONTROL Reset Security Token]**。

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   安全令牌将通过电子邮件发送给您。

## 设置同步用户凭据 {#set-sync-user-credentials}

1. 在Marketo中，转到&#x200B;**[!UICONTROL Admin]**，选择&#x200B;**[!UICONTROL CRM]**，然后单击&#x200B;**[!UICONTROL Sync with Salesforce.com]**。

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >在单击[之前，请确保向同步用户](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"}隐藏Marketo中所有不需要的字段&#x200B;**[!UICONTROL Sync Fields]**。 单击“同步字段”后，该用户可以看到的所有字段都将在Marketo中永久创建，并且无法删除。

1. 输入在Salesforce配置第2部分中创建的Salesforce同步用户凭据([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)， [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md))，然后单击&#x200B;**[!UICONTROL Sync Fields]**。

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >如果您正在将Marketo沙盒同步到Salesforce沙盒，请选中&#x200B;**[!UICONTROL Sandbox]**。

1. 阅读警告，然后单击&#x200B;**[!UICONTROL Confirm Credentials]**。

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >如果要查看[映射并自定义它们](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md){target="_blank"}，这是您唯一的选择！ 单击“启动Salesforce同步”后，该操作即完成。

## 启动[!DNL Salesforce]同步 {#start-salesforce-sync}

1. 单击&#x200B;**[!UICONTROL Start Salesforce Sync]**&#x200B;开始永久性Marketo-Salesforce同步。

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

1. 在Marketo中，单击&#x200B;**[!UICONTROL Admin]**，然后单击&#x200B;**Salesforce**。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同步状态将显示在右上角。 它将显示以下三条消息之一：**[!UICONTROL Last Synced]**、**[!UICONTROL Sync in Progress]**&#x200B;或&#x200B;**[!UICONTROL Failed]**。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

您刚刚完成了Marketo最强大功能的配置，现在就开始！

>[!MORELIKETHIS]
>
>* [在Salesforce AppExchange中安装Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [在Marketo Professional Edition中配置Salesforce Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md){target="_blank"}

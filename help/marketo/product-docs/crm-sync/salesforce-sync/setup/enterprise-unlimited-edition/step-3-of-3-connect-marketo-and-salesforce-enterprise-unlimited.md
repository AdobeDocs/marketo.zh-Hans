---
unique-page-id: 2360366
description: 第3步（共3步） — 连接Marketo和Salesforce (Enterprise/Unlimited) - Marketo文档 — 产品文档
title: 第3步（共3步） — 连接Marketo和Salesforce (Enterprise/Unlimited)
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# 第3步（共3步）：连接Marketo和Salesforce (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

在本文中，您将配置Marketo Engage以与配置的Salesforce实例同步。

>[!PREREQUISITES]
>
>* [第1步（共3步）：将Marketo字段添加到Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [第2步（共3步）：为Marketo (Enterprise/Unlimited)创建Salesforce用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}

## 检索同步用户安全令牌 {#retrieve-sync-user-security-token}

>[!TIP]
>
>如果您已经具有安全令牌，请直接进入“设置同步用户凭据”和“称号”以进行准备！

1. 使用Marketo同步用户登录Salesforce，单击同步用户的名称，然后单击&#x200B;**[!UICONTROL 我的设置]**。

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. 在快速查找中，键入“reset”，然后单击&#x200B;**[!UICONTROL 重置我的安全令牌]**。

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. 单击&#x200B;**[!UICONTROL 重置安全令牌]**。

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   安全令牌将通过电子邮件发送给您。

## 设置同步用户凭据 {#set-sync-user-credentials}

1. 在Marketo中，转到&#x200B;**[!UICONTROL 管理员]**，选择&#x200B;**[!UICONTROL CRM]**，然后单击&#x200B;**与[Salesforce.com](https://Salesforce.com)**&#x200B;同步

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >在单击&#x200B;**[!UICONTROL 同步字段]**&#x200B;之前，请确保向同步用户[隐藏Marketo中所有不需要的字段](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"}。 单击“同步字段”后，该用户可以看到的所有字段都将在Marketo中永久创建，并且无法删除。

1. 输入在Salesforce配置的第2部分中创建的Salesforce Sync User凭据（[Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"}或[Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}），然后单击&#x200B;**[!UICONTROL 同步字段]**(仅当将Marketo沙盒同步到Salesforce沙盒时，才选中&#x200B;**[!UICONTROL 沙盒]**)。

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >如果您看到“登录到Salesforce”按钮而不是“用户名/密码/令牌”字段，则会为OAuth启用Marketo订阅。 请[参阅此文章](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md){target="_blank"}。 一旦开始使用一组凭据进行同步，_就不会切换Salesforce凭据或订阅_。 如果要使用基本身份验证，请联系Adobe客户团队（您的客户经理）。

1. 阅读警告，然后单击&#x200B;**[!UICONTROL 确认凭据]**。

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >如果要查看[映射并自定义它们](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md){target="_blank"}，这是您唯一的选择！ 单击“启动Salesforce同步”后，该操作即完成。

## 启动Salesforce同步 {#start-salesforce-sync}

1. 单击&#x200B;**[!UICONTROL 启动Salesforce同步]**&#x200B;以开始永久性Marketo-Salesforce同步。

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo不会针对Salesforce同步或手动输入潜在客户时自动执行重复数据删除。

1. 单击&#x200B;**[!UICONTROL 开始同步]**。

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >完成初始同步的时间因数据库的大小和复杂性而异。

## 验证同步 {#verify-sync}

Marketo在管理区域为Salesforce同步提供状态消息。 您可以按照以下步骤验证同步是否正常工作。

1. 在Marketo中，单击&#x200B;**[!UICONTROL 管理员]**，然后单击&#x200B;**Salesforce**。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同步状态将显示在右上角。 它将显示以下三条消息之一：**[!UICONTROL 上次同步]**、**[!UICONTROL 正在同步]**&#x200B;或&#x200B;**[!UICONTROL 失败]**。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

您刚刚完成了Marketo最强大功能的配置，现在就开始！

>[!MORELIKETHIS]
>
>* [第1步（共3步）：将Marketo字段添加到Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [第2步（共3步）：为Marketo (Enterprise/Unlimited)创建Salesforce用户](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
>* [在SalesforceAppExchange中安装Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [在Salesforce Enterprise/Unlimited中配置Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md){target="_blank"}

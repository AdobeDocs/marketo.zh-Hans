---
description: 第3步（共3步） — ConnectMarketo Engage和Veeva CRM - Marketo文档 — 产品文档
title: 第3步（共3步） — 连接Marketo Engage和Veeva CRM
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# 第3步（共3步）：连接Marketo Engage和Veeva CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

在本文中，您将配置Marketo Engage以与配置的Veeva CRM实例同步。 **你会在弹出窗口中看到Salesforce** 因为Veeva CRM构建在Salesforce平台上。

>[!PREREQUISITES]
>
>* [第1步（共3步）：将Marketo字段添加到Veeva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [第2步（共3步）：为Marketo创建Veeva用户](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>一次只能将一个Marketo实例连接到Veeva CRM实例。

## 使用OAuth连接到Veeva CRM {#connect-to-veeva-crm-using-oauth}

1. 在Marketo中，单击 **管理员**. 选择 **CRM** 并单击 **与Veeva同步**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >请务必 [隐藏所有不需要的字段](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} Marketo ，然后再单击“同步字段”。 单击“同步字段”后，该用户可以看到的所有字段都将在Marketo中永久创建，并且无法删除。

1. 单击 **使用Veeva登录**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >如果您正在将Marketo沙盒同步到Veeva CRM沙盒，请选中沙盒。

1. 单击 **确认凭据**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. 此时将出现一个显示Salesforce登录页面的弹出窗口。 输入您的“Marketo同步用户”凭据，然后单击 **登录**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. 输入您通过电子邮件收到的验证码（由Salesforce发送），然后单击 **验证**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. 成功验证后，访问页面将显示请求访问。 单击 **允许**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. 几分钟后，Marketo Engae中将出现弹出窗口。 单击 **确认凭据**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## 启动Veeva同步 {#start-veeva-sync}

1. 单击 **启动Veeva同步** 开始永久性Marketo-Veeva CRM同步。

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo不会针对Veeva CRM同步或手动输入潜在客户时自动执行重复数据删除。

1. 单击 **开始同步**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>完成初始同步的时间因数据库的大小和复杂性而异。

## 验证同步 {#verify-sync}

Marketo在管理区域为Veeva CRM同步提供状态消息。 您可以按照以下步骤验证同步是否正常工作。

1. 在Marketo中，单击 **管理员**，则 **Veeva**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. 同步状态将显示在右上角。 它将显示以下三条消息之一：“上次同步”、“同步进行中”或“失败”。

>[!MORELIKETHIS]
>
>[配置自定义对象](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

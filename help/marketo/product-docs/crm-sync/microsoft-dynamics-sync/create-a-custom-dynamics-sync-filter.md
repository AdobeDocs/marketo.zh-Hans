---
unique-page-id: 9437903
description: 创建自定义 [!DNL Dynamics] 同步筛选器 — Marketo文档 — 产品文档
title: 创建自定义 [!DNL Dynamics] 同步筛选器
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
feature: Microsoft Dynamics
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 1%

---

# 创建自定义[!DNL Dynamics]同步筛选器 {#create-a-custom-dynamics-sync-filter}

Marketo允许您设置同步过滤器，并仅同步部分记录。

## 概述 {#overview}

要设置[!DNL Dynamics]同步筛选器：

1. 在Dynamics CRM中为任何对象（潜在客户、联系人、帐户、机会和其他自定义实体）创建名为`new_synctomkto`的自定义两个选项（布尔值）字段。
1. 为此字段分配一个“是”/“否”值。

您必须在Dynamics CRM(而非您的数据库或Marketo)中进行这些更改。

>[!CAUTION]
>
>如果不分配该字段并将其留空/NULL，它将同步但不会更新。 Dynamics CRM中字段值为空/空的记录将在Marketo中将此字段值显示为“false”。

Marketo在自动后台同步期间查找此字段，并根据此逻辑确定要同步哪些记录：

| 字段值 | 是否同步到Marketo？ |
|---|---|
| 字段不存在 | 是 |
| 字段为空 | 是 |
| 字段的值为Yes | 是 |
| 字段具有值否 | 否 |

>[!CAUTION]
>
>告知Marketo跳过记录的唯一方法是将字段值显式设置为&#x200B;**否**。 即使字段值为空，Marketo仍会通过同步记录。

>[!PREREQUISITES]
>
>安装最新版本的Marketo插件（3.0.0.1或更高版本）。 转到Marketo > [!UICONTROL Admin] > [!DNL Microsoft Dynamics] > [!UICONTROL Download Marketo Solution]。

## 创建SyncToMkto字段 {#create-synctomkto-field}

1. 登录您的Dynamics CRM。 单击&#x200B;**设置**，然后单击&#x200B;**自定义项**。

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. 单击 **[!UICONTROL Customize the System]**。

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. 单击![](assets/image2015-8-10-21-3a44-3a23.png)旁边的&#x200B;**[!UICONTROL Entities]**。

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. 单击![](assets/image2015-8-10-21-3a44-3a23.png)旁边的&#x200B;**[!UICONTROL Lead]**&#x200B;并选择&#x200B;**[!UICONTROL Fields]**。 接着，单击 **[!UICONTROL New]**。

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. 在&#x200B;**字段中输入** SyncToMkto **[!UICONTROL Display Name]**&#x200B;并选择&#x200B;**[!UICONTROL Two Options]**&#x200B;作为&#x200B;**[!UICONTROL Data Type]**。 接着，单击 **[!UICONTROL Save and Close]**。

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >为该字段选择任意显示名称，但“名称”字段必须正好是&#x200B;**new_synctomkto**。 您必须使用&#x200B;**new**&#x200B;作为默认前缀。 如果已更改默认值，请转到此处[重置自定义字段名称](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md){target="_blank"}的默认前缀。 创建新字段后，可以更改回原始字段。

   >[!NOTE]
   >
   >如果设置了异步工作流，记录将获取您在字段中设置的默认SyncToMkto值，并在工作流完成运行时几秒钟后获取正确的值。 如果默认值设置为“是”，则将在Marketo中创建这些记录，然后这些记录会过时。 使用&#x200B;**否**&#x200B;作为默认值以避免此情况。

1. 重复此过程并为要限制同步的任何其他实体（如联系人、帐户、商机和自定义实体）创建&#x200B;**SyncToMkto**&#x200B;字段。

## 在Marketo中选择筛选器 {#select-the-filter-in-marketo}

即使您已完成初始同步，请转到并选择要与Marketo同步的字段。

1. 转到管理员并选择&#x200B;**[!UICONTROL Microsoft Dynamics]**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击字段同步详细信息中的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到字段并选中。 实际名称必须是new_synctomkto ，但“显示名称”可以是任何内容。 单击 **[!UICONTROL Save]**。

   ![](assets/image2015-10-9-9-3a56-3a23.png)

非常好，现在您已为Marketo启用同步过滤器。

## 创建[!DNL Dynamics]工作流以自动分配同步筛选器值 {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

您始终可以手动为记录的SyncToMkto字段分配值。 但是，为什么不利用[!DNL Dynamics]工作流的强大功能并在创建或更新记录时自动为SyncToMkto字段分配值？

>[!NOTE]
>
>不能在数据库级别执行此操作。 必须在CRM中手动或使用工作流完成此操作。
>
>[!DNL Dynamics]工作流仅适用于以后创建的新记录，而不适用于历史数据。 使用批次更新在现有记录上移动。

1. 转到您的Dynamics CRM。 单击&#x200B;**设置**，然后单击&#x200B;**进程**。

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. 单击 **[!UICONTROL New]**。

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. 输入工作流的名称，并选择&#x200B;**[!UICONTROL Workflow]**&#x200B;作为[!UICONTROL Category]，**[!UICONTROL Lead]**&#x200B;作为[!UICONTROL Entity]。 然后单击&#x200B;**确定**。

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. 创建规则以根据您组织的偏好为&#x200B;**SyncToMkto**&#x200B;字段分配true或false值。 单击 **[!UICONTROL Save and Close]**。

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >在单击&#x200B;**[!UICONTROL Add Step]**&#x200B;添加Check Condition后定义默认操作。 这会设置您不想同步到&#x200B;**否**&#x200B;的记录。 否则，它们将同步。

1. 选择工作流并单击&#x200B;**[!UICONTROL Activate]**。

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >请参阅电子邮件地址的[自定义同步筛选器规则](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}，以设置规则只同步具有电子邮件地址的人员的记录。

## 同步筛选器详细信息 {#sync-filter-details}

以下是我们认为您应了解的一些实施详细信息：

* 启动同步操作

  当&#x200B;**SyncToMkto**&#x200B;值从&#x200B;**No**&#x200B;更改为&#x200B;**Yes**&#x200B;时，[!DNL Dynamics]会立即通知Marketo开始同步此记录。 如果记录已存在，则Marketo会更新它。 否则，Marketo将创建记录。

* 停止同步操作

  当记录将其SyncToMkto值从“是”更改为“否”时，Marketo将收到停止同步此记录的通知。 但是，不会删除记录，而是会停止获取更新并变得过时。

>[!MORELIKETHIS]
>
>* [Microsoft Dynamics同步筛选器：符合条件](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md){target="_blank"}
>* [Microsoft Dynamics同步筛选器：合并](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md){target="_blank"}
>* [电子邮件地址的自定义同步筛选器规则](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}

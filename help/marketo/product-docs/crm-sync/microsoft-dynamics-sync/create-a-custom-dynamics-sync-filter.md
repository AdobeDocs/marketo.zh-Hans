---
unique-page-id: 9437903
description: 创建自定义Dynamics同步筛选器 — Marketo Docs — 产品文档
title: 创建自定义Dynamics同步筛选器
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# 创建自定义Dynamics同步筛选器{#create-a-custom-dynamics-sync-filter}

是否不希望将Dynamics CRM中的所有内容同步到Marketo? 别担心！ Marketo允许您设置同步过滤器并仅同步部分记录。

## 概述{#overview}

要设置Dynamics同步筛选器：

1. 在Dynamics CRM中为任何对象（潜在客户、联系人、帐户、业务机会和其他自定义实体）创建名为new_synctomkto的自定义“两个选项”（布尔值）字段。
1. 为此字段指定“是”/“否”值，或将其留空。

>[!NOTE]
>
>您必须在Dynamics CRM中进行这些更改，而不是数据库或Marketo。

Marketo在自动后台同步过程中查找此字段，并根据此逻辑确定要同步的记录：

| 字段值 | 同步到Marketo? |
|---|---|
| 字段不存在 | 是 |
| 字段为空 | 是 |
| 字段的值为是 | 是 |
| 字段的值为否 | 否 |

>[!CAUTION]
>
>告诉Marketo跳过记录的唯一方法是将字段值显式设置为&#x200B;**否**。 即使字段值为空，Marketo仍会同步记录。

>[!PREREQUISITES]
>
>安装最新版Marketo插件（3.0.0.1或更高版本）。 转到Marketo >管理> Microsoft Dynamics >下载Marketo解决方案。

## 创建SyncToMkto字段{#create-synctomkto-field}

1. 登录Dynamics CRM。 单击&#x200B;**设置**，然后单击&#x200B;**自定义**。

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. 单击&#x200B;**自定义系统**。

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. 单击&#x200B;**实体**&#x200B;旁边的![](assets/image2015-8-10-21-3a44-3a23.png)。

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. 单击&#x200B;**Lead**&#x200B;旁边的![](assets/image2015-8-10-21-3a44-3a23.png)，然后选择&#x200B;**字段**。 然后单击&#x200B;**新建**。

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. 在&#x200B;**显示名称**&#x200B;字段中输入&#x200B;**SyncToMkto**，然后选择&#x200B;**两个选项**&#x200B;作为&#x200B;**数据类型**。 然后单击&#x200B;**保存并关闭**。

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >为此字段选择任何显示名称，但“名称”字段必须恰好为&#x200B;**new_synctomkto**。 必须使用&#x200B;**new**&#x200B;作为默认前缀。 如果您更改了默认值，请转到[重置自定义字段名称的默认前缀](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md)。 在创建新字段后，可以将其更改回。

   >[!NOTE]
   >
   >如果您设置了异步工作流，记录将获取您在字段中设置的默认SyncToMkto值，并在工作流完成运行后几秒后获取正确值。 如果将默认值设置为“是”，则这些记录将在Marketo中创建，然后变得陈旧。 请使用&#x200B;**否**&#x200B;作为默认值以避免出现这种情况。

1. 重复此过程，并为希望限制同步的任何其他实体（如联系人、帐户、业务机会和自定义实体）创建&#x200B;**SyncToMkto**&#x200B;字段。

## 选择Marketo {#select-the-filter-in-marketo}中的筛选器

即使您已经完成了初始同步，请进入并选择要与Marketo同步的字段。

1. 转至“管理员”并选择&#x200B;**MiCrosoft Dynamics**。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击“字段同步详细信息”上的&#x200B;**编辑**。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到该字段并检查它。 实际名称必须是new_synctomkto，但“显示名称”可以是任何内容。 单击&#x200B;**保存**。

   ![](assets/image2015-10-9-9-3a56-3a23.png)

太好了，现在您已为Marketo启用了同步筛选器。

## 创建动态工作流以自动分配同步筛选器值{#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

您始终可以手动为记录的SyncToMkto字段分配一个值。 但是，在创建或更新记录时，为什么不充分利用Dynamics工作流的强大功能并自动为SyncToMkto字段分配值？

>[!NOTE]
>
>无法在数据库级别执行此操作。 必须在CRM中手动或使用工作流来完成。
>
>Dynamics工作流仅适用于将来创建的新记录，而不适用于历史数据。 使用批更新移至现有记录上。

1. 转到Dynamics CRM。 单击&#x200B;**设置**，然后单击&#x200B;**进程**。

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. 单击&#x200B;**新建**。

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. 输入工作流的名称，然后选择&#x200B;**工作流**&#x200B;作为类别，选择&#x200B;**潜在客户**&#x200B;作为实体。 然后单击&#x200B;**确定**。

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. 创建规则，以根据您的组织的首选项为&#x200B;**SyncToMkto**&#x200B;字段分配真值或假值。 单击&#x200B;**保存并关闭**。

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >单击&#x200B;**添加步骤**&#x200B;添加检查条件后，定义默认操作。 这将设置不想同步到&#x200B;**否**&#x200B;的记录。 否则，它们将同步。

1. 选择工作流，然后单击&#x200B;**激活**。

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >请参阅[电子邮件地址的自定义同步筛选器规则](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md)，以设置规则，仅同步具有电子邮件地址的人员的记录。

## 同步筛选器详细信息{#sync-filter-details}

以下是我们认为您应该了解的一些实施详细信息：

1. 开始同步操作

   当&#x200B;**SyncToMkto**&#x200B;值从&#x200B;**No**&#x200B;更改为&#x200B;**Yes**&#x200B;时，Dynamics会立即通知Marketo开始同步此记录。 如果记录已存在，Marketo会更新它。 否则，Marketo会创建记录。

   >[!TIP]
   >
   >发生此情况时，将向Marketo日志添加`Create [StartSync]`操作。

1. 停止同步操作

   当记录将其SyncToMkto值从“是”更改为“否”时，将通知Marketo停止同步此记录。 但是，该记录未被删除，而是会停止获取更新并变得陈旧。

>[!MORELIKETHIS]
>
>* [Microsoft Dynamics同步筛选器：资格](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md)
>* [Microsoft Dynamics同步筛选器：合并](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md)
>* [电子邮件地址的自定义同步筛选器规则](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md)


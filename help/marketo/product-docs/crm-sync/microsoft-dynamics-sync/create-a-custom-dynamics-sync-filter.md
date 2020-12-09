---
unique-page-id: 9437903
description: 创建自定义Dynamics同步筛选器- Marketo Docs —— 产品文档
title: 创建自定义Dynamics同步筛选器
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 0%

---


# 创建自定义Dynamics同步筛选器 {#create-a-custom-dynamics-sync-filter}

您不想将Dynamics CRM中的所有内容同步到Marketo? 别担心！ Marketo允许您设置同步过滤器并仅同步部分记录。

## 概述 {#overview}

要设置Dynamics同步筛选器，请执行以下操作：

1. 在Dynamics CRM中为任何对象（潜在客户、联系人、帐户、业务机会和其他自定义实体）创建一个名为new_synctomkto的自定义“两个选项”（布尔值）字段。
1. 为此字段指定“是／否”值，或将其留空。

>[!NOTE]
>
>您必须在Dynamics CRM中进行这些更改，而不是在数据库或Marketo中进行。

Marketo在自动后台同步过程中查找此字段，并根据此逻辑确定要同步的记录：

| 字段值 | 同步到Marketo? |
|---|---|
| 字段不存在 | 是 |
| 字段为空 | 是 |
| 字段的值为是 | 是 |
| 字段的值为否 | 否 |

>[!CAUTION]
>
>告诉Market跳过记录的唯一方法是将字段值显式设置为 **否**。 即使字段值为空，Marketo仍会同步记录。

>[!PREREQUISITES]
>
>安装最新版Marketo插件（3.0.0.1或更高版本）。 转到Marketo >管理> Microsoft Dynamics >下载Marketo Solution。

## 创建SyncToMkto字段 {#create-synctomkto-field}

1. 登录Dynamics CRM。 单击 **设置** ，然后单击 **自定义**。

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. 单击 **“Customize the System**”。

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. 单击 ![](assets/image2015-8-10-21-3a44-3a23.png) “实体”( **Entities)旁边**。

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. 单 ![](assets/image2015-8-10-21-3a44-3a23.png) 击“**潜在客户**”旁边的，然后选择“ **字段**”。 然后，单击 **“新建**”。

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. 在“显 **示名** ”字 **段中输入SyncToMkto** ，然后选择两 **个选项** ，作为“数 ****&#x200B;据类型”。 然后，单 **击保存并关闭**。

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >为此字段选择任何显示名称，但“名称”字段必须完全 **是new_synctomkto**。 必须使用 **new** 作为默认前缀。 如果已更改默认字段，请转到此 [处重置自定义字段名称的默认前缀](create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md)。 在创建新字段后，可以重新更改它。

   >[!NOTE]
   >
   >如果您设置了异步工作流，记录将获取您在字段中设置的默认SyncToMkto值，并在工作流完成运行后几秒钟后获取正确的值。 如果默认值设置为“是”，则这些记录将在Marketo中创建，然后变得陈旧。 请 **使用** “否”作为默认值以避免此情况。

1. 重复此过程，并为 **要限制同步** （如联系人、帐户、业务机会和自定义实体）的任何其他实体创建SyncToMkto字段。

## 选择Marketo中的筛选器 {#select-the-filter-in-marketo}

即使您已经完成了初始同步，请进入并选择要与Marketo同步的字段。

1. 转至“管理员”并选 **择“Microsoft Dynamics**”。

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. 单击“ **字段同步** ”详细信息上的“编辑”。

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. 向下滚动到字段并进行检查。 实际名称必须是new_synctomkto，但显示名称可以是任何内容。 单击 **保存**。

   ![](assets/image2015-10-9-9-3a56-3a23.png)

很好，现在您已启用了Marketo的同步过滤器。

## 创建动态工作流以自动分配同步筛选器值 {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

您始终可以为记录手动为SyncToMkto字段分配值。 但是，在创建或更新记录时，为什么不充分利用Dynamics Workflow的强大功能并自动为SyncToMkto字段分配值？

>[!NOTE]
>
>不能在数据库级别执行此操作。 它必须在CRM中手动或使用工作流来完成。
>
>Dynamics工作流只适用于将来创建的新记录，而不适用于历史数据。 使用批更新移至现有记录。

1. 转至Dynamics CRM。 单击 **设置** ，然后单 **击进程**。

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. 单击 **新建**。

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. 输入工作流的名称，然后选择 **工作流** 作为类别, **并选择潜在** 客户作为实体。 然后，单 **击确定**。

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. 创建规则，根据您组织的首 **选项** ，为SyncToMkto字段分配真值或假值。 单击 **保存并关闭**。

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >单击添加步骤以添加检查条 **件后** ，定义默认操作。 这会将您不想同步的记录设置为“ **否”**。 否则，它们将同步。

1. 选择工作流，然后单击 **激活**。

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >请参 [阅电子邮件地址的自定义同步过滤规则](create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md) ，以设置规则，仅同步具有电子邮件地址的人员的记录。

## 同步筛选器详细信息 {#sync-filter-details}

以下是我们认为您应该了解的一些实施详细信息：

1. 开始同步操作

   当SyncToMkto **值从** No变 **为Yes时** ,Dynamics会通 **知Market**，立即开始同步此记录。 如果记录已存在，Marketo将更新它。 否则，Marketo将创建记录。

   >[!TIP]
   >
   >发 **生此 [情况时]** ，将向Marketo日志添加Create StartSync操作。

1. 停止同步操作

   当记录将其SyncToMkto值从“是”更改为“否”时，将通知Marketo停止同步此记录。 但是，该记录并未删除，而是会停止获取更新并变得陈旧。

>[!NOTE]
>
>**相关文章**
>
>* [Microsoft Dynamics同步筛选器：资格](create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md)
>* [Microsoft Dynamics同步筛选器：合并](create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md)
>* [电子邮件地址的自定义同步筛选器规则](create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md)

>




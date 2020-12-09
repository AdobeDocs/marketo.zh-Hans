---
unique-page-id: 2953471
description: SFDC Sync —— 自定义对象同步- Marketo Docs —— 产品文档
title: SFDC同步——自定义对象同步
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---


# SFDC同步：自定义对象同步 {#sfdc-sync-custom-object-sync}

在Salesforce实例中创建的自定义对象也可以是Marketo的一部分。  下面介绍如何设置。

>[!NOTE]
>
>**需要管理员权限**

>[!PREREQUISITES]
>
>要使用自定义对象，它必须与Salesforce中的潜在客户 [、联系](sfdc-sync-lead-sync.md)[](sfdc-sync-contact-sync.md)人 [](sfdc-sync-account-sync.md)帐户对象关联。

## 启用自定义对象  {#enable-custom-object}

1. 单 **击** “管理员”和** Salesforce对象同步 **链接**。**

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. 如果这是您的第一个自定义对象，请单击“同 **步”模式。**

   ![](assets/rtaimage-2.png)

1. 单击“ **禁用全局同步”。**

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Salesforce自定义对象模式的初始同步可能需要几分钟时间。

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. 将要同步的自定义对象拖入画布。

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >自定义对象必须具有唯一名称。 Marketo不支持两个名称相同的不同自定义对象。

1. 单击 **启用同步。**

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. 再次单 **击“启用同** 步”。

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >不要忘记重新启用全局同步！

1. 返回**Salesforce **选项卡。

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. 单击 **启用同步。**

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. 要视图所有Salesforce自定义对象，请单 **击** “管理员”和** Salesforce对象同步**链接（与上面的步骤1相同）。

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo仅支持链接到标准实体（深度为一或两级）的自定义实体。

### 下一步： {#whats-next}

[添加／删除自定义对象字段作为智能列表/触发器约束](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

太棒了！ 您现在可以在智能活动和智能列表中使用此自定义对象中的数据。


---
unique-page-id: 4719297
description: 启用／禁用自定义对象同步- Marketo文档——产品文档
title: 启用／禁用自定义对象同步
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# 启用／禁用自定义对象同步 {#enable-disable-custom-object-sync}

在Salesforce实例中创建的自定义对象也可以是Marketo的一部分。 下面介绍如何设置。

## 启用／禁用自定义对象同步 {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>需要管理员权限。

1. 单击 **管理**。

   ** ![](assets/one.png)

   **

1. 在“数据库管理”菜单中，单 **击Salesforce****对象同步**。

   ![](assets/two-2.png)

1. 如果这是您的第一个自定义对象，请单击“同 **步”模式。** 否则，请 **单击“刷新模式** ”，以确保您拥有最新版本。

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. 如果全局同步正在运行，则必须单击“禁用全局同 **步”以禁用它。**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Salesforce自定义对象模式的同步可能需要几分钟时间。

1. 单击“ **刷新模式**”。

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. 选择要同步的对象，然后单击“启 **用同步”**。

   >[!TIP]
   >
   >Marketo只有与Salesforce中的潜在客户、联系人或帐户对象有直接关系时，才能同步自定义对象。

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. 再次单 **击“启用同** 步”。

   ** ![](assets/image2014-12-10-10-3a15-3a40.png)

   **

1. 返回Salesforce选 **项卡** ，然后单击 **启用同步**。

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## 使用自定义对象 {#using-your-custom-objects}

>[!NOTE]
>
>不能在智能活动中将自定义对象与触发器一起使用。

1. 在智能列表中，拖动Has **Opportunity过**&#x200B;滤器并设置为&#x200B;**true**。

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. 然后，使用过滤器约束来缩小焦点。

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   太棒了！ 您现在可以在智能活动和智能列表中使用此自定义对象的数据。

>[!MORELIKETHIS]
>
>* [添加／删除自定义对象字段作为智能列表/触发器约束](add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

>




---
unique-page-id: 3571846
description: Microsoft Dynamics Sync —— 自定义实体同步- Marketo Docs —— 产品文档
title: Microsoft Dynamics同步——自定义实体同步
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Microsoft Dynamics同步：自定义实体同步 {#microsoft-dynamics-sync-custom-entity-sync}

如果您需要启用初始自定义实体同步，以使Dynamics中的数据在Marketo中可用，下面将介绍如何实现。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>**先决条件**
>
>要使用自定义对象，它必须与Dynamics中的潜在客 [户](microsoft-dynamics-sync-lead-sync.md)、 [联系人](microsoft-dynamics-sync-contact-sync.md)或帐 [](microsoft-dynamics-sync-account-sync.md)户对象关联。

>[!CAUTION]
>
>在开始自定义实体的同步之前，请确保初始同步已完成（将通过电子邮件通知您）。

1. 转到“管理员”部分。

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. 单击 **“禁用同步** ”可临时禁用标准全局同步。

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. 安装支持自定义实体同步的Microsoft Dynamics版本（在2_0_0_2之后）。 请参 [阅Marketo Dynamics插件发行版](../../../../product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md)。
1. 为Marketo Sync用户授予对您计划同步的任何实体的读取权限。
1. 在“数据库管理”下，单击** Dynamics实体同步**链接。

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. 单击“ **同步模式** ”链接可转换可用自定义实体的列表。

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. 在列表同步后，选择要同步的字段和要在智能列表中用作 [约束](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) 和／或触发器的字段。 完成后，单击“启 **用同步**”。

   ![](assets/image2014-10-20-14-3a32-3a55.png)

1. 重新启用全局同步。

   ![](assets/image2015-11-10-9-3a48-3a35.png)

   >[!NOTE]
   >
   >Marketo仅支持链接到标准实体（深度为一或两级）的自定义实体。

   >[!NOTE]
   >
   >实体名称最多可包含** 33个字符**。

你很好！
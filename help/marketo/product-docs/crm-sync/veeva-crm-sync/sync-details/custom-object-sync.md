---
description: 自定义对象同步 — Marketo文档 — 产品文档
title: 自定义对象同步
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 自定义对象同步 {#custom-object-sync}

在Veeva CRM实例中创建的自定义对象也可以包含在Marketo Engage中。 下面是如何设置它。

>[!NOTE]
>
>**需要管理员权限**

>[!PREREQUISITES]
>
>要使用自定义对象，它必须与Veeva CRM中的联系人或帐户对象关联。

## 启用自定义对象 {#enable-custom-object}

1. 在Marketo中，单击 **管理员**，则 **Veeva对象同步**.

   ![](assets/custom-object-sync-1.png)

1. 如果这是您的第一个自定义对象，请单击 **同步架构**.

   ![](assets/custom-object-sync-2.png)

1. 单击 **禁用全局同步**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >Veeva自定义对象架构的初始同步可能需要几分钟时间。

1. 将您要同步的自定义对象拖到画布中。

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >自定义对象必须具有唯一名称。 Marketo不支持具有相同名称的两个不同的自定义对象。

1. 单击 **启用同步**.

   ![](assets/custom-object-sync-5.png)

1. 单击 **启用同步** 再次。

   ![](assets/custom-object-sync-6.png)

1. 返回到 **韦瓦** 选项卡。

   ![](assets/custom-object-sync-7.png)

1. 单击 **启用同步**.

   ![](assets/custom-object-sync-8.png)

1. 要查看所有Veeva自定义对象，请单击“管理”和“Veeva对象同步”。

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo仅支持链接到一到两级深度标准实体的自定义实体。

太棒了！ 现在，您可以在智能营销活动和智能列表中使用来自此自定义对象的数据。

>[!MORELIKETHIS]
>
>* [正在同步呼叫和呼叫密钥消息](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}
>* [将自定义对象字段添加/删除为智能列表/触发器约束](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target=&quot;_blank&quot;}


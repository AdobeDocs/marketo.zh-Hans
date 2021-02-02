---
unique-page-id: 10098379
description: 将Quick Sync with Microsoft Dynamics用于新的自定义字段- Marketo Docs —— 产品文档
title: 将快速同步与Microsoft Dynamics用于新的自定义字段
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# 对新自定义字段{#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}使用与Microsoft Dynamics快速同步

营销或销售部门需要一个新字段。 或者，您在初始字段选择中忘记了一个。 或者，您的需求已经改变。 无论如何，您都可以使用快速同步来重新同步特定字段。

通常，您将使用快速同步添加新字段并刷新值。 但是，在某些情况下，您可能希望同步现有字段。 您可以根据更新或创建的日期范围限制字段同步。 有关详细信息，请参阅下面的[高级同步选项](#Advanced_Sync_Options)。

快速同步可同步空值。 例如，如果您使用值A和B，并将Dynamics中的B值更改为null，它将null值同步到Marketo。

## 所有记录的快速同步{#quick-sync-for-all-records}

下面介绍如何使用快速同步重新同步新字段。

1. 在Marketo中，单击&#x200B;**管理**。

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. 单击&#x200B;**Microsoft Dynamics**。

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. 在“字段同步详细信息”中，单击&#x200B;**编辑**。

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. 选择要快速同步的字段，然后单击&#x200B;**保存**。

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >您可以从多个实体中选择字段。

1. 同步完成后，您将收到通知。

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >同步与其他同步并排运行，并且根据数据库的大小，完成该同步可能需要很长时间。 当字段在等待同步的队列中时，您无法取消选择该字段。

## 高级同步选项{#advanced-sync-options}

如果要同步现有字段，但仅对有限的数据集同步，该怎么办？ 这是方法。

1. 清除现有字段的复选框。 单击&#x200B;**保存**。

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. 再次打开弹出窗口并重新选择字段。

   ![](assets/select-field-reselect-hand.png)

1. 单击&#x200B;**高级同步**。

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. 选择&#x200B;**已更新**&#x200B;并使用日期选择器选择日期范围。 单击&#x200B;**保存**。

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   只有在8/19/16和9/19/16之间更新的记录才会为字段进行快速同步。

## 修复不同步字段{#fixing-out-of-sync-fields}

在极少数情况下，Dynamics和Marketo字段不同步，有一种快速、轻松的方法可重新同步它们。

1. 取消选择该字段，然后单击“保存”**。**

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. 重新选择字段，然后单击&#x200B;**保存**。 仅此而已！

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   那应该能解决！

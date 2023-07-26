---
unique-page-id: 10098379
description: 将与Microsoft Dynamics快速同步用于新的自定义字段 — Marketo文档 — 产品文档
title: 将与Microsoft Dynamics快速同步用于新自定义字段
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# 将与Microsoft Dynamics快速同步用于新自定义字段 {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

市场营销或销售人员需要一个新领域。 或者，也许你在初始字段选择中忘记了一个。 或者说，你的需求改变了。 在任何情况下，您都可以使用快速同步来重新同步特定字段。

通常，您将使用快速同步添加新字段并刷新值。 但是，在某些情况下，您可能希望同步现有字段。 您可以根据更新或创建的日期范围限制字段同步。 请参阅 [高级同步选项](#Advanced_Sync_Options) 详情请参阅下文。

快速同步可以同步Null值。 例如，如果您使用值A和B，并将Dynamics中的B值更改为null，则会将null值同步到Marketo。

## 快速同步所有记录 {#quick-sync-for-all-records}

以下是如何使用快速同步为新字段重新同步。

1. 在Marketo中，单击 **管理员**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. 单击 **Microsoft Dynamics**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. 在字段同步详细信息中，单击 **编辑**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. 选择要快速同步的字段，然后单击 **保存**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >您可以从多个实体中选择字段。

1. 同步完成后，您将收到通知。

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >同步与其他同步并排运行，根据数据库的大小，可能需要很长时间才能完成。 当字段在队列中等待同步时，不能取消选择它。

## 高级同步选项 {#advanced-sync-options}

如果要同步现有字段，但只针对有限的数据集执行同步操作，该怎么办？ 具体方法如下。

1. 清除现有字段的复选框。 单击 **保存**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. 再次打开弹出窗口并重新选择字段。

   ![](assets/select-field-reselect-hand.png)

1. 单击 **高级同步**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. 选择 **已更新** 并使用日期选取器选择日期范围。 单击 **保存**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   只有在2016年8月19日至2016年9月19日之间更新的记录才会在现场快速同步。

## 修复不同步的字段 {#fixing-out-of-sync-fields}

在极少数情况下，如果Dynamics和Marketo字段不同步，则可以快速轻松地重新同步它们。

1. 取消选择字段并单击 **保存**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. 重新选择字段并单击 **保存**. 仅此而已！

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   这应该能解决这个问题！

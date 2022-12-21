---
unique-page-id: 10098379
description: 使用与Microsoft Dynamics快速同步来获取新的自定义字段 — Marketo文档 — 产品文档
title: 使用与Microsoft Dynamics快速同步来获取新的自定义字段
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# 使用与Microsoft Dynamics快速同步来获取新的自定义字段 {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

营销或销售部门需要一个新字段。 或者，在最初的字段选择中，你可能忘记了一个。 或者，你的需求改变了。 无论如何，您都可以使用快速同步来重新同步特定字段。

通常，您会使用快速同步来添加新字段并刷新值。 但是，在某些情况下，您可能希望同步现有字段。 您可以根据更新或创建的日期范围限制字段同步。 请参阅 [高级同步选项](#Advanced_Sync_Options) 详情请参阅下文。

快速同步可以同步空值。 例如，如果您使用值A和B，并将Dynamics中的B值更改为null，则会将null值同步到Marketo。

## 所有记录的快速同步 {#quick-sync-for-all-records}

以下是如何使用“快速同步”对新字段重新同步的方法。

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
   >同步与其他同步并排运行，并且根据数据库的大小，完成同步可能需要很长时间。 当字段在待同步的队列中时，无法取消选择该字段。

## 高级同步选项 {#advanced-sync-options}

如果要同步现有字段，但仅对有限的数据集同步，该怎么办？ 这是方法。

1. 清除现有字段的复选框。 单击 **保存**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. 再次打开弹出窗口，然后重新选择字段。

   ![](assets/select-field-reselect-hand.png)

1. 单击 **高级同步**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. 选择 **已更新** ，然后使用日期选取器选择日期范围。 单击 **保存**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   只有8/19/16到9/19/16之间更新的记录才会为字段快速同步。

## 修复不同步字段 {#fixing-out-of-sync-fields}

在极少数情况下，如果Dynamics和Marketo字段不同步，可以快速轻松地重新同步它们。

1. 取消选择该字段并单击 **保存**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. 重新选择字段并单击 **保存**. 仅此而已！

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   那应该能解决！

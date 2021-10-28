---
unique-page-id: 2359418
description: 导入人员列表 — Marketo文档 — 产品文档
title: 导入人员列表
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
source-git-commit: a3da3f466e6131fdd3507b7b567fac91ad9c5b6c
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# 导入人员列表 {#import-a-list-of-people}

## 任务：将展会与会者的电子表格列表导入数据库 {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[设置并添加人员](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

在本教程中，您将学习如何将人员从电子表格文件导入Marketo。

## 步骤1:下载和编辑电子表格 {#step-download-and-edit-a-spreadsheet}

1. 要开始，请下载我们的实践电子表格文件([**tradeshow-tohates.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv))。

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >导入日期时，请使用以下格式： **9/21/20** （月/日/年）。

   >[!NOTE]
   >
   >正在导入的任何日期/时间字段都将被视为中央时间。 如果您的日期/时间字段位于不同的时区，则可以使用Excel公式将其转换为中部时间（美国/芝加哥）。

1. 添加您自己的名字、姓氏、实际电子邮件地址（以便您能够收到下次任务中将发送的培养电子邮件）和职位。 将文件保存在您的计算机上。

   ![](assets/image2014-9-24-12-3a5-3a30.png)

   >[!CAUTION]
   >
   >Marketo **not** 支持包含表情符号的电子邮件地址。

## 步骤2:创建项目 {#step-create-a-program}

1. 转到 **营销活动** 的上界。

   ![](assets/ma-2.png)

1. 选择 **学习** 文件夹，然后在 **新建** 单击 **新计划**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **名称** “我的贸易展项目”，并为 **程序类型**.

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. 选择 **贸易展** 对于 **渠道** 单击 **创建**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>事件程序在特定日期发生。 详细了解 [**事件**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md).

## 步骤3:将电子表格导入Marketo {#step-import-your-spreadsheet-into-marketo}

1. 在 **我的贸易展计划**，单击 **新建** 选择 **新建本地资产**.

   ![](assets/seven-3.png)

1. 单击 **列表**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **名称** 列出“展会与会者”，然后单击 **创建**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. 在 **展会与会者** 列表，单击 **列出操作** 选择 **导入列表**.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >如果您使用自己的CSV文件，请确保该文件已编码为UTF-8、UTF-16、Shift-JIS或EUC-JP。

   >[!NOTE]
   >
   >CSV文件的大小限制为100MB。

1. **浏览** 到 **tradeshow-tohates.csv** 在您的计算机上，单击 **下一个**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >在列表导入模式下，选择 **跳过新人员和更新** 意味着您不会影响现有人员记录或记录任何活动。 如果您希望在营销活动中使用现有人员的快速、预过滤静态列表，请使用此模式。 选择此模式将：
   >
   > * 跳过新人员创建
   > * 跳过人员字段更新
   > * 跳过活动日志记录


1. 将列表列字段映射到相应的Marketo字段，然后单击 **下一个**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >列标题应始终与字段完全匹配（区分大小写），以获得最佳的自动映射结果。 如果您使用自定义字段，但在下拉列表中未看到这些字段，请返回 [创建它们](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) 这样它们就能成为选择。

   >[!NOTE]
   >
   >如果有任何不想导入的字段，请选择 **忽略** (位于Marketo字段下拉菜单中)。

1. 选择 **我的贸易展计划** 对于 **客户获取计划**，然后单击 **导入**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. 等待人员导入，然后关闭导入进度弹出窗口。

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. 返回 **我的贸易展计划**，请单击 **成员** 选项卡。 你会看到刚进来的人。

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>您可以通过跟踪项目成员资格来分析项目是否成功。 详细了解 [**程序**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md).

## 任务完成 {#mission-complete}

您的贸易展与会者现在是您的Marketo计划的成员！

<br> 

[◄任务4:电子邮件自动响应](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[任务6:滴，滴，抚►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

---
unique-page-id: 2359418
description: 导入人员列表 — Marketo文档 — 产品文档
title: 导入人员列表
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
source-git-commit: 1b37a750c5e609b9e43e942df752305d85153989
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 导入人员列表 {#import-a-list-of-people}

## 任务：将展会与会者的电子表格列表导入数据库 {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[设置并添加人员](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

在本教程中，您将学习如何将人员从电子表格文件导入Marketo。

## 步骤1:下载和编辑电子表格 {#step-download-and-edit-a-spreadsheet}

1. 要开始，请将我们练习的电子表格文件([**tradeshow-retachests.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv))下载到您的计算机。

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >导入日期时，请使用以下格式：**9/21/20**（月/日/年）。

   >[!NOTE]
   >
   >正在导入的任何日期/时间字段都将被视为中央时间。 如果您的日期/时间字段位于不同的时区，则可以使用Excel公式将其转换为中部时间（美国/芝加哥）。

1. 添加您自己的名字、姓氏、电子邮件地址和职位，然后将文件保存到您的计算机上。

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>在CSV文件中输入您的真实电子邮件地址，以便您能够接收在下次任务中发送的培养电子邮件。

## 步骤2:创建项目 {#step-create-a-program}

1. 转到&#x200B;**营销活动**&#x200B;区域。

   ![](assets/ma-2.png)

1. 选择您的&#x200B;**Learning**&#x200B;文件夹，然后在&#x200B;**New**&#x200B;下单击&#x200B;**New Program**。

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **** 将程序命名为“My Tradeshow Program”，然后为“Program Type”选择“ **Event”**。

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. 为&#x200B;**Channel**&#x200B;选择&#x200B;**Tradeshow**，然后单击&#x200B;**创建**。

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>事件程序在特定日期发生。 了解有关&#x200B;[**Events**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md)&#x200B;的更多信息。

## 步骤3:将电子表格导入Marketo {#step-import-your-spreadsheet-into-marketo}

1. 在&#x200B;**My Tradeshow Program**&#x200B;中，单击&#x200B;**新建**，然后选择&#x200B;**新建本地资产**。

   ![](assets/seven-3.png)

1. 单击&#x200B;**列表**。

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **** 将列表命名为“贸易展与会者”，然后单击 **创建**。

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. 在&#x200B;**Tradeshow Requotess**&#x200B;列表中，单击&#x200B;**List Actions**&#x200B;并选择&#x200B;**Import List**。

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >如果您使用自己的CSV文件，请确保该文件已编码为UTF-8、UTF-16、Shift-JIS或EUC-JP。

   >[!NOTE]
   >
   >CSV文件的大小限制为100MB。

1. **** 浏览到您 **计算机上的tradeshow-athodes.** csvspreadsheet文件，然后单击 **下一步**。

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >在列表导入模式下，选择&#x200B;**跳过新人员和更新**&#x200B;意味着您不会影响现有人员记录或记录任何活动。 如果您希望在营销活动中使用现有人员的快速、预过滤静态列表，请使用此模式。 选择此模式将：
   >
   > * 跳过新人员创建
   > * 跳过人员字段更新
   > * 跳过活动日志记录


1. 将列表列字段映射到其各自的Marketo字段，然后单击&#x200B;**Next**。

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >列标题应始终与字段完全匹配（区分大小写），以获得最佳的自动映射结果。 如果您使用自定义字段，但在下拉列表中未看到这些字段，请返回并[创建它们](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)，以便它们成为选项。

   >[!NOTE]
   >
   >如果有任何不想导入的字段，请在“Marketo字段”下拉菜单中选择&#x200B;**忽略**。

1. 为&#x200B;**客户获取程序**&#x200B;选择&#x200B;**My Tradeshow Program**，然后单击&#x200B;**导入**。

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. 等待人员导入，然后关闭导入进度弹出窗口。

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. 返回&#x200B;**My Tradeshow Program**，单击&#x200B;**Members**&#x200B;选项卡。 你会看到刚进来的人。

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>您可以通过跟踪项目成员资格来分析项目是否成功。 了解有关&#x200B;[**程序**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)&#x200B;的更多信息。

## 任务完成 {#mission-complete}

您的贸易展与会者现在是您的Marketo计划的成员！

<br> 

[◄任务4:电子邮件自动响应](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[任务6:滴，滴，抚►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

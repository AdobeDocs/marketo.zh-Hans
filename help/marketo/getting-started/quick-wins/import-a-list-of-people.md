---
unique-page-id: 2359418
description: 导入人员列表 - Marketo 文档 - 产品文档
title: 导入人员列表
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '541'
ht-degree: 100%

---

# 导入人员列表 {#import-a-list-of-people}

## 任务：将展会与会人员的电子表格列表导入您的数据库 {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[完成设置并添加人员](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

在本教程中，您将学习如何将电子表格文件中的人员导入 Marketo。

## 步骤 1：下载并编辑电子表格 {#step-download-and-edit-a-spreadsheet}

1. 首先，将我们的示例电子表格文件（[**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"}）下载到您的计算机。

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >导入日期时，请使用此格式：**9/21/20**（月份/日期/年份）。

   >[!NOTE]
   >
   >导入的所有日期/时间字段将视为中部时间（Central Time）。如果您的日期/时间字段为其他时区，可以使用 Excel 公式将其转换为中部时间（美国/芝加哥）。

1. 添加您的名字、姓氏、真实电子邮件地址（以便在下一任务中接收您发送的培养邮件）和职位名称。将文件保存在您的计算机上。

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >* 请确保电子邮件地址仅包含 ASCII 字符。
   >
   >* Marketo **不**&#x200B;支持包含表情符号的电子邮件地址。
   >
   >* 通过 CSV 导入 `NULL` 值时，_即使这些字段为空_，也可能会在人员的[活动日志](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"}中生成“更改数据值”的记录。如果您有任何使用“数据值已更改”过滤器或“数据值更改”触发器的[智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target="_blank"}，即使数据实际上没有更改，也可能会使人员满足这些营销活动的条件。您可以使用[约束条件](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"}，确保在导入时无人符合这些营销活动的条件。

## 步骤 2：创建项目 {#step-create-a-program}

1. 进入 **[!UICONTROL Marketing Activities]** 区域。

   ![](assets/import-a-list-of-people-3.png)

1. 选择您的&#x200B;**学习**&#x200B;文件夹，然后在 **[!UICONTROL New]** 下点击 **[!UICONTROL New Program]**。

   ![](assets/import-a-list-of-people-4.png)

1. 将项目&#x200B;**命名**&#x200B;为“我的展会项目”，并将 **[!UICONTROL Program Type]** 选择为“活动”。

   ![](assets/import-a-list-of-people-5.png)

1. 将 **[!UICONTROL Channel]** 选择为 **[!UICONTROL Tradeshow]** 并点击 **[!UICONTROL Create]**。

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>活动项目会在特定日期进行。了解更多关于&#x200B;[**活动**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}&#x200B;的信息。

## 步骤 3：将电子表格导入 Marketo {#step-import-your-spreadsheet-into-marketo}

1. 在&#x200B;**我的展会项目**&#x200B;中，点击 **[!UICONTROL New]** 并选择 **[!UICONTROL New Local Asset]**。

   ![](assets/import-a-list-of-people-7.png)

1. 选择 **[!UICONTROL List]**。

   ![](assets/import-a-list-of-people-8.png)

1. 将列表&#x200B;**命名为**“展会与会人员”，然后点击 **[!UICONTROL Create]**。

   ![](assets/import-a-list-of-people-9.png)

1. 在您的 **[!UICONTROL Tradeshow Attendees]** 列表中，点击 **[!UICONTROL List Actions]** 并选择 **[!UICONTROL Import List]**。

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >如果您使用自己的 CSV 文件，请确保其编码为 UTF-8、UTF-16、Shift-JIS 或 EUC-JP。

   >[!NOTE]
   >
   >CSV 文件大小限制为 100MB。

1. 在您的计算机中 **[!UICONTROL Browse]** **tradeshow-attendees.csv** 电子表格文件并点击 **[!UICONTROL Next]**。

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >在列表导入模式中，选择 **[!UICONTROL Skip new people and updates]** 意味着不会影响现有人员记录或记录任何活动。如果您需要一个经过预筛选的现有人员静态列表用于营销活动，请使用此模式。选择此模式将会：
   >
   > * 跳过新人员创建
   > * 跳过人员字段更新
   > * 跳过活动日志记录

1. 将您的 [!UICONTROL List Column] 字段映射到相应的 Marketo 字段，然后点击 **[!UICONTROL Next]**。

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >列标题应与字段完全匹配（区分大小写），以获得最佳自动映射结果。如果您使用的是自定义字段且未在下拉列表中看到它们，请返回并[创建自定义字段](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}，这样它们才会显示为可选项。

   >[!NOTE]
   >
   >如果有不想导入的字段，请在 Marketo 字段下拉菜单中选择&#x200B;**忽略**。

1. 将 **[!UICONTROL Acquisition Program]** 选择为&#x200B;**我的展会项目**，然后点击 **[!UICONTROL Import]**。

   ![](assets/import-a-list-of-people-13.png)

1. 等待人员导入完成，然后关闭导入进度弹出窗口。

   ![](assets/import-a-list-of-people-14.png)

1. 返回&#x200B;**我的展会项目**，点击 **[!UICONTROL Members]** 选项卡。您将看到刚导入的所有人员。

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>您可以通过跟踪项目成员来分析项目的成功情况。进一步了解&#x200B;[**项目**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}。

## 任务完成 {#mission-complete}

您的展会与会人员现已成为 Marketo 项目的成员！

<br> 

[◄ 任务 4：电子邮件自动回复](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[任务 6：滴灌式培养►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

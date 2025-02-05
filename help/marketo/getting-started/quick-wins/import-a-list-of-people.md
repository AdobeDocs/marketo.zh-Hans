---
unique-page-id: 2359418
description: 导入人员列表 — Marketo文档 — 产品文档
title: 导入人员列表
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
feature: Getting Started
source-git-commit: 292626741d3b2334da104a515c3e968fb340706a
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# 导入人员列表 {#import-a-list-of-people}

## 任务：将贸易展会与会者的电子表格列表导入数据库 {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[设置并添加人员](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

在本教程中，您将了解如何将人员从电子表格文件导入Marketo。

## 步骤1：下载并编辑电子表格 {#step-download-and-edit-a-spreadsheet}

1. 若要开始，请将我们的练习电子表格文件([**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"})下载到您的计算机。

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >导入日期时，请使用此格式：**9/21/20**（月/日/年）。

   >[!NOTE]
   >
   >正在导入的任何日期/时间字段都将被视为中部时间。 如果您的日期/时间字段位于不同的时区，则可以使用Excel公式将其转换为中部时间（美洲/芝加哥）。

1. 添加您自己的名字、姓氏、实际电子邮件地址（这样您就可以接收将在下一个任务中发送的培养型电子邮件）以及职务。 将文件保存在计算机上。

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >* 确保电子邮件地址仅包含ASCII字符。
   >
   >* Marketo **不**&#x200B;支持包含表情符号的电子邮件地址。
   >
   >* 通过CSV导入`NULL`值可能会为人员的[活动日志](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"}、_中的数值字段生成“更改数据值”，即使这些字段已经为空_。 如果您有任何[智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target="_blank"}使用“数据值已更改”过滤器或“数据值更改”触发器，那么即使数据实际上并未更改，也可能导致人员符合这些营销活动的资格。 您可以使用[约束](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"}来确保在导入时没有任何人符合这些促销活动的条件。

## 第2步：创建项目 {#step-create-a-program}

1. 转到&#x200B;**[!UICONTROL 营销活动]**&#x200B;区域。

   ![](assets/import-a-list-of-people-3.png)

1. 选择您的&#x200B;**学习**&#x200B;文件夹，然后在&#x200B;**[!UICONTROL 新建]**&#x200B;下单击&#x200B;**[!UICONTROL 新建计划]**。

   ![](assets/import-a-list-of-people-4.png)

1. **命名**&#x200B;节目“我的商展节目”并为&#x200B;**[!UICONTROL 节目类型]**&#x200B;选择“事件”。

   ![](assets/import-a-list-of-people-5.png)

1. 为&#x200B;**[!UICONTROL 渠道]**&#x200B;选择&#x200B;**[!UICONTROL 商展]**&#x200B;并单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>事件程序在特定日期发生。 了解有关&#x200B;[**事件**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}&#x200B;的详细信息。

## 步骤3：将电子表格导入Marketo {#step-import-your-spreadsheet-into-marketo}

1. 在&#x200B;**我的商展计划**&#x200B;中，单击&#x200B;**[!UICONTROL 新建]**，然后选择&#x200B;**[!UICONTROL 新建本地资产]**。

   ![](assets/import-a-list-of-people-7.png)

1. 选择&#x200B;**[!UICONTROL 列表]**。

   ![](assets/import-a-list-of-people-8.png)

1. **将**&#x200B;命名为“商展与会者”列表，然后单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/import-a-list-of-people-9.png)

1. 在您的&#x200B;**[!UICONTROL 商展与会者]**&#x200B;列表中，单击&#x200B;**[!UICONTROL 列表操作]**&#x200B;并选择&#x200B;**[!UICONTROL 导入列表]**。

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >如果您使用自己的CSV文件，请确保该文件采用UTF-8、UTF-16、Shift-JIS或EUC-JP编码。

   >[!NOTE]
   >
   >CSV文件的大小限制为100MB。

1. **[!UICONTROL 浏览]**&#x200B;到您计算机上的&#x200B;**tradeshow-attendees.csv**&#x200B;电子表格文件，然后单击&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >在列表导入模式下，选择&#x200B;**[!UICONTROL 跳过新人员和更新]**&#x200B;意味着您将不会影响现有人员记录或记录任何活动。 如果您希望在营销活动中使用的现有人员的快速、预过滤静态列表，请使用此模式。 选择此模式将：
   >
   > * 跳过新人员创建
   > * 跳过人员字段更新
   > * 跳过活动日志记录

1. 将您的[!UICONTROL 列表列]字段映射到它们各自的Marketo字段，然后单击&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >列标题应始终与字段完全匹配（区分大小写），以获得最佳自动映射结果。 如果您正在使用自定义字段，但未在下拉列表中看到它们，请返回并[创建它们](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}，以便它们可以成为选项。

   >[!NOTE]
   >
   >如果有任何您不想导入的字段，请在Marketo字段下拉菜单中选择&#x200B;**忽略**。

1. 为&#x200B;**[!UICONTROL 客户获取计划]**&#x200B;选择&#x200B;**我的商展计划**，然后单击&#x200B;**[!UICONTROL 导入]**。

   ![](assets/import-a-list-of-people-13.png)

1. 等待人员导入，然后关闭导入进度弹出窗口。

   ![](assets/import-a-list-of-people-14.png)

1. 返回&#x200B;**我的商展计划**，单击&#x200B;**[!UICONTROL 成员]**&#x200B;选项卡。 您将看到所有您刚刚导入的人员。

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>您可以通过跟踪计划会员资格来分析计划是否成功。 了解有关&#x200B;[**程序**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}&#x200B;的更多信息。

## 任务完成 {#mission-complete}

您的商展与会者现在已成为Marketo计划的成员！

<br> 

[◄任务4：电子邮件自动响应](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[任务6：滴水、滴水、Nurture ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

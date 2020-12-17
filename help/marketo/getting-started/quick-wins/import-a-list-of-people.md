---
unique-page-id: 2359418
description: 导入人员列表- Marketo Docs —— 产品文档
title: 导入人员列表
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---


# 导入人员列表{#import-a-list-of-people}

## 任务：将trade show与会者的电子表格列表导入您的数据库{#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[设置并添加人物](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

在本教程中，您将学习如何将人员从电子表格文件导入Marketo。

## 第1步：下载并编辑电子表格{#step-download-and-edit-a-spreadsheet}

1. 要进行开始，请将我们的练习电子表格文件([**tradeshow-reatheeds.csv**](https://docs.marketo.com/display/docs/assets/tradeshow-attendees.csv))下载到您的计算机。

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >导入日期时，请使用以下格式：**9/21/20**（月／日/年）。

   >[!NOTE]
   >
   >导入的任何日期／时间字段均视为中央时间。 如果日期／时间字段位于其他时区，则可使用Excel公式将其转换为中时（美国／芝加哥）。

1. 添加您自己的名字、姓氏、电子邮件地址和职位，然后将文件保存在您的计算机上。

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>在CSV文件中输入您的真实电子邮件地址，以便您能够接收在下一个任务中发送的培育电子邮件。

## 第2步：创建项目{#step-create-a-program}

1. 转至&#x200B;**营销活动**&#x200B;区域。

   ![](assets/ma-2.png)

1. 选择&#x200B;**Learning**&#x200B;文件夹，然后在&#x200B;**New**&#x200B;下单击&#x200B;**New项目**。

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **将项目** 命名为“我的贸易展项目”，并选择“事件”作为 **项目类型**。

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. 为&#x200B;**渠道**&#x200B;选择&#x200B;**商展**，然后单击&#x200B;**创建**。

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>事件项目在特定日期发生。 进一步了解&#x200B;[**事件**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md)。

## 第3步：将电子表格导入Marketo {#step-import-your-spreadsheet-into-marketo}

1. 在&#x200B;**我的贸易展项目**&#x200B;中，单击&#x200B;**新建**&#x200B;并选择&#x200B;**新建本地资产**。

   ![](assets/seven-3.png)

1. 单击&#x200B;**列表**。

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **将列表** 命名为“贸易展与会者”，然后单击“ **创建”**。

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. 在&#x200B;**展会与会者**&#x200B;列表中，单击&#x200B;**列表操作**&#x200B;并选择&#x200B;**导入列表**。

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >如果您使用自己的CSV文件，请确保它采用UTF-8、UTF-16、Shift-JIS或EUC-JP编码。

   >[!NOTE]
   >
   >CSV文件的大小限制为100MB。

1. **浏** 览至计 **算机上的tradeshow-** reathers.csvspreadsheet文件，然后单击“下 **一步”**。

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >在列表导入模式中，选择&#x200B;**跳过新人和更新**&#x200B;表示您不会影响现有人员记录或记录任何活动。 如果您希望对现有人员进行快速、预过滤的静态列表，以便在营销活动中使用，请使用此模式。 选择此模式将：
   >
   > * 跳过新人创建
   > * 跳过人员字段更新
   > * 跳过活动记录


1. 将您的列表列字段映射到其各自的标记字段，然后单击&#x200B;**下一步**。

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >列标题应始终与字段完全匹配（区分大小写），以获得最佳自动映射结果。 如果您使用的是自定义字段，但在下拉列表中看不到这些字段，请返回并[创建它们](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)，以便它们成为选项。

   >[!NOTE]
   >
   >如果有任何您不想导入的字段，请在Marketo Field（市场营销字段）下拉菜单中选择&#x200B;**忽略**。

1. 为&#x200B;**客户获取项目**&#x200B;选择&#x200B;**我的贸易展项目**，然后单击&#x200B;**导入**。

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. 等待人员导入，然后关闭导入进度弹出窗口。

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. 返回至&#x200B;**我的贸易展项目**，单击&#x200B;**成员**&#x200B;选项卡。 您将看到您刚导入的所有人员。

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>您可以通过跟踪项目成员身份来分析项目的成功。 进一步了解&#x200B;[**项目**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)。

## 任务完成{#mission-complete}

您的贸易展与会者现在是您的营销人员项目的成员！

<br> 

[÷¿î:电子邮件自动响应](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[任务6:滴水，滴水，培养](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

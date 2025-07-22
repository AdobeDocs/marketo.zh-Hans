---
unique-page-id: 2951220
description: 使用Mobile Platform列构建人员绩效报表 — Marketo文档 — 产品文档
title: 使用Mobile Platform列构建人员绩效报表
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
feature: Reporting
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# 使用Mobile Platform列构建人员绩效报表 {#build-a-people-performance-report-with-mobile-platform-columns}

按照以下步骤创建使用Mobile Platform (iOS/Android)列的人员绩效报表。

## 创建移动设备智能列表 {#create-mobile-smart-lists}

1. 转到&#x200B;**[!UICONTROL Marketing Activities]**。

   ![](assets/ma.png)

1. 选择程序。

   ![](assets/two-1.png)

1. 在&#x200B;**[!UICONTROL New]**&#x200B;下，选择&#x200B;**[!UICONTROL New Local Asset]**。

   ![](assets/three-1.png)

1. 单击 **[!UICONTROL Smart List]**。

   ![](assets/four-1.png)

1. 键入名称并单击&#x200B;**[!UICONTROL Create]**。

   ![](assets/five-1.png)

1. 查找[!UICONTROL Opened Email]筛选器并将其拖到画布中。

   ![](assets/six-1.png)

1. 将电子邮件设置为&#x200B;**[!UICONTROL is any]**。

   ![](assets/seven.png)

1. 单击&#x200B;**[!UICONTROL Add Constraint]**&#x200B;并选择&#x200B;**[!UICONTROL Platform]**。

   ![](assets/eight.png)

   >[!TIP]
   >
   >在此示例中，我们使用了[!UICONTROL Opened Email]筛选器。 您还可以使用[!UICONTROL Clicked Email]筛选器，因为它具有Platform约束。

1. 将[!UICONTROL Platform]设置为&#x200B;**[!UICONTROL iOS]**。

   ![](assets/nine.png)

   >[!NOTE]
   >
   >必须至少有一个人在iOS设备上打开了您的某个电子邮件，Marketo的自动建议才能找到它。 如果未出现，您可以手动键入并保存。

   现在，为“Android”平台创建第二个智能列表。 完成后，转到下一部分。

## 创建人员绩效报表 {#create-a-people-performance-report}

1. 在营销活动下，选择包含您的&#x200B;**[!UICONTROL iOS]**&#x200B;和&#x200B;**[!UICONTROL Android]**&#x200B;智能列表的程序。

   ![](assets/ten.png)

1. 在&#x200B;**[!UICONTROL New]**&#x200B;下，选择&#x200B;**[!UICONTROL New Local Asset]**。

   ![](assets/eleven.png)

1. 单击 **[!UICONTROL Report]**。

   ![](assets/twelve.png)

1. 将类型设置为&#x200B;**[!UICONTROL People Performance]**。

   ![](assets/thirteen.png)

1. 单击 **[!UICONTROL Create]**。

   ![](assets/fourteen.png)

   你做得很好！ 现在转到下一部分。

## 将移动设备智能列表添加为列 {#add-mobile-smart-lists-as-columns}

1. 在刚刚创建的报告中，单击&#x200B;**[!UICONTROL Setup]**，然后将&#x200B;**[!UICONTROL Custom Columns]**&#x200B;拖到画布中。

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >默认情况下，人员绩效报表会查看过去7天。 您可以通过双击该时间范围来更改时间范围。

1. 查找并选择您之前创建的智能列表，然后单击&#x200B;**[!UICONTROL Apply]**。

   ![](assets/sixteen.png)

1. 单击&#x200B;**[!UICONTROL Report]**&#x200B;运行报告并查看您的数据。

   ![](assets/seventeen.png)

   很酷吧？ 做得好！

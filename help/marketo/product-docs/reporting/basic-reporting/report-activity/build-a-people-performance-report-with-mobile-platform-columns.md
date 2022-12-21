---
unique-page-id: 2951220
description: 使用移动平台列构建人员性能报表 — Marketo文档 — 产品文档
title: 使用Mobile Platform列构建人员性能报表
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 使用Mobile Platform列构建人员性能报表 {#build-a-people-performance-report-with-mobile-platform-columns}

请按照以下步骤操作，创建带有移动平台(iOS/Android)列的“人员性能报表”。

## 创建移动设备智能列表 {#create-mobile-smart-lists}

1. 转到 **营销活动**.

   ![](assets/ma.png)

1. 选择项目。

   ![](assets/two-1.png)

1. 在 **新建**，选择 **新建本地资产**.

   ![](assets/three-1.png)

1. 单击 **智能列表**.

   ![](assets/four-1.png)

1. 键入名称并单击 **创建**.

   ![](assets/five-1.png)

1. 查找“已打开的电子邮件”过滤器并将其拖到画布中。

   ![](assets/six-1.png)

1. 将电子邮件设置为 **any**.

   ![](assets/seven.png)

1. 单击 **添加约束** 选择 **平台**.

   ![](assets/eight.png)

   >[!TIP]
   >
   >在此示例中，我们使用了“已打开的电子邮件”过滤器。 您还可以使用“已单击的电子邮件”过滤器，因为该过滤器具有平台约束。

1. 将平台设置为 **iOS**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >必须至少有一个人在iOS设备上打开了您的电子邮件之一，Marketo才能自动提出查找建议。 如果未显示，您可以手动键入并保存。

   现在，为“Android”平台创建第二个智能列表。 完成后，转到下一部分。

## 创建人员绩效报表 {#create-a-people-performance-report}

1. 在营销活动下，选择容纳您的 **iOS** 和 **Android** 智能列表。

   ![](assets/ten.png)

1. 在 **新建**，选择 **新建本地资产**.

   ![](assets/eleven.png)

1. 单击 **报表**.

   ![](assets/twelve.png)

1. 将类型设置为 **人员绩效**.

   ![](assets/thirteen.png)

1. 单击&#x200B;**创建**。

   ![](assets/fourteen.png)

   你做得很好！ 现在转到下一节。

## 将移动设备智能列表添加为列 {#add-mobile-smart-lists-as-columns}

1. 在刚刚创建的报表中，单击 **设置**，然后拖动 **自定义列** 放到画布上。

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >默认情况下，“人员绩效”报表会查看过去7天的情况。 您可以通过双击来更改时间范围。

1. 查找并选择您之前创建的智能列表，然后单击 **应用**.

   ![](assets/sixteen.png)

1. 单击 **报表** 运行报表并查看数据。

   ![](assets/seventeen.png)

   很酷吧？ 干得好！

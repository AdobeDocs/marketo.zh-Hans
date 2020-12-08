---
unique-page-id: 2951220
description: 使用移动平台列构建人员性能报告- Marketo Docs —— 产品文档
title: 使用移动平台列构建人员性能报告
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---


# 使用移动平台列构建人员性能报告 {#build-a-people-performance-report-with-mobile-platform-columns}

按照以下步骤创建具有移动平台(iOS/Android)列的“人员性能报告”。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

## 创建移动智能列表 {#create-mobile-smart-lists}

1. 转到营 **销活动**。

   ![](assets/ma.png)

1. 选择项目。

   ![](assets/two-1.png)

1. 在“ **新建**”下， **选择“新建本地资产**”。

   ![](assets/three-1.png)

1. 单击 **智能列表**。

   ![](assets/four-1.png)

1. 键入名称，然后单击“ **创建**”。

   ![](assets/five-1.png)

1. 查找“已打开的电子邮件”过滤器并将其拖入画布。

   ![](assets/six-1.png)

1. 将“电子邮件”设 **置为“任意**”。

   ![](assets/seven.png)

1. 单击“添 **加约束** ”(Add Constraint **)并选**&#x200B;择“平台”(Platform)。

   ![](assets/eight.png)

   >[!TIP]
   >
   >我们在此示例中使用了“已打开的电子邮件”(Opened Email)过滤器。 您还可以使用“已点击电子邮件”过滤器，因为它具有平台约束。

1. 将平台设 **置为iOS**。

   ![](assets/nine.png)

   >[!NOTE]
   >
   >必须至少有一个人在iOS设备上打开了您的电子邮件之一，Marketo才能自动建议找到它。 如果未出现，可手动键入并保存。

   现在为“Android”平台创建第二个智能列表。 完成后，转到下一节。

## 创建人员绩效报告 {#create-a-people-performance-report}

1. 在“营销活动”下，选择包含iOS和Android **智能列表****的** 项目。

   ![](assets/ten.png)

1. 在“ **新建**”下， **选择“新建本地资产**”。

   ![](assets/eleven.png)

1. 单击 **报告**。

   ![](assets/twelve.png)

1. 将“类型”设置为“ **人员性能”**。

   ![](assets/thirteen.png)

1. 单击 **创建**。

   ![](assets/fourteen.png)

   你做得很好！ 现在转到下一节。

## 将移动智能列表添加为列 {#add-mobile-smart-lists-as-columns}

1. 在刚刚创建的报告中，单击“ **设置**”，然后 **将“自定义列** ”拖入画布。

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >默认情况下，“人员绩效”报表查看的是过去7天。 您可以通过多次单击来更改时间范围。

1. 查找并选择您之前创建的智能列表，然后单击“ **应用**”。

   ![](assets/sixteen.png)

1. 单击 **报告** ，运行报告并查看您的数据。

   ![](assets/seventeen.png)

   很酷吧？ 干得好！


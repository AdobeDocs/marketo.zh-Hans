---
unique-page-id: 2951220
description: 使用Mobile Platform列 — Marketo Docs — 产品文档构建人员绩效报告
title: 使用移动平台列构建人员绩效报告
translation-type: tm+mt
source-git-commit: 03ee7b69f691efce12825aa708c81dffa23cecd9
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# 使用移动平台列{#build-a-people-performance-report-with-mobile-platform-columns}构建人员绩效报告

按照以下步骤创建带有移动平台(iOS/Android)列的人员性能报告。

## 创建移动智能列表{#create-mobile-smart-lists}

1. 转至&#x200B;**营销活动**。

   ![](assets/ma.png)

1. 选择项目。

   ![](assets/two-1.png)

1. 在&#x200B;**New**&#x200B;下，选择&#x200B;**新建本地资产**。

   ![](assets/three-1.png)

1. 单击&#x200B;**智能列表**。

   ![](assets/four-1.png)

1. 键入名称，然后单击&#x200B;**创建**。

   ![](assets/five-1.png)

1. 查找已打开的电子邮件过滤器并将其拖动到画布中。

   ![](assets/six-1.png)

1. 将“电子邮件”设置为&#x200B;**是任何**。

   ![](assets/seven.png)

1. 单击&#x200B;**添加约束**&#x200B;并选择&#x200B;**平台**。

   ![](assets/eight.png)

   >[!TIP]
   >
   >我们在此示例中使用了“已打开的电子邮件”(Opened Email)过滤器。 您还可以使用“已点击电子邮件”过滤器，因为它具有“平台”约束。

1. 将平台设置为&#x200B;**iOS**。

   ![](assets/nine.png)

   >[!NOTE]
   >
   >至少必须有一个人在iOS设备上打开了您的电子邮件，Marketo的自动建议才能找到。 如果未出现，可手动键入并保存。

   现在为“Android”平台创建第二个智能列表。 完成后，转到下一部分。

## 创建人员绩效报告{#create-a-people-performance-report}

1. 在“营销活动”下，选择包含&#x200B;**iOS**&#x200B;和&#x200B;**Android**&#x200B;智能列表的项目。

   ![](assets/ten.png)

1. 在&#x200B;**New**&#x200B;下，选择&#x200B;**新建本地资产**。

   ![](assets/eleven.png)

1. 单击&#x200B;**报告**。

   ![](assets/twelve.png)

1. 将“类型”设置为&#x200B;**人员性能**。

   ![](assets/thirteen.png)

1. 单击&#x200B;**创建**。

   ![](assets/fourteen.png)

   你做得很好！ 现在，转到下一节。

## 将移动智能列表添加为列{#add-mobile-smart-lists-as-columns}

1. 在刚刚创建的报表中，单击&#x200B;**Setup**，然后将&#x200B;**Custom Columns**&#x200B;拖入画布中。

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >默认情况下，“人员绩效”报表查看的是过去7天。 您可以通过多次单击来更改时间范围。

1. 查找并选择之前创建的智能列表，然后单击&#x200B;**应用**。

   ![](assets/sixteen.png)

1. 单击&#x200B;**报表**&#x200B;运行报表并查看数据。

   ![](assets/seventeen.png)

   很酷吧？ 干得好！

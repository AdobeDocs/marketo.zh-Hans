---
unique-page-id: 10098812
description: 设置数字广告促销活动的收入归因 — Marketo文档 — 产品文档
title: 设置数字广告促销活动的收入归因
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# 设置数字广告促销活动的收入归因 {#set-up-revenue-attribution-for-digital-advertising-campaigns}

下面是如何设置数字广告渠道和营销活动的收入归因。 完成设置后，您可以像在其他Marketo程序中一样，对数字广告进行首次接触和多接触点收入归因。

在Marketo中设置第一个广告程序后，您可以克隆并更新其他渠道的该程序。 例如，将LinkedIn程序克隆到Facebook程序。

通过单独的程序，您可以跟踪每个程序的转化次数，并在Program Analyzer、Opportunity Influence Analyzer和其他Marketo Analytics功能中查看您的程序。

>[!PREREQUISITES]
>
>* 设置具有状态值和项目成功的渠道标记（例如，数字广告或社交付费和PPC）
>* 创建或编辑表单以传递查询字符串给人员
>* 确保您有权访问一些Revenue Cycle Analytics功能以报告广告渠道和营销活动

## 创建默认程序 {#create-a-default-program}

与某些程序（如电子邮件）可能定期运行特定时间段不同，默认程序始终处于打开状态。

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-5.png)

1. 单击 **新建** 并选择 **新建项目群**.

   ![](assets/image2016-3-14-15-52-0.png)

1. 如果您已设置程序，则可以 [克隆它](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >无论何时克隆程序，请务必替换智能列表的查询字符串字段中的名称。

1. 设置初始项目后，将新项目放入特定的campaign文件夹中。

   >[!NOTE]
   >
   >**示例**
   >
   >通过URL传递的查询字符串有助于Marketo了解某人在成为Marketo用户后点击了哪个广告营销活动。
   >
   >您可以创建一个查询字符串方法，其中包含要测量的所有变量。 Marketo使用这些变量将人员添加到您的其他程序。
   >
   >例如，您可以使用渠道type_Channel__Asset__Region。 类似于：SP_FB_NewGuide_US。 **注意**：缩写可节省空间。
   >
   >或者，将其设置为Channel_Adsource_AssetName_Region_UniqueIdNumber。 这可能类似于：Social-Paid_Facebook_NewGuide_NA_123。

## 为新名称创建智能营销活动 {#create-a-smart-campaign-for-new-names}

1. 在智能营销活动中，创建一个包含两个触发器和两个过滤器的智能列表，如下所示。

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >两个触发器和中使用的查询字符串 **捕获名称的程序** 过滤器对于您是唯一的。 此处显示的查询字符串仅为示例。 如果克隆了字段，则只需替换这些字段即可。

1. 创建流程步骤以将属性更改为 **客户获取计划** 并将新值设置为您为付费社交营销活动定义的值。

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. 计划和激活营销活动。

## 创建Smart Campaign以便状态/项目成功 {#create-a-smart-campaign-for-status-program-success}

您需要第二个智能营销活动来更改人员的状态，以便他们能够实现项目成功并包含在收入归因计算中。

1. 在 **填写表单** 触发器，在查询字符串中输入程序名称。 如果要克隆程序，只需将旧的查询字符串名称替换为新的查询字符串名称即可。

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. 创建流程步骤以将状态更改为与项目成功关联的状态。

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >上面的示例显示 **已转换**，但这取决于您的状态/成功值。

1. 计划和激活营销活动。

## 创建广告 {#create-your-ad}

设置项目和营销策划后，即可创建新广告。

1. 转到渠道；例如，LinkedIn或Facebook。
1. 创建新广告。
1. 选择Marketo登陆页面作为营销活动中行动号召的目标。
1. 将查询字符串添加到URL中。

   >[!NOTE]
   >
   >**示例**
   >
   >以下是将设置的所有信息添加到实际URL中的方法。 项目用与号(&amp;)分隔：
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **源** 是用作渠道标识符的人员来源
   >* **注释** 是为每个项目创建的唯一标识符
   >* **camp** 是Facebook、LinkedIn或Google中的营销活动
   >* **kk** 是要捕获的关键字或资源名称
   >
   >**这四个术语必须全部小写，并且URL中不能有任何空格才能捕获此信息。**

## 最佳实践 {#best-practices}

使用单个渠道标记来表示所有数字广告，或者，如果您希望与其他营销渠道进行更细微的比较（例如，社交 — 付费、搜索 — 付费、显示、重新定位），请使用多个渠道标记。

然后，为所需的每个报表视图设置不同的程序。 如果您有10个区域同时启动了“Big Campaign”，并且希望能够跨区域查看结果，请使用公共ID作为查询字符串中URL的参数（例如BC）。

如果要报告每个地区和大型营销活动的总体结果，请创建11个项目，每个地区一个项目，大型营销活动一个项目。 每个程序仅引用查询字符串中的相关字符（如BC）。

大型营销活动与地区项目之间存在人员计数方面的有意重叠，因此您不希望报告所有11个项目中的人员总数，因为有些人员同时参与了大型营销活动和地区项目。

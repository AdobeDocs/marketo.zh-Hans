---
unique-page-id: 10098812
description: 为数字广告促销活动设置收入归因 — Marketo文档 — 产品文档
title: 为数字广告促销活动设置收入归因
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# 为数字广告促销活动设置收入归因 {#set-up-revenue-attribution-for-digital-advertising-campaigns}

以下是如何为数字广告渠道和促销活动设置收入归因。 设置后，您可以对数字广告进行首次联系和多次联系收入归因，其方式与在其他Marketo项目中相同。

在Marketo中设置第一个广告程序后，您可以克隆并更新其他渠道的广告程序。 例如，将LinkedIn程序克隆到Facebook程序。

然后，通过单独的程序，您可以跟踪每个程序的转化次数，并在程序分析器、机会影响分析器和其他Marketo分析功能中查看您的程序。

>[!PREREQUISITES]
>
>* 设置具有状态值和计划成功率（例如，数字广告或Social付费和PPC）的渠道标记
>* 创建或编辑表单以将查询字符串与人员一起传递
>* 确保您有权访问一些收入周期分析功能来报告您的广告渠道和促销活动


## 创建默认程序 {#create-a-default-program}

与某些可能会在特定时间段内定期运行的程序（如电子邮件）不同，默认程序始终处于打开状态。

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-5.png)

1. 单击 **新建** 选择 **新计划**.

   ![](assets/image2016-3-14-15-52-0.png)

1. 如果您已经有项目，则可以 [克隆](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >每当克隆程序时，请务必替换智能列表的查询字符串字段中的名称。

1. 在设置初始项目后，将新项目放在特定的营销活动文件夹中。

   >[!NOTE]
   >
   >**示例**
   >
   >通过URL传递的查询字符串可帮助Marketo了解访客在成为Marketo人员时点击了哪个广告促销活动。
   >
   >您可以创建查询字符串方法，其中包含要测量的所有变量。 Marketo会使用这些变量将人员添加到您的不同程序。
   >
   >例如，您可以使用Channel type_Channel__Asset__Region。 这看起来可能是：SP_FB_NewGuide_US。 **注意**:缩写节省空间。
   >
   >或者，将其设置为Channel_Adsource_AssetName_Region_UniqueIdNumber。 这看起来可能是：Social-Paid_Facebook_NewGuide_NA_123。

## 为新名称创建智能营销活动 {#create-a-smart-campaign-for-new-names}

1. 在智能营销活动中，创建一个智能列表，其中包含两个触发器和两个过滤器，如所示。

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >两个触发器和 **捕获名称的程序** 过滤器是您特有的。 例如，此处显示的查询字符串仅为。 如果克隆了字段，则只需替换这些字段。

1. 创建流程步骤以将属性更改为 **客户获取计划** 并将新值设置为您为付费社交营销活动定义的值。

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. 计划并激活营销活动。

## 为状态/项目成功创建智能营销活动 {#create-a-smart-campaign-for-status-program-success}

您需要第二个智能营销活动来更改人员状态，以便他们能够取得项目成功并包含在收入归因计算中。

1. 在 **填写表单** 触发器，在查询字符串中输入程序名称。 如果要克隆程序，只需将旧的查询字符串名称替换为新名称即可。

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. 创建流程步骤，将状态更改为与项目成功关联的状态。

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >上例显示 **已转换**，但这取决于您的状态/成功值。

1. 计划并激活营销活动。

## 创建广告 {#create-your-ad}

设置项目和营销策划后，请创建新广告。

1. 转到频道；例如，LinkedIn或Facebook。
1. 创建新广告。
1. 选择Marketo登陆页面作为营销活动中行动动员的目标。
1. 将查询字符串添加到URL。

   >[!NOTE]
   >
   >**示例**
   >
   >下面介绍了如何将您设置的所有信息添加到实际URL中。 这些项目之间以与号(&amp;)分隔：
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **来源** 是用作渠道标识符的人员源
   >* **评论** 是为每个程序创建的唯一标识符
   >* **营地** 是Facebook、LinkedIn或Google中的促销活动
   >* **k** 是要捕获的关键词或资产名称

   >
   >**这四个术语必须全部为小写，并且URL中不能有任何空格，才能捕获此信息。**

## 最佳实践 {#best-practices}

使用单个渠道标记来表示所有数字广告，或者如果您希望与其他营销渠道（例如，社交付费、搜索付费、显示、重定位）进行更精细的比较，则使用多个渠道标记。

然后，针对您需要的每个报表视图设置不同的程序。 如果您有10个区域共同启动“大型营销活动”，并且希望能够跨区域查看结果，请在查询字符串的URL（例如BC）中将通用ID用作参数。

如果要报告大型营销活动的每个地区和总体结果，请创建11个项目 — 每个地区一个，大型营销活动一个。 每个程序仅引用查询字符串中的相关字符（如BC）。

“大型营销活动”与“地区”项目之间的人员计数存在有意重叠，因此您不希望报告所有11个项目的总人数，因为“大型营销活动”和“地区”项目中的某些人都参与过。

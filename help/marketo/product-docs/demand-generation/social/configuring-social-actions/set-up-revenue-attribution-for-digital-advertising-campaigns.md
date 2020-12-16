---
unique-page-id: 10098812
description: 为数字广告活动设置收入归因- Marketo Docs —— 产品文档
title: 为数字广告活动设置收入归因
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---


# 为数字广告活动设置收入归因 {#set-up-revenue-attribution-for-digital-advertising-campaigns}

下面介绍如何为数字广告渠道和活动设置收入归因。 设置后，您可以像其他营销项目一样对数字广告进行首次接触和多次接触收入归因。

在Marketo中设置第一个广告项目后，您可以克隆并更新它以用于其他渠道。 例如，将LinkedIn项目克隆到Facebook In。

通过单独的项目，您可以跟踪每个客户的转化次数，并在项目分析器、机会影响分析器和其他营销分析功能中查看项目。

>[!PREREQUISITES]
>
>* 设置具有状态值和项目成功率的渠道标签（例如，数字广告或社交付费和PPC）
>* 创建或编辑表单以将查询字符串传递给人员
>* 确保您有权使用某些收入周期分析功能来报告您的广告渠道和活动

>



## 创建默认项目 {#create-a-default-program}

与某些项目（如电子邮件）不同，默认项目始终处于打开状态，这些可能会在特定时间段内定期运行。

1. 转到营 **销活动**。

   ![](assets/login-marketing-activities-5.png)

1. 单击 **新建** ，然后选 **择新建项目**。

   ![](assets/image2016-3-14-15-52-0.png)

1. 如果您已有项目，可以克隆 [它](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md)。

   >[!TIP]
   >
   >无论何时克隆项目，请务必替换智能列表的查询字符串字段中的名称。

1. 在设置初始项目后，将新项目放在特定活动文件夹中。

   >[!NOTE]
   >
   >**示例**
   >
   >
   >通过URL传递的查询字符串有助于Market了解某人成为Marketo中的人时点击了哪个广告活动。
   >
   >
   >您可以创建包含要度量的所有变量的查询字符串方法。 Marketo使用这些变量将人添加到您的不同项目。
   >
   >
   >例如，您可以使用渠道类型渠道资产区域。 这可能是：SP_FB_NewGuide_US。 **注意**:缩写节省空间。
   >
   >
   >或者，将其设置为渠道_Adsource_AssetName_Region_UniqueIdNumber。 这可能是：Social-Paid_Facebook_NewGuide_NA_123。

## 为新名称创建智能活动 {#create-a-smart-campaign-for-new-names}

1. 在智能活动中，创建一个包含两个触发器和两个过滤器的智能列表，如图所示。

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >在两个触发器中使用的查询字符串和“捕获 **的名称的项目** ”过滤器是您特有的。 此处显示的查询字符串只是示例。 如果克隆了该字段，只需替换这些字段。

1. 创建流步骤，将属性更改为“ **客户赢取项目** ”，并将“新值”设置为您为付费社交活动定义的值。

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. 计划并激活活动。

## 为状态/活动成功创建智能项目 {#create-a-smart-campaign-for-status-program-success}

您需要第二个智能活动来更改人员状态，以便他们获得项目成功并纳入收入归因计算。

1. 在“填 **出表单** ”触发器中，在查询字符串中输入项目名称。 如果要仿制项目，只需将旧查询字符串名称替换为新名称。

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. 创建流程步骤，将状态更改为与项目成功关联的状态。

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >上例显示**Converted, **，但这取决于您的状态／成功值。

1. 计划并激活活动。

## 创建广告 {#create-your-ad}

设置项目和活动后，请创建新广告。

1. 去渠道;例如，LinkedIn或Facebook。
1. 创建新广告。
1. 在登陆页中选择“营销人员”活动作为“行动动员”的目标。
1. 将查询字符串添加到URL。

   >[!NOTE]
   >
   >**示例**
   >
   >
   >下面介绍如何将设置的所有信息添加到实际URL。 这些项目用和号(&amp;)分隔：
   >
   >
   >[www.marketo.com?**source**=Social-Paid&amp;**comment**=Social-Paid_Facebook_NewGuide_NA&amp;**camp**=abc&amp;**k=**xyz](http://www.marketo.com?source=Social-Paid&amp;comment=Social-Paid_Facebook_NewGUide_NA&amp;camp=abc&amp;kk+xyz)
   >
   >    
   >    
   >    * **source** 是用作渠道标识符的人员来源
   >    * **comment** 是为每个项目创建的唯一标识符
   >    * **camp是** Facebook、LinkedIn或Google中的活动
   >    * **kk** 是您要捕获的关键字或资产名称

   >    
   >    
   >**这四个术语必须全为小写，并且URL中不能有任何空格来捕获此信息。**

## 最佳实践 {#best-practices}

使用单个渠道标签来表示所有数字广告，或者，如果您希望与其他营销渠道（例如，社交付费、搜索付费、展示广告、重定位）进行更精细的比较，则使用多个渠道标签。

然后，为您需要的每个项目视图设置不同的报告。 如果您有10个区域一起启动“大查询”，并且希望能够跨区域视图结果，请将公用ID用作活动字符串中URL（例如BC）的参数。

如果您希望报告每个地区以及大活动的集体结果，请创建11个项目-每个地区一个，大活动一个。 每个项目只引用查询字符串中的相关字符（如BC）。

大活动和区域项目之间有意重叠的人数统计，因此您不希望报告所有11个项目的总人数，因为大活动和某个区域项目都有一些人。

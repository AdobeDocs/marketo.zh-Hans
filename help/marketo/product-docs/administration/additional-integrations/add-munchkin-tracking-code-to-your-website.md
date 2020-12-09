---
unique-page-id: 2360354
description: 将Munchkin跟踪代码添加到您的网站- Marketo Docs —— 产品文档
title: 将Munchkin跟踪代码添加到您的网站
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 0%

---


# 将Munchkin跟踪代码添加到您的网站 {#add-munchkin-tracking-code-to-your-website}

Marketo的自定义JavaScript跟踪代码称为Munchkin，它跟踪访问您网站的所有个人，以便您能够通过自动化营销活动对其访问做出响应。 即使是匿名访客也会跟踪其IP地址和其他信息。 **如果没有此跟踪代码，您将无法跟踪您网站上的访问或其他活动!**

>[!PREREQUISITES]
>
>请确保您有权访问经验丰富的JavaScript开发人员。 Marketo技术支持未设置为有助于对自定义JavaScript进行故障诊断。

## 将跟踪代码添加到您的网站 {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Adobe Experience Cloud的客户还可以使用Marketo在Adobe启动中的集成，在其网页上包含Munchkin脚本。 在此处获取应 [用程序](https://www.adobeexchange.com/experiencecloud.details.101054.html)。

1. 转到 **Admin** ，并 **单击左** 侧树中的Munchkin。

   ![](assets/image2015-8-25-16-3a21-3a14.png)

   为“跟踪代码类型”选择“异步”。

   ![](assets/image2015-8-25-16-3a24-3a33.png)

   >[!NOTE]
   >
   >几乎所有情况下，您都应使用异步代码。 [了解更多信息。](#types-of-munchkin-tracking-codes)

   单击并复制要放在您网站上的Javascript跟踪代码。

   ![](assets/image2015-8-25-16-3a26-3a12.png)

   >[!CAUTION]
   >
   >不要使用此屏幕截图中显示的代码——必须使用帐户中显示的唯一代码！

   >[!TIP]
   >
   >在要跟踪的网页上放置跟踪代码。 这可能是较小站点的每个页面，或仅是具有许多动态生成的网页、用户论坛等的站点上的关键页面。

   为获得最佳效果，请使用异步Munchkin代码并将其放 `<head>` 置到页面元素中。 如果您使用的是简单代码（不推荐），则此代码就在标记之 `</body>` 前。
   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!TIP]
>
>对于流量大（即每月数十万次访问）的站点，我们建议您选择不跟踪匿名人员。 [了解更多信息。](http://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/)

## 使用多个工作区时添加跟踪代码 {#add-tracking-code-when-using-multiple-workspaces}

如果您在Marketo帐户中使用工作区，您可能还有与工作区对应的单独Web演示。 在这种情况下，您可以使用Munchkin跟踪Javascript将匿名人员分配到正确的工作区和分区。

1. 转至“管理员”，然后单击左侧树中的“Munchkin”。

![](assets/image2015-8-25-16-3a28-3a41.png)

1. 为要跟踪的网页选择适当的工作区。

![](assets/image2015-8-25-16-3a30-3a32.png)

>[!NOTE]
>
>如果您不使用特殊工作区Munchkin代码，则人员将分配到设置帐户时创建的默认分区。 它最初被命名为“默认”，但您可能已在自己的Marketo帐户中更改了它。

1. 为“跟踪代码类型”选择“异步”。

   ![](assets/image2015-8-25-16-3a32-3a42.png)

1. 单击并复制要放在您网站上的JavaScript跟踪代码。

![](assets/image2015-8-25-16-3a34-3a7.png)

>[!CAUTION]
>
>不要使用此屏幕截图中显示的代码——必须使用帐户中显示的唯一代码！

1. 将跟踪代码放在元素中的网页 `<head>` 上。 将为访问此页面的新人员分配到此分区。

![](assets/image2015-8-25-16-3a5-3a20.png)

>[!CAUTION]
>
>对于页面上的单个分区和工作区，只能使用一个Munchkin跟踪脚本。 不要包括网站上多个分区／工作区的跟踪脚本。

>[!NOTE]
>
>在Market中创建的登陆页自动包含跟踪代码，因此您无需在这些代码上添加此代码。

## 蒙奇金跟踪代码的类型 {#types-of-munchkin-tracking-codes}

您可以选择3种类型的Munchkin跟踪代码。 每个因素对网页加载次数的影响都各不相同。

1. **简单**:代码行最少，但不针对网页加载时间进行优化。 每次加载网页时，此代码加载jQuery库。
1. **异步**:缩短网页加载时间。
1. **异步jQuery**:减少了网页加载时间，提高了系统性能。 此代码假定您已拥有jQuery，且不检查是否加载它。

## 测试Munchkin代码是否有效 {#test-if-your-munchkin-code-is-working}

在添加Munchkin代码后，检查该代码是否正常工作：

1. 访问网页。
1. 转到 **Analytics**。

   ![](assets/mainnav-analytics-hand.png)

1. 单击 **网页活动**。

   ![](assets/webanalytics.png)

1. 单击“ **设置** ”选项卡，按住多次 **单击“**&#x200B;活动源 **”，然后将其更改为“匿名访客”(**&#x200B;包括ISP)。

   ![](assets/analytics-activity-source.png)

   ![](assets/activitysource.png)

1. 单击“报 **告** ”选项卡。 如果看不到任何数据，请等待几分钟，然后单击底部的刷新图标。


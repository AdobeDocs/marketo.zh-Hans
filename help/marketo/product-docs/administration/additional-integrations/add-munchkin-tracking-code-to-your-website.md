---
unique-page-id: 2360354
description: 将Munchkin跟踪代码添加到您的网站 — Marketo Docs — 产品文档
title: 将Munchkin跟踪代码添加到您的网站
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 将Munchkin跟踪代码添加到您的网站{#add-munchkin-tracking-code-to-your-website}

Marketo的自定义JavaScript跟踪代码称为Munchkin，可跟踪访问您网站的所有个人，以便您能够通过自动化营销活动对其访问做出响应。 即使是匿名访客也会跟踪其IP地址和其他信息。 **如果没有此跟踪代码，您将无法跟踪您网站上的访问或其他活动**!

>[!PREREQUISITES]
>
>请确保您有权访问经验丰富的JavaScript开发人员。 Marketo技术支持未设置为有助于对自定义JavaScript进行疑难解答。

## 将跟踪代码添加到您的网站{#add-tracking-code-to-your-website}

>[!NOTE]
>
>Adobe Experience Cloud客户还可以使用Marketo在Adobe Launch中的集成，在其网页中包含Munchkin脚本。 在此处](https://www.adobeexchange.com/experiencecloud.details.101054.html)获取应用程序。[

1. 转至&#x200B;**Admin**&#x200B;并单击左侧树中的&#x200B;**Munchkin**。

   ![](assets/image2015-8-25-16-3a21-3a14.png)

   为“跟踪代码类型”选择“异步”。

   ![](assets/image2015-8-25-16-3a24-3a33.png)

   >[!NOTE]
   >
   >在几乎所有情况下，您都应使用异步代码。 [了解更多信息。](#types-of-munchkin-tracking-codes)

   单击并复制要放入您网站的Javascript跟踪代码。

   ![](assets/image2015-8-25-16-3a26-3a12.png)

   >[!CAUTION]
   >
   >不要使用此屏幕截图中显示的代码 — 您必须使用帐户中显示的唯一代码！

   >[!TIP]
   >
   >在要跟踪的网页上放置跟踪代码。 这可能是较小网站的每个页面，或仅是具有许多动态生成网页、用户论坛等的网站上的关键页面。

   为获得最佳效果，请使用异步Munchkin代码并将它放在页面的`<head>`元素中。 如果您使用的是简单代码（不推荐），则它就在`</body>`标记之前。
   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!TIP]
>
>对于流量较大（即每月数十万次访问）的网站，我们建议您选择不跟踪匿名人员。 [了解更多](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/)。

## 使用多个工作区{#add-tracking-code-when-using-multiple-workspaces}时添加跟踪代码

如果您在Marketo帐户中使用工作区，则可能还具有与工作区对应的单独Web演示。 在这种情况下，您可以使用Munchkin跟踪Javascript，将匿名人员分配到正确的工作区和分区。

1. 转至&#x200B;**Admin**&#x200B;并单击左侧树中的&#x200B;**Munchkin**。

![](assets/image2015-8-25-16-3a28-3a41.png)

1. 为要跟踪的网页选择适当的工作区。

   ![](assets/image2015-8-25-16-3a30-3a32.png)

>[!NOTE]
>
>如果您不使用特殊工作区Munchkin代码，则人员将分配到在设置帐户时创建的默认分区。 它最初名为“Default”，但您可能已在自己的Marketo帐户中更改了它。

1. 选择&#x200B;**异步**&#x200B;作为跟踪代码类型。

   ![](assets/image2015-8-25-16-3a32-3a42.png)

1. 单击并复制要放在您网站上的JavaScript跟踪代码。

   ![](assets/image2015-8-25-16-3a34-3a7.png)

   >[!CAUTION]
   >
   >不要使用此屏幕截图中显示的代码 — 您必须使用帐户中显示的唯一代码！

1. 将跟踪代码放在网页的`<head>`元素中。 将为此分区分配访问此页面的新人员。

   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!CAUTION]
>
>只能对页面上的单个分区和工作区使用一个Munchkin跟踪脚本。 不要包括网站上多个分区/工作区的跟踪脚本。

>[!NOTE]
>
>在Marketo中创建的登陆页会自动包含跟踪代码，因此您无需在这些代码上放置此代码。

## Munchkin跟踪代码的类型{#types-of-munchkin-tracking-codes}

您可以选择三种类型的Munchkin跟踪代码。 每种方式对网页加载次数的影响都不同。

1. **简单**:代码行最少，但不优化网页加载时间。每次加载网页时，此代码加载jQuery库。
1. **异步**:缩短网页加载时间。
1. **异步jQuery**:减少了网页加载时间，提高了系统性能。此代码假定您已拥有jQuery，且不检查是否加载它。

## 测试Munchkin代码是否正在工作{#test-if-your-munchkin-code-is-working}

要在添加Munchkin代码后检查其是否正常工作，请执行以下操作：

1. 访问网页。

1. 转至&#x200B;**Analytics**。

   ![](assets/mainnav-analytics-hand.png)

1. 单击&#x200B;**网页活动**。

   ![](assets/webanalytics.png)

1. 单击&#x200B;**设置**&#x200B;选项卡，按住多次键并单击&#x200B;**活动源**，将其更改为&#x200B;**匿名访客（包括ISP）**。

   ![](assets/analytics-activity-source.png)

   ![](assets/activitysource.png)

1. 单击&#x200B;**报告**&#x200B;选项卡。 如果看不到任何数据，请稍等几分钟，然后单击底部的刷新图标。

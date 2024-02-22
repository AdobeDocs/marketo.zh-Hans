---
unique-page-id: 2360354
description: '"添加 [!DNL Munchkin] 将代码跟踪到您的网站 — Marketo文档 — 产品文档”'
title: '"添加 [!DNL Munchkin] 将代码跟踪到您的网站”'
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
feature: Administration, Munchkin Tracking Code
source-git-commit: bb9593ab500d57127f22b14757688d7521661e38
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# 添加 [!DNL Munchkin] 将代码跟踪到您的网站 {#add-munchkin-tracking-code-to-your-website}

Marketo的自定义JavaScript跟踪代码，称为 [!DNL Munchkin]，可跟踪访问您网站的所有个人，以便您能够通过自动营销活动对其访问做出反应。 甚至匿名访客也会与其IP地址和其他信息一起被跟踪。 **如果没有此跟踪代码，您将无法跟踪网站上的访问或其他活动**！

>[!PREREQUISITES]
>
>请确保您有权访问经验丰富的JavaScript开发人员。 Marketo技术支持未设置为帮助排除自定义JavaScript故障。

## 将跟踪代码添加到您的网站 {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Adobe Experience Cloud用户还可以使用 [Adobe Launch中的Marketo集成](https://exchange.adobe.com/apps/ec/100223/adobe-launch-core-extension){target="_blank"} 要包含 [!DNL Munchkin] 脚本。 如果您使用Adobe启动项， _该 [!DNL Munchkin] 脚本自动添加_，因此您无需自行添加。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. 单击 **[!UICONTROL 蒙奇金]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. 选择 **[!UICONTROL 异步]** 对象 **[!UICONTROL 跟踪代码类型]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-3.png)

   >[!NOTE]
   >
   >在大多数情况下，您应使用异步代码。 [了解详情](#types-of-munchkin-tracking-codes).

1. 单击并复制Javascript跟踪代码以放置到您的网站上。

   ![](assets/add-munchkin-tracking-code-to-your-website-4.png)

   >[!CAUTION]
   >
   >请勿使用此屏幕快照中显示的代码 — 您必须使用帐户中显示的唯一代码！

   >[!TIP]
   >
   >将跟踪代码置于要跟踪的网页上。 这可能是较小站点的每个页面，或者只有具有许多动态生成的网页、用户论坛等的站点上的关键页面。

   为获得最佳结果，请使用异步 [!DNL Munchkin] 代码并将其置于 `<head>` 元素。 如果您使用的是简单代码（不推荐），则此代码位于 `</body>` 标记之前。

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >对于访问量大的网站（即每月访问数十万次），我们建议您选择不跟踪匿名人员。 [了解详情](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/){target="_blank"}.

## 使用多个工作区时添加跟踪代码 {#add-tracking-code-when-using-multiple-workspaces}

如果您在Marketo帐户中使用工作区，则可能还会有与您的工作区对应的单独Web存在。 在这种情况下，您可以使用 [!DNL Munchkin] 跟踪Javascript以将您的匿名用户分配到正确的工作区和分区。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. 单击 **[!UICONTROL 蒙奇金]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. 为要跟踪的网页选择适当的工作区。

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >如果您不使用特殊工作区 [!DNL Munchkin] 代码中，人员将分配到在设置帐户时创建的默认分区。 它名为“[!UICONTROL 默认]”一开始，但您可能在自己的Marketo帐户中更改了此设置。

1. 选择 **[!UICONTROL 异步]** 对象 **[!UICONTROL 跟踪代码类型]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. 单击并复制JavaScript跟踪代码以放置到您的网站上。

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >请勿使用此屏幕快照中显示的代码 — 您必须使用帐户中显示的唯一代码！

1. 将跟踪代码放置在网页上的 `<head>` 元素。 访问此页面的新用户将分配给此分区。

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >您只能使用一个 [!DNL Munchkin] 页面上单个分区和工作区的跟踪脚本。 不要在网站上包含多个分区/工作区的跟踪脚本。

   >[!NOTE]
   >
   >在Marketo中创建的登陆页面会自动包含跟踪代码，因此您无需在其上放置此代码。

## 类型 [!DNL Munchkin] 跟踪代码 {#types-of-munchkin-tracking-codes}

有三种类型 [!DNL Munchkin] 可选择的跟踪代码。 每种方法都会以不同的方式影响网页加载时间。

1. **[!UICONTROL 简单]**：代码行最少，但不会优化网页加载时间。 每次加载网页时，此代码都会加载jQuery库。
1. **[!UICONTROL 异步]**：缩短网页加载时间。
1. **[!UICONTROL 异步jQuery]**：减少网页加载时间，并提高系统性能。 此代码假定您已经拥有jQuery，并且不检查以加载它。

## 测试您的 [!DNL Munchkin] 代码正在工作 {#test-if-your-munchkin-code-is-working}

检查您的 [!DNL Munchkin] 添加代码后，该代码仍然可用：

1. 访问网页。

1. 在您的 [!DNL My Marketo]，单击 **[!UICONTROL 分析]** 磁贴。

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. 单击 **[!UICONTROL 网页活动]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. 单击 **[!UICONTROL 设置]** 选项卡，双击 **[!UICONTROL 活动源]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. 更改 [!UICONTROL 活动源] 到 **[!UICONTROL 匿名访客（包括ISP）]** 并单击 **[!UICONTROL 应用]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. 单击 **[!UICONTROL 报表]** 选项卡。

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >如果您没有看到任何数据，请等待几分钟，然后单击底部的刷新图标。

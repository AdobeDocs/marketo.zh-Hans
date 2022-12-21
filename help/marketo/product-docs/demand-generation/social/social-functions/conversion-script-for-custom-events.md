---
unique-page-id: 2950561
description: 自定义事件的转化脚本 — Marketo文档 — 产品文档
title: 自定义事件的转换脚本
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# 自定义事件的转换脚本 {#conversion-script-for-custom-events}

在创建引荐选件时，您可以定义实现目标。 如果针对目标执行的操作是您自己的网页上的特定事件，则可以使用转化脚本调用我们的JavaScript API。

## 检索转换脚本 {#retrieve-the-conversion-script}

1. 在引荐选件编辑器中，单击 **选件详细信息** 然后选择 **客户JavaScript事件** 从“实现目标”下拉列表中。

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. 复制灰色框中的顶部脚本，并将其放在 `<body>` 标记。 底部脚本位于 `<header>` 标记。

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >如果这两个脚本都在非Marketo网站上，请记住复制并粘贴它们。

## 检索加载器脚本 {#retrieve-the-loader-script}

1. 从树中选择引荐选件，然后单击 **反向链接选件操作** 和 **嵌入代码**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. 右键单击 **标题代码** 并将其插入您的网页标题中。 那么，为 **正文代码**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## 将脚本粘贴到您的网页上 {#pasting-the-scripts-onto-your-webpage}

将转换脚本粘贴到主体和标题的HTML中。 接下来，将加载器脚本放入主体和标头的HTML中。

![](assets/image2015-4-20-21-3a0-3a16.png)

## 连接转换脚本 {#connecting-the-conversion-script}

在这里，您将编写一个JavaScript函数，该函数使用您要在其中触发目标完成的任何页面元素的特定HTMLID。 例如：

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

在此示例中，网页上有一个ID为“#myButtonId”的按钮。 单击该按钮后，会将人员注册为已完成目标。

太棒了！ 您的网站现在正在通过Marketo捕获自定义社交促销目标。

>[!MORELIKETHIS]
>
>* [指定引荐选件的目标](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [创建反向链接选件](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [在您的网站上部署Social](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)


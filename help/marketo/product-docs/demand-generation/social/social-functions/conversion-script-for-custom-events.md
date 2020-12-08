---
unique-page-id: 2950561
description: 自定义事件的转换脚本- Marketo Docs —— 产品文档
title: 自定义事件的转换脚本
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# 自定义事件的转换脚本 {#conversion-script-for-custom-events}

在创建推荐优惠时，您可以定义实施目标。 如果目标操作是您自己网页上的特定事件，则可以使用转换脚本调用我们的JavaScript API。

## 检索转换脚本 {#retrieve-the-conversion-script}

1. 在引用优惠编辑器中，单 **击优惠详** 细信息，然后从 **实现目标下拉框中** 选择客户JavaScript事件。

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. 复制灰色框中的顶部脚本，并将其放在标记内的网页 `<body>` 上。 底部脚本放在标记 `<header>` 中。

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >如果两个脚本正在非Marketo网站上，请记住复制和粘贴它们。

## 检索加载器脚本 {#retrieve-the-loader-script}

1. 从树中选择引用优惠，然后单击 **引用优惠操作****和嵌入代码**。

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. 右键单击标 **题代码** ，将其插入网页标题。 然后，对正文代码执 **行相同操作**。

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## 将脚本粘贴到您的网页上 {#pasting-the-scripts-onto-your-webpage}

将转换脚本粘贴到正文和标题的HTML中。 接下来，将加载器脚本放入HTML中作为正文和标题。

![](assets/image2015-4-20-21-3a0-3a16.png)

## 连接转换脚本 {#connecting-the-conversion-script}

这里您将编写一个JavaScript函数，该函数使用任何要触发目标完成的页面元素的特定HTML ID。 例如：

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

在此示例中，网页上有一个ID为“#myButtonId”的按钮。 单击该按钮后，该人将被注册为已完成目标。

太棒了！ 您的网站现在正在使用Marketo获取自定义社交促销目标。

>[!NOTE]
>
>**相关文章**
>
>* [指定引用优惠的目标](../../../../product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [创建推荐优惠](../../../../product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [在您的网站上部署Social](deploy-social-on-your-website.md)


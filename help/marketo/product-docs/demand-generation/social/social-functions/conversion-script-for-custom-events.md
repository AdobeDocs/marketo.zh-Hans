---
unique-page-id: 2950561
description: 自定义事件的转化脚本 — Marketo文档 — 产品文档
title: 自定义事件的转换脚本
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 1%

---

# 自定义事件的转换脚本 {#conversion-script-for-custom-events}

您可以在创建反向链接优惠时定义实现目标。 如果计入目标的操作是您自己网页上的特定事件，则可以使用转化脚本来调用我们的JavaScript API。

>[!IMPORTANT]
>
>2024年7月31日，我们开始了弃用此功能的过程。 无法再创建新资产。 现有资产将继续使用到2025年1月31日。 [了解详情](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## 检索转换脚本 {#retrieve-the-conversion-script}

1. 在反向链接优惠编辑器中，单击&#x200B;**优惠详细信息**，然后从实现目标下拉列表中选择&#x200B;**客户JavaScript事件**。

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. 复制灰色框中的顶部脚本，并将其放在网页的`<body>`标记内。 底部脚本放在`<header>`标记中。

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >如果这两个脚本在非Marketo网站上运行，请记得复制并粘贴它们。

## 检索Loader脚本 {#retrieve-the-loader-script}

1. 从树中选择引用选件，然后单击&#x200B;**引用选件操作**&#x200B;和&#x200B;**嵌入代码**。

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. 右键单击&#x200B;**页眉代码**&#x200B;并将其插入到网页页眉。 然后对&#x200B;**正文代码**&#x200B;执行相同操作。

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## 将脚本粘贴到网页上 {#pasting-the-scripts-onto-your-webpage}

将转换脚本粘贴到正文和标题的HTML中。 接下来，将加载器脚本放入正文和标题的HTML中。

![](assets/image2015-4-20-21-3a0-3a16.png)

## 连接转换脚本 {#connecting-the-conversion-script}

在这里，您将编写一个JavaScript函数，该函数使用您要触发目标完成的任何页面元素的特定HTMLID。 例如：

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

在此示例中，网页上有一个id为“#myButtonId”的按钮。 单击该按钮后，将会将该人员注册为已完成目标。

太棒了！ 您的网站现在通过Marketo捕获自定义社交促销目标。

>[!MORELIKETHIS]
>
>* [指定推荐选件的目标](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [创建推荐选件](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [在您的网站上部署Social](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)

---
unique-page-id: 6094879
description: 向Web营销活动添加Target URL - Marketo文档 — 产品文档
title: 向Web营销活动添加目标URL
exl-id: 5fbb3f12-1474-46c3-8315-8d081422e154
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# 向Web营销活动添加目标URL {#adding-a-target-url-to-a-web-campaign}

Target URL位于Set Campaign页面下方，用于定义将显示Web营销活动的特定URL。

## 为对话框或构件Web营销活动添加Target URL {#adding-a-target-url-for-dialog-or-widget-web-campaigns}

1. 转到 **Web营销活动**.

   ![](assets/web-campaigns-hand-5.jpg)

1. 选择 **新建Web营销活动**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. 添加 **营销活动名称**. 选择 **目标区段**. 添加 **目标URL**.

   ![](assets/set-web-campaign-hands.jpg)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">名称</th> 
   <th colspan="1" rowspan="1">描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>任意页面</strong></td> 
   <td colspan="1" rowspan="1"><p>允许营销活动显示在任何页面上。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>匹配时包含URL参数</strong></p></td> 
   <td colspan="1" rowspan="1">添加URL参数以在包含此参数的URL上匹配和显示促销活动。 例如 campaign=cpc</td> 
  </tr> 
 </tbody> 
</table>

## 向目标URL添加多个URL {#adding-multiple-urls-to-target-url}

单击加号图标(![—](assets/image2015-2-18-8-3a40-3a59.png))将打开多值条目对话框以添加多个URL。 每行添加一个URL。

![](assets/image2015-2-23-18-3a15-3a57.png)

>[!NOTE]
>
>* 对话框和小部件Web营销活动可以使用任何页面和通配符(&#42;)选项。
>* 在高级用例中，在区域中，Web营销活动可以在URL路径末尾使用通配符。 示例： [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)
>* URL区分大小写

## 为区域Web营销活动添加目标URL {#adding-a-target-url-for-in-zone-web-campaigns}

1. 转到 **Web** **营销活动**.

   ![](assets/web-campaigns-hand-5.jpg)

1. 选择 **新建Web营销活动**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. 添加 **营销活动名称**. 选择 **目标区段**. 添加 **目标URL**.

   >[!NOTE]
   >
   >具有位于区域中的目标URL必须定义一个或多个URL。 在高级用例中，在区域中，Web营销活动可以在URL路径末尾使用通配符。 示例： [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)

   ![](assets/set-web-campaign-multiple-hands.jpg)

>[!MORELIKETHIS]
>
>* [创建对话营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [在区域营销活动中创建RTP](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [创建RTP构件营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)

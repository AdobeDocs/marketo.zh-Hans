---
unique-page-id: 6094879
description: 向Web促销活动添加Target URL - Marketo文档 — 产品文档
title: 向Web营销活动添加目标URL
exl-id: 5fbb3f12-1474-46c3-8315-8d081422e154
source-git-commit: 6ad418c8f4056b9a2fb31b0ac995692f0c618795
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# 向Web营销活动添加目标URL {#adding-a-target-url-to-a-web-campaign}

Target URL位于“设置促销活动”页面下，可定义Web促销活动将显示的特定URL或URL。

## 为对话框或小组件Web促销活动添加目标URL {#adding-a-target-url-for-dialog-or-widget-web-campaigns}

1. 转到 **Web营销活动**.

   ![](assets/web-campaigns-hand-5.jpg)

1. 选择 **创建新Web营销活动**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. 添加 **营销活动名称**. 选择 **目标区段**. 添加 **Target URL**.

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
   <td colspan="1" rowspan="1"><p>允许营销活动在任何页面上显示。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>匹配时包含URL参数</strong></p></td> 
   <td colspan="1" rowspan="1">添加URL参数以在包含此参数的URL上匹配和显示营销活动。 例如 campaign=cpc</td> 
  </tr> 
 </tbody> 
</table>

## 向Target URL添加多个URL {#adding-multiple-urls-to-target-url}

单击加号图标(![—](assets/image2015-2-18-8-3a40-3a59.png))将打开多值条目对话框以添加多个URL。 每行添加一个URL。

![](assets/image2015-2-23-18-3a15-3a57.png)

>[!NOTE]
>
>* 对话框和小组件Web营销活动可使用任意页面和通配符(&#42;)选项。
>* 在高级用例中，In Zone Web促销活动可在URL路径末尾使用通配符。 示例： [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)
>* URL区分大小写


## 为区域Web促销活动中的目标URL添加 {#adding-a-target-url-for-in-zone-web-campaigns}

1. 转到 **Web** **促销活动**.

   ![](assets/web-campaigns-hand-5.jpg)

1. 选择 **创建新Web营销活动**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. 添加 **营销活动名称**. 选择 **目标区段**. 添加 **Target URL**.

   >[!NOTE]
   >
   >具有区域内的目标URL必须定义特定的URL或URL。 在高级用例中，In Zone Web促销活动可在URL路径末尾使用通配符。 示例： [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)

   ![](assets/set-web-campaign-multiple-hands.jpg)

>[!MORELIKETHIS]
>
>* [创建对话营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [在区域营销活动中创建RTP](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [创建RTP小组件促销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)


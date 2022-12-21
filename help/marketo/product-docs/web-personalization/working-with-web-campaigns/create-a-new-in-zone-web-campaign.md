---
unique-page-id: 4719400
description: 在Zone Web Campaign - Marketo文档 — 产品文档中新建
title: 在区域Web营销活动中新建
exl-id: 5cbe80a2-5e20-4e35-a722-b4cb479b4df7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# 在区域Web营销活动中新建 {#create-a-new-in-zone-web-campaign}

Web促销活动是与特定区段关联的自定义反应，可以是 [对话框](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) 在您的网站上，区域替换 [小组件功能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md) 或电子邮件警报。 “区域内”Web营销活动将基于区域ID的网站元素替换为内容或图形横幅。

## 在区域内创建Web营销活动 {#create-an-in-zone-web-campaign}

1. 转到 **Web营销活动**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. 选择 **创建新Web营销活动。**

   ![](assets/create-new-web-campaign-hand.png)

1. 选择 **区域内** 营销活动类型。 自定义和添加 **区域ID。** 将营销活动设置为 **置顶** 并在编辑器中添加您的创作元素。 添加要预览的页面的URL并单击 **预览** 以了解营销活动在您的网站上将作何反应。

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**什么是区域ID?**
   >
   >区域ID是您希望在现场找到“区域内”Web营销活动的位置。 要查找“区域ID”，只需转到您的网站，选择要替换为Web营销活动的区域并右键单击即可。 在Chrome中，选项为“Inspect元素”，而在其他浏览器中，选项可能会有所不同。
   >
   >然后，您需要查找与网站的此部分关联的“id”，该ID会突出显示，因为您正在检查该元素。 例如，如果在Chrome中右键单击后，突出显示的文本显示 `<div id="featured-slider">` 那么，“featured-slider”即是您应在“zone id”部分中键入的内容。 通常使用“div id”，但也可以使用任何ID，如h1 id、p id等。

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">名称</th> 
   <th colspan="1" rowspan="1">描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong> 区域ID </strong></td> 
   <td colspan="1" rowspan="1"><p>输入在营销活动替换的网站元素的HTML代码中找到的ID的名称。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> 置顶 </strong></p></td> 
   <td colspan="1" rowspan="1">默认情况下，“在区域”营销活动会选中“置顶”复选框，并在网站上访客会话期间将“在区域”营销活动保留在“区域ID”位置。 建议始终将“In Zone（区域）”设置为“置顶”。</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> 淡出</strong> </p></td> 
   <td colspan="1" rowspan="1">选中使用效果复选框和淡入色对网站上的区域id区域提供淡入色的效果。 如果“入区”是图形横幅，则首先加载页面，然后激活营销活动，并产生渐隐效果。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>滑动</strong></td> 
   <td colspan="1">选中使用效果复选框和滑动选项会对网站上的区域ID区域产生滑动效果。 如果In Zone是图形横幅，则首先加载页面，然后激活营销活动，并具有从左到右的滑动效果。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> 富文本编辑器  </strong></td> 
   <td colspan="1">富文本编辑器允许文本格式、链接和图像插入。 <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">有关更多信息，请参阅此处</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> 在网站上预览   </strong></td> 
   <td colspan="1">在启动促销活动之前进行预览。 <br> 
    <ul> 
     <li> URL — 输入运行营销活动的示例URL，以查看营销活动外观的预览示例。</li> 
     <li>设备 — 预览按设备显示营销活动的方式：台式机、移动设备纵向、移动设备横向、平板电脑纵向、纵向横向。</li> 
     <li> 预览 — 单击 <strong>预览</strong> 打开示例URL的新窗口，以了解营销活动如何反应。</li> 
     <li> 共享 — 使用“共享”按钮向同事发送一封包含链接的电子邮件，以查看代理营销活动。</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>通过使用 [内置模板](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) 或 [保存现有营销活动](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) 作为模板以供重复使用。

>[!NOTE]
>
>**想要A/B测试您的Web营销活动？** 一个或多个Web营销活动可以是 [测试A/B以获得最佳结果](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md). 利用自动调节功能，平台可自动识别效果更好的营销活动，继续进行转化率最高的营销活动并暂停其他营销活动。

## 编辑Web营销活动 {#edit-a-web-campaign}

从 **Web营销活动** 页面，单击 **编辑** 在营销活动上。

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>为了更便于查找所需的营销活动，请使用 [过滤功能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md).

## 预览Web营销活动 {#preview-a-web-campaign}

1. 在“Web营销活动”页面中，单击 **预览** 在要查看的web营销活动上。

   ![](assets/in-zone-web-campaign-preview.png)

## 克隆Web营销活动 {#clone-a-web-campaign}

请参阅 [克隆Web营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## 删除Web营销活动 {#delete-a-web-campaign}

1. 在“Web营销活动”页面中，单击 **删除** 在要删除的营销活动上。

   ![](assets/in-zone-web-campaign-delete.png)

1. 此时会显示确认消息，确认您是否要删除营销活动。

>[!MORELIKETHIS]
>
>* [创建新的小组件Web营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [创建新对话框Web营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)


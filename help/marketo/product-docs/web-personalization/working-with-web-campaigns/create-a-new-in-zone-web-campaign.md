---
unique-page-id: 4719400
description: 在区域中新建Web促销活动 — Marketo文档 — 产品文档
title: 新建区域内的Web营销活动
exl-id: 5cbe80a2-5e20-4e35-a722-b4cb479b4df7
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# 新建区域内的Web营销活动 {#create-a-new-in-zone-web-campaign}

Web营销活动是与特定区段关联的自定义反应，可以是 [对话框](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) 在您的网站上，使用区域替换、 [构件功能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md) 或电子邮件提醒。 区域Web促销活动会根据区域ID将网站的某个元素替换为内容或图形横幅。

## 创建区域内的Web营销活动 {#create-an-in-zone-web-campaign}

1. 转到 **Web营销活动**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. 选择 **创建新的Web营销活动。**

   ![](assets/create-new-web-campaign-hand.png)

1. 选择 **所在区域** 营销活动类型。 自定义和添加 **区域ID。** 将营销活动设置为 **粘性** 并在编辑器中添加您的创意。 添加要预览的页面的URL并单击 **预览** 以了解营销活动在您的网站上的反应。

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**什么是区域ID？**
   >
   >区域ID是您希望“所在区域”Web营销活动位于现场的位置。 要查找“区域ID”，只需转到您的网站，选择要替换为Web促销活动的区域，然后右键单击即可。 在Chrome中，选项为“Inspect元素”，而在其他浏览器中，该选项可能有所不同。
   >
   >然后，您需要查找与网站的此部分关联的“id”，由于您正在检查该元素，该“id”会突出显示。 例如，在Chrome中右键单击后，高亮显示的文本会显示 `<div id="featured-slider">` 此时，“feature-slider”是您应在“zone id”部分中键入的内容。 通常使用“div id”，但也可以使用任何ID，例如h1 id、p id等。

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
   <td colspan="1" rowspan="1"><p><strong> 粘性 </strong></p></td> 
   <td colspan="1" rowspan="1">默认情况下，“置顶”复选框对于“所在区域”营销活动处于选中状态，并且会在访客在网站上的整个会话期间将所在区域的营销活动保持在其区域ID位置。 建议始终将“区域”设置为“粘性”。</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> 渐隐</strong> </p></td> 
   <td colspan="1" rowspan="1">选中“使用效果”复选框和“淡化”会对网站上的“区域ID”区域产生淡出效果。 如果进入区域是图形横幅，则首先加载页面，然后营销活动激活，并逐渐消退。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>滑动</strong></td> 
   <td colspan="1">选中“使用效果”复选框和“滑动”选项后，网站上的“区域ID”区域将滑动。 如果进入区域是图形横幅，则首先加载页面，然后营销活动从左到右激活，并产生滑动效果。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> 富文本编辑器  </strong></td> 
   <td colspan="1">富文本编辑器允许设置文本格式、链接和插入图像。 <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">有关更多信息，请参阅此处</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> 在站点上预览   </strong></td> 
   <td colspan="1">在启动营销活动之前进行预览。 <br> 
    <ul> 
     <li> URL — 输入营销活动将运行的示例URL，以查看营销活动实时外观的预览示例。</li> 
     <li>设备 — 按设备预览营销活动的显示方式：桌面、移动设备纵向、移动设备横向、平板电脑纵向、纵向横向。</li> 
     <li> 预览 — 单击 <strong>预览</strong> 打开示例URL的新窗口以查看营销活动的反应方式。</li> 
     <li> 共享 — 使用“共享”按钮向同事发送电子邮件，其中包含查看代理营销活动的链接。</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>通过使用我们的 [内置模板](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) 或 [保存现有营销活动](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) 作为模板供重用。

>[!NOTE]
>
>**是否希望对Web营销活动进行A/B测试？** 一个或多个Web营销活动可以是 [A/B测试以获得最佳结果](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md). 借助自动调整功能，平台会自动识别效果较好的营销活动，继续提供转化率最高的营销活动，并暂停其他营销活动。

## 编辑Web活动 {#edit-a-web-campaign}

从 **Web营销活动** 页面，单击 **编辑** 在营销策划中。

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>为了更便于找到所需的营销策划，请使用 [筛选功能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md).

## 预览Web营销活动 {#preview-a-web-campaign}

1. 在Web营销策划页面中，单击 **预览** 在要查看的Web营销活动上。

   ![](assets/in-zone-web-campaign-preview.png)

## 克隆Web营销活动 {#clone-a-web-campaign}

参见 [克隆Web营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## 删除Web活动 {#delete-a-web-campaign}

1. 在Web营销策划页面中，单击 **删除** 要删除的Campaign上。

   ![](assets/in-zone-web-campaign-delete.png)

1. 此时会显示确认消息，确认是否要删除营销策划。

>[!MORELIKETHIS]
>
>* [创建新的构件Web营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [新建Dialog Web营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)

---
unique-page-id: 4719400
description: 在Zone Web活动- Marketo Docs — 产品文档中新建
title: 在Zone Web活动中新建
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---


# 在区域Web活动{#create-a-new-in-zone-web-campaign}中新建

Web活动是与特定区段关联的自定义反应，可以是您网站上的[对话框](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)、区域替换、[构件功能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)或电子邮件警报。 “区域内”Web活动将基于区域ID的网站元素替换为内容或图形横幅。

## 创建In Zone Web活动{#create-an-in-zone-web-campaign}

1. 转到&#x200B;**Web活动**。

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. 选择&#x200B;**“新建Web活动”。**

   ![](assets/create-new-web-campaign-hand.png)

1. 选择&#x200B;**In Zone**&#x200B;活动类型。 自定义和添加&#x200B;**区域ID。** 将活动设置为 **** Sticky，并在编辑器中添加您的创意。将页面的URL添加到预览，然后单击&#x200B;**预览**&#x200B;以查看活动对您网站的反应。

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**什么是区域ID?**
   >
   >区域ID是您希望“区域内”Web活动在现场的位置。 要查找“区域ID”，只需转到您的网站，选择要替换为Web活动的区域并右键单击。 在Chrome中，选项是“Inspect元素”，在其他浏览器中可能有所不同。
   >
   >然后，您要查找与网站的此部分关联的“id”，因为您正在检查该元素，此部分会高亮显示。 例如，如果您在Chrome中右键单击后，高亮显示的文本显示`<div id="featured-slider">`，则“featured-slider”是您应在“zone id”部分中键入的内容。 通常使用“div id”，但也可以使用任何ID，如h1 id、p id等。

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">名称</th> 
   <th colspan="1" rowspan="1">说明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong> 区域ID </strong></td> 
   <td colspan="1" rowspan="1"><p>输入在活动替换的网站元素的HTML代码中找到的ID的名称。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> 粘滞 </strong></p></td> 
   <td colspan="1" rowspan="1">默认情况下，对于“在区域中”活动，“粘滞”复选框处于选中状态，并在网站上的访客会话中将“在区域中”活动保持在其“区域ID”位置。 建议始终将“内区”设置为“粘滞”。</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> 渐隐</strong> </p></td> 
   <td colspan="1" rowspan="1">选中“使用效果”复选框和“淡化”可对网站上的“区域”ID区域提供淡入淡出的效果。 如果“入区”是图形横幅，则首先加载页面，然后活动激活时会产生淡入效果。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>滑动</strong></td> 
   <td colspan="1">选中“使用效果”复选框和“滑动”选项可提供对网站上“区域标识”区域的滑动效果。 如果“入区”是图形横幅，则首先加载页面，然后激活活动，并从左到右显示滑动效果。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> 富文本编辑器  </strong></td> 
   <td colspan="1">富文本编辑器允许文本格式化、链接和图像插入。 <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">在此处阅读更多内容</a> 。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> 预览现场   </strong></td> 
   <td colspan="1">预览活动。<br> 
    <ul> 
     <li> URL — 输入活动将运行的示例URL，以查看活动如何显示的预览示例。</li> 
     <li>设备 — 预览活动按设备的显示方式：桌面、移动纵向、移动横向、平板电脑纵向、纵向横向。</li> 
     <li> 预览 — 单击<strong>预览</strong>打开示例URL的新窗口，查看活动的反应。</li> 
     <li> 共享 — 使用“共享”按钮向同事发送一封包含链接的电子邮件，以查看代理活动。</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>使用我们的[内置模板](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md)或[将现有活动](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md)保存为模板以供重用，从而加快和简化活动创建过程。

>[!NOTE]
>
>**想要A/B测试Web活动?** 可以对一个或多个Web活动进 [行A/B测试以获得最佳结果](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md)。借助“自动调整”功能，平台可自动识别性能更好的活动，继续执行转换率最高的活动并暂停其他。

## 编辑Web活动{#edit-a-web-campaign}

从&#x200B;**Web活动**&#x200B;页面，单击活动上的&#x200B;**编辑**。

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>要更轻松地找到所需的活动，请使用[过滤器功能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md)。

## 预览Web活动{#preview-a-web-campaign}

1. 在“Web活动”页中，单击要视图的Web活动上的&#x200B;**预览**。

   ![](assets/in-zone-web-campaign-preview.png)

## 克隆Web活动{#clone-a-web-campaign}

请参阅[克隆Web活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md)。

## 删除Web活动{#delete-a-web-campaign}

1. 在“Web活动”页中，单击要删除的活动上的&#x200B;**删除**。

   ![](assets/in-zone-web-campaign-delete.png)

1. 此时将显示确认消息，确认是否要删除活动。

>[!MORELIKETHIS]
>
>* [创建新的Widget Web活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [创建新对话框Web活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)


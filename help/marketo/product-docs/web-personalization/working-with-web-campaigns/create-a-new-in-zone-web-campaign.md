---
unique-page-id: 4719400
description: 在区域中创建新的Web促销活动 — Marketo文档 — 产品文档
title: 在区域中创建新的Web营销活动
exl-id: 5cbe80a2-5e20-4e35-a722-b4cb479b4df7
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 在区域中创建新的Web营销活动 {#create-a-new-in-zone-web-campaign}

Web营销活动是与特定区段关联的自定义反应，可以是您网站上的[对话框](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)、区域内替换、[构件功能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)或电子邮件警报。 区域Web促销活动将基于区域ID的网站元素替换为内容或图形横幅。

## 创建区域Web营销活动 {#create-an-in-zone-web-campaign}

1. 转到&#x200B;**[!UICONTROL Web Campaigns]**。

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. 选择&#x200B;**[!UICONTROL Create New Web Campaign].**

   ![](assets/create-new-web-campaign-hand.png)

1. 选择&#x200B;**[!UICONTROL In Zone]**&#x200B;营销活动类型。 自定义并添加&#x200B;**[!UICONTROL Zone id]。**&#x200B;将营销活动设置为&#x200B;**[!UICONTROL Sticky]**&#x200B;并在编辑器中添加您的创意内容。 添加要预览的页面URL，然后单击&#x200B;**[!UICONTROL Preview]**&#x200B;以查看营销活动在您的网站上将如何反应。

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**什么是区域ID？**
   >
   >区域ID是您希望“[!UICONTROL In Zone]”Web营销活动位于现场的位置。 要查找“[!UICONTROL Zone ID]”，只需转到您的网站，选择要替换为Web营销活动的区域，然后右键单击即可。 在Chrome中，选项为“检查元素”，而在其他浏览器中，该选项可能有所不同。
   >
   >然后，您要查找与网站此部分关联的“id”，由于您正在检查该元素，该“id”会突出显示。 例如，在Chrome中右键单击后，突出显示的文本显示`<div id="featured-slider">`，则“featured-slider”是您应在“区域ID”部分中键入的内容。 通常使用“div id”，但也可以使用任何ID，例如h1 id、p id等。

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
   <td colspan="1" rowspan="1"><p>输入在营销活动所替换的网站元素的HTML代码中找到的ID的名称。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> 粘性 </strong></p></td> 
   <td colspan="1" rowspan="1">默认情况下，“置顶”复选框对于“所在区域”营销活动处于选中状态，并且会在访客在网站上的整个会话期间将所在区域的营销活动保留在其区域ID位置。 建议始终将输入区域设置为“粘性”。</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>正在淡出</strong> </p></td> 
   <td colspan="1" rowspan="1">选中“使用效果”复选框和“淡化”会对网站上的“区域ID”区域产生淡出效果。 如果进入区域是图形横幅，则首先加载页面，然后营销活动会激活，并呈渐隐效果。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>滑动</strong></td> 
   <td colspan="1">选中“使用效果”复选框和“滑动”选项，可提供一个对网站上的“区域ID”区域有效的滑动。 如果In Zone是图形横幅，则首先加载页面，然后营销活动从左到右激活，并产生滑动效果。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> 富文本编辑器  </strong></td> 
   <td colspan="1">富文本编辑器允许设置文本格式、链接和插入图像。 <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">在此阅读更多</a> 。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> 在站点上预览   </strong></td> 
   <td colspan="1">在启动营销活动之前进行预览。<br> 
    <ul> 
     <li> URL — 输入营销活动将运行的示例URL，以查看营销活动实时效果的预览示例。</li> 
     <li>设备 — 按设备预览营销活动的显示方式：桌面、移动设备纵向、移动设备横向、平板电脑纵向、纵向横向。</li> 
     <li> 预览 — 单击<strong>预览</strong>可打开示例URL的新窗口，以查看营销活动的反应方式。</li> 
     <li> 共享 — 使用“共享”按钮向同事发送电子邮件，其中包含查看代理营销活动的链接。</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>通过使用我们的[内置模板](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md)或[将现有营销活动](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md)另存为模板以供重复使用，加快并简化营销活动创建过程。

>[!NOTE]
>
>**要对Web营销活动进行A/B测试吗？**&#x200B;一个或多个网站营销活动可以[A/B测试以获得最佳结果](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md)。 借助自动调整功能，平台会自动识别表现较好的营销活动，继续提供转化率最高的营销活动，并暂停其他营销活动。

## 编辑Web活动 {#edit-a-web-campaign}

从&#x200B;**Web营销活动**&#x200B;页面，单击营销活动上的&#x200B;**编辑**。

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>若要更轻松地找到所需的营销活动，请使用[筛选器功能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md)。

## 预览Web活动 {#preview-a-web-campaign}

1. 从[!UICONTROL Web Campaigns]页面，单击要查看的Web营销活动上的&#x200B;**[!UICONTROL Preview]**。

   ![](assets/in-zone-web-campaign-preview.png)

## 克隆Web营销活动 {#clone-a-web-campaign}

请参阅[克隆Web营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md)。

## 删除Web活动 {#delete-a-web-campaign}

1. 在Web营销活动页面中，单击要删除的营销活动上的&#x200B;**[!UICONTROL Delete]**。

   ![](assets/in-zone-web-campaign-delete.png)

1. 此时会显示确认消息，确认您是否要删除营销策划。

>[!MORELIKETHIS]
>
>* [创建新的构件Web营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [新建Dialog Web营销活动](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)

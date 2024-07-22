---
unique-page-id: 4720917
description: facebook中的个性化再营销 — Marketo文档 — 产品文档
title: facebook中的个性化再营销
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 1%

---

# facebook中的个性化再营销 {#personalized-remarketing-in-facebook}

通过个性化再营销，您可以使用RTP数据和Facebook再营销的强大功能，重新吸引用户。

>[!PREREQUISITES]
>
>* 使用Web Personalization数据完成[重定位](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)设置
>* 查看有关自定义受众](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)和再营销的[](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [Facebook文档。

## 在Facebook中创建受众 {#creating-an-audience-in-facebook}

1. 在Facebook中，转到广告管理器中的[受众选项卡](https://www.facebook.com/ads/audience_manager)。

1. 单击&#x200B;**工具**&#x200B;并选择&#x200B;**受众**。

   ![](assets/one-1.png)

1. 单击&#x200B;**创建自定义受众**。

   ![](assets/two-1.png)

1. 选择&#x200B;**网站流量**。

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. 在网站流量列表中，选择&#x200B;**自定义组合**。

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. 在包含列表中，选择&#x200B;**事件**。

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. 在“事件”列表中，选择&#x200B;**RTP再营销**&#x200B;并选择参数。

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. 对于此示例，请选择“行业”以包含&#x200B;**教育**。 输入&#x200B;**教育**，并在最近&#x200B;**内将**&#x200B;编辑为180天。 输入受众名称： **教育行业**。 单击&#x200B;**创建受众**。

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. 现在，您已使用Facebook中的RTP数据创建新的自定义受众。

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## facebook中的RTP数据点 {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>事件名称</th> 
   <th> </th> 
  </tr> 
  <tr> 
   <td>RTP再营销</td> 
   <td> 
    <div> 
     <table> 
      <tbody> 
       <tr> 
        <th>参数</th> 
        <th>值</th> 
       </tr> 
       <tr> 
        <td>ABM列表</td> 
        <td>（基于帐户的列表的名称）</td> 
       </tr> 
       <tr> 
        <td colspan="1">类别</td> 
        <td colspan="1"><p>财富500强</p><p>财富1000强</p><p>Global 2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">组</td> 
        <td colspan="1"><p>企业</p><p>SMB</p></td> 
       </tr> 
       <tr> 
        <td>行业</td> 
        <td><p>防御</p><p>教育</p><p>金融服务</p><p>政府</p><p>医疗保健、医药、生物技术</p><p>软件和Internet</p><p>等等…… （根据RTP Industry选项）</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">分段受众</td> 
        <td colspan="1">（在RTP中创建的分段受众的名称）</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## 使用广告定位受众 {#target-your-audience-with-an-ad}

有关其他详细信息，请参阅[Facebook的文档](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience)。

1. 转到广告管理器，单击&#x200B;**创建广告**。

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. 选择&#x200B;**将联系人发送到您的网站**&#x200B;作为您的营销活动的目标。

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. 输入您的网站URL。

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. 创建您的广告集。 从您创建的受众列表中选择自定义受众，例如“教育行业”。

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. 选择所有其他广告集选项，设置预算并定义广告创意。

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. 现在，您已在Facebook中设置了一个个性化的再营销活动。

>[!MORELIKETHIS]
>
>* [使用Web Personalization数据重新定位](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* 在Google中[个性化再营销](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)

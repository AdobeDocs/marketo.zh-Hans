---
unique-page-id: 4720917
description: facebook中的个性化再营销 — Marketo文档 — 产品文档
title: facebook中的个性化再营销
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---

# facebook中的个性化再营销 {#personalized-remarketing-in-facebook}

个性化再营销让您能够使用RTP数据和Facebook再营销的强大功能，重新吸引用户。

>[!PREREQUISITES]
>
>* 完成 [使用Web个性化数据重定位](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) 设置
>* 查看 [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [Facebook自定义受众文档](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) 和再营销。


## 在Facebook中创建受众 {#creating-an-audience-in-facebook}

1. 在Facebook，转到 [“受众”选项卡](https://www.facebook.com/ads/audience_manager) 在广告管理器中。

1. 单击 **工具** 选择 **受众**.

   ![](assets/one-1.png)

1. 单击 **创建自定义受众**.

   ![](assets/two-1.png)

1. 选择 **网站流量**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. 在网站流量列表中，选择 **自定义组合**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. 在“Include（包含）”列表中，选择 **事件**.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. 在事件列表中，选择 **RTP再营销** 并选择一个参数。

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. 在本例中，选择要包含的行业 **教育**. 输入 **教育**，编辑 **最后** 180天。 输入受众名称： **教育产业**. 单击 **创建受众**.

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. 您现在已在Facebook中使用RTP数据创建了新的自定义受众。

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## facebook的RTP数据点 {#rtp-data-points-in-facebook}

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
        <td>（基于帐户的列表名称）</td> 
       </tr> 
       <tr> 
        <td colspan="1">类别</td> 
        <td colspan="1"><p>财富500强</p><p>财富1000强</p><p>2000年全球</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">组</td> 
        <td colspan="1"><p>企业</p><p>中小型企业</p></td> 
       </tr> 
       <tr> 
        <td>行业</td> 
        <td><p>防御</p><p>教育</p><p>金融服务</p><p>政府</p><p>医疗保健、制药、生物技术</p><p>软件和Internet</p><p>等……（根据RTP行业选项）</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">分段受众</td> 
        <td colspan="1">（RTP中创建的分段受众的名称）</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## 使用广告定位受众 {#target-your-audience-with-an-ad}

有关更多详细信息，请参阅 [Facebook文档](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. 转到广告管理器，单击 **创建广告**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. 选择 **将人员发送到您的网站** 作为营销活动的目标。

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. 输入您的网站URL。

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. 创建广告集。 从您创建的受众列表中选择自定义受众，例如教育行业。

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. 选择所有其他广告集选项，设置预算并定义广告创作元素。

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. 您现在都可以在Facebook中设置个性化的再营销活动。

>[!MORELIKETHIS]
>
>* [使用Web个性化数据重定位](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Google中的个性化再营销](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)


---
unique-page-id: 4720796
description: 使用Web个性化数据重新定位 — Marketo Docs — 产品文档
title: 使用Web个性化数据重新定位
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---


# 使用Web个性化数据{#retargeting-with-web-personalization-data}重新定位

>[!AVAILABILITY]
>
>网站重定位现在属于Web个性化拼贴。 如果您仅购买了“重定位”，您将看到此拼贴并访问Web个性化产品，并且仅&#x200B;****&#x200B;启用了“重定位”功能。 这样，您便可以访问帐户设置、重新定位页面、区段和其他跟踪页面。

过去访问过您网站的目标潜在客户，会根据他们的身份和行为进行展示广告再营销。 通过基于行业、指定帐户和已知人数据的相关广告，个性化地重新定位目标特定受众。

Web个性化当前会将数据附加到以下再营销平台：

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

Web个性化会将以下数据发送到再营销平台，以创建受众并运行再营销广告活动:

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Web个性化数据</th> 
  </tr> 
  <tr> 
   <th><p>行业</p></th> 
  </tr> 
  <tr> 
   <th><p>组（企业、SMB）</p></th> 
  </tr> 
  <tr> 
   <th><p>类别（《财富》500/1000, 2000年全球）</p></th> 
  </tr> 
  <tr> 
   <th><p>ABM列表(指定帐户列表)</p></th> 
  </tr> 
  <tr> 
   <th><p>分段受众（基于区段）</p></th> 
  </tr> 
  <tr> 
   <th><p>已点击Web活动</p></th> 
  </tr> 
 </tbody> 
</table>

## 再营销配置{#remarketing-configuration}

1. 转到&#x200B;**重定位**。

   ![](assets/one.png)

   >[!NOTE]
   >
   >重定位配置是按域或子域。 如果要将数据从这些域发送到重定向平台，请激活其他域。

1. 为每个域的Google Analytics或Google Universal Analytics激活设置。

   >[!NOTE]
   >
   >您需要在您的网站上实施Google重定位标记。
   >
   >如果您已经设置了与Web个性化和Google Analytics的集成，则无需编辑此部件，因为它与“帐户设置”下的配置相同。

   ![](assets/two.png)

1. 激活Facebook的配置。 单击并展开Facebook折叠面板，单击&#x200B;**On**&#x200B;以将相应的事件和数据发送到FacebookAudience Manager。 单击&#x200B;**保存**。

   >[!NOTE]
   >
   >您需要安装[Facebook自定义受众像素](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)您的网站，才能使用此功能。

   ![](assets/three.png)

## 创建分段受众{#creating-segmented-audience}

分段受众允许您选择现有区段作为受众，以用于重新定位活动。 例如，选择“已知人员”区段。

>[!TIP]
>
>无需为已通过域配置发送的行业或其他数据创建分段受众。 最好根据已知人数数据对细分使用细分受众。

1. 单击&#x200B;**创建分段受众**。

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. 输入受众名称，选择渠道，然后从现有区段的列表中选择区段。

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. 单击&#x200B;**保存**。

   您现在已完成Web个性化中的重新定位设置，登录到您的重新定位平台，并基于此数据创建受众，并设置您的重新定位广告活动。

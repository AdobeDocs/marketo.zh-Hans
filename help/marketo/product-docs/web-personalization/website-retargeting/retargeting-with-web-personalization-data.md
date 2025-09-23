---
unique-page-id: 4720796
description: 使用Web Personalization数据重新定位 — Marketo文档 — 产品文档
title: 使用 Web 个性化数据进行重定向
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 3%

---

# 使用[!DNL Web Personalization]数据重新定位 {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>网站重定位现在归入Web Personalization拼贴下。 如果您只购买了重定位，您将看到此磁贴并访问[!DNL Web Personalization]产品，其中启用了&#x200B;**仅**&#x200B;重定位功能。 这让您能够访问帐户设置、重定位页面、区段和其他跟踪页面。

再营销活动根据访问者的身份和行为来定位以前访问过您的网站的潜在客户，并投放基于他们的展示广告。 个性化重定位通过基于行业、指定帐户和已知人员数据的相关广告定位特定受众。

Web Personalization当前会将数据附加到以下再营销平台：

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

[!DNL Web Personalization]将以下数据发送到再营销平台以创建受众并运行再营销广告活动：

<table>
 <tbody>
  <tr>
   <th colspan="1">[!DNL Web Personalization] 数据</th>
  </tr>
  <tr>
   <th><p>行业</p></th>
  </tr>
  <tr>
   <th><p>组（企业、SMB）</p></th>
  </tr>
  <tr>
   <th><p>类别(Fortune 500/1000， Global 2000)</p></th>
  </tr>
  <tr>
   <th><p>ABM列表（指定帐户列表）</p></th>
  </tr>
  <tr>
   <th><p>分段受众（基于区段）</p></th>
  </tr>
  <tr>
   <th><p>已单击Web营销活动</p></th>
  </tr>
 </tbody>
</table>

## 再营销配置 {#remarketing-configuration}

1. 转到&#x200B;**[!UICONTROL Retargeting]**。

   ![](assets/one.png)

   >[!NOTE]
   >
   >重定位配置是按域或子域进行的。 如果要将数据从其他域发送到重定位平台，请激活这些域。

1. 激活Google Analytics的设置或每个域的[!DNL Google Universal Analytics]。

   >[!NOTE]
   >
   >您需要在网站上实施Google重定位标记。
   >
   >如果您已设置与Web Personalization和Google Analytics的集成，则无需编辑此部件，因为它与“帐户设置”下的配置相同。

   ![](assets/two.png)

1. 激活Facebook的配置。 单击并展开[!DNL Facebook]折叠面板，单击&#x200B;**[!UICONTROL On]**&#x200B;以将相应的事件和数据发送到Facebook Audience Manager。 单击 **[!UICONTROL Save]**。

   >[!NOTE]
   >
   >您需要安装[[!DNL Facebook] Custom Audience Pixel](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)网站才能使用此功能。

   ![](assets/three.png)

## 创建分段受众 {#creating-segmented-audience}

使用分段受众，您可以选择现有区段作为受众，用于重新定位营销活动。 例如，选择您的已知人员区段。

>[!TIP]
>
>无需为已在域配置中通过发送的行业数据或其他数据创建分段受众。 最好对基于已知人员数据的区段使用分段受众。

1. 单击 **[!UICONTROL Create Segmented Audience]**。

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. 输入受众名称，选择渠道，然后从现有区段列表中选择区段。

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. 单击 **[!UICONTROL Save]**。

   您现在已在[!DNL Web Personalization]中完成重定位设置，登录到重定位平台并根据此数据创建受众，然后设置重定位广告营销活动。

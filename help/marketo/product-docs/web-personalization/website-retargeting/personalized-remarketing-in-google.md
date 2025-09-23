---
unique-page-id: 4720810
description: Google中的个性化再营销 — Marketo文档 — 产品文档
title: 在 Google 中进行个性化二次营销
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 6%

---

# 在 Google 中进行个性化二次营销 {#personalized-remarketing-in-google}

通过个性化再营销，您可以使用RTP数据和Google Analytics的强大功能重新吸引用户，从而触及Google显示网络。

>[!PREREQUISITES]
>
>* 使用[数据 [!DNL Web Personalization] 配置完成](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)重定位
>* 查看[Google Analytics帮助的再营销](https://support.google.com/analytics/topic/2611283?hl=en&ref_topic=3413645)文档。

## 在Google中创建再营销受众 {#creating-a-remarketing-audience-in-google}

1. 登录到您的Google Analytics。 单击&#x200B;**[!UICONTROL Admin]**、**[!UICONTROL Account]**、**[!UICONTROL Property]**。 单击&#x200B;**[!UICONTROL Audience Definitions]**&#x200B;和&#x200B;**[!UICONTROL Audiences]**。

   ![](assets/remarketing-ga-screenshots.jpg)

1. 单击 **[!UICONTROL +New Audience]**。

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **[!UICONTROL Link Configuration]**：链接到您的[!DNL Google Adwords]帐户。 **[!UICONTROL Define Audience]**：单击&#x200B;**[!UICONTROL Create New]**。

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. 在受众生成器中，单击&#x200B;**[!UICONTROL Sequences]**、**[!UICONTROL Find the RTP Data]**、[!UICONTROL Custom Dimensions]下的[!UICONTROL UICONTROL [ !] Custom Variables]和[!UICONTROL Events]。

>[!TIP]
>
>如何在Analytics中查找RTP数据以构建受众？
>
>在Google Analytics中：
>
>* 自定义变量：组织、行业
>* 事件类别：区段、Insightera-CTA、RTP — 再营销
>* 事件标签：区段名称、促销活动名称、分段受众名称
>
>在Google Universal Analytics中：
>
>* 自定义维度：组织、行业、类别(Fortune 500,1000， Global 2000)、组(Enterprise， SMB)、ABM列表（指定帐户列表）
>* 事件类别：RTP-Segment、RTP-Campaign RTP-Remarketing
>* 事件标签：区段名称、促销活动名称、分段受众名称

**来自RTP分段受众数据的再营销受众示例**

1. 单击&#x200B;**[!UICONTROL Sequences].**
1. 选择&#x200B;**[!UICONTROL Event Label].**
1. 输入&#x200B;**[!UICONTROL Name of Segmented Audience]** （在RTP中显示）。
1. 单击 **[!UICONTROL Apply]**。

![](assets/image2015-2-10-14-3a51-3a43.png)

**来自RTP行业数据的受众示例**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. 单击 **[!UICONTROL Sequences]**。
1. 选择 **[!UICONTROL RTP-Industry]**。
1. 输入&#x200B;**行业名称** （例如[!UICONTROL Financial Services]，[!UICONTROL Education]...）。
1. 单击 **[!UICONTROL Apply]**。
1. 输入&#x200B;**[!UICONTROL Audience Name]**。 单击 **[!UICONTROL Save]**。

![](assets/image2015-1-15-18-3a29-3a16.png)

## 在[!DNL Google Adwords]中创建再营销广告营销活动 {#create-a-remarketing-ad-campaign-in-google-adwords}

1. 登录到&#x200B;**[!DNL Google Adwords]**。 单击&#x200B;**[!UICONTROL Campaigns]**，选择&#x200B;**[!UICONTROL Display Network only]**。

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. 输入&#x200B;**[!UICONTROL Campaign Name]**，选择&#x200B;**[!UICONTROL Type Remarketing].**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. 输入&#x200B;**[!UICONTROL Ad Group Name]，**&#x200B;输入&#x200B;**[!UICONTROL Enhanced CPC]**，选择&#x200B;**[!UICONTROL Remarketing List]**。

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. 单击&#x200B;**[!UICONTROL Save]**&#x200B;并继续。
1. 添加图像或文本广告，然后开始再营销活动。

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* 使用[数据 [!DNL Web Personalization] 重新定位](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [在 [!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)中进行个性化再营销

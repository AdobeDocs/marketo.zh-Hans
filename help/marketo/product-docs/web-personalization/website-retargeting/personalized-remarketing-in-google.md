---
unique-page-id: 4720810
description: Google中的个性化再营销 — Marketo文档 — 产品文档
title: Google中的个性化再营销
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Google中的个性化再营销 {#personalized-remarketing-in-google}

通过个性化再营销，您可以使用RTP数据和Google Analytics的强大功能重新吸引用户，从而触及Google显示网络。

>[!PREREQUISITES]
>
>* 使用Web Personalization数据完成[重定位](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)配置
>* 查看[使用Google Analytics帮助](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645)进行再营销文档。

## 在Google中创建再营销受众 {#creating-a-remarketing-audience-in-google}

1. 登录到您的Google Analytics。 单击&#x200B;**管理员**、**帐户**、**属性**。 单击&#x200B;**受众定义**&#x200B;和&#x200B;**受众**。

   ![](assets/remarketing-ga-screenshots.jpg)

1. 单击&#x200B;**+新受众**。

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **链接配置**：链接到您的Google Adwords帐户。 **定义受众**：单击&#x200B;**新建**。

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. 在受众生成器中，单击“自定义Dimension”、“自定义变量”、“事件”下的&#x200B;**序列**&#x200B;和&#x200B;**查找RTP数据**。

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
>* 自定义Dimension：组织、行业、类别(Fortune 500,1000， Global 2000)、组(Enterprise， SMB)、ABM列表（指定帐户列表）
>* 事件类别：RTP-Segment、RTP-Campaign RTP-Remarketing
>* 事件标签：区段名称、促销活动名称、分段受众名称

**来自RTP分段受众数据的再营销受众示例**

1. 单击&#x200B;**序列。**
1. 选择&#x200B;**事件标签。**
1. 输入&#x200B;**分段受众的名称**（在RTP中显示）。
1. 单击&#x200B;**应用**。

![](assets/image2015-2-10-14-3a51-3a43.png)

**来自RTP行业数据的受众示例**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. 单击&#x200B;**序列**。
1. 选择&#x200B;**RTP — 行业**。
1. 输入&#x200B;**行业名称**(例如 金融服务、教育……)。
1. 单击&#x200B;**应用**。
1. 输入&#x200B;**受众名称**。 单击&#x200B;**保存**。

![](assets/image2015-1-15-18-3a29-3a16.png)

## 在Google Adwords中创建再营销广告营销活动 {#create-a-remarketing-ad-campaign-in-google-adwords}

1. 登录到&#x200B;**Google Adwords**。 单击&#x200B;**营销活动**，选择&#x200B;**仅显示网络**。

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. 输入&#x200B;**促销活动名称**，选择&#x200B;**键入再营销。**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. 输入&#x200B;**广告组名称，**&#x200B;输入&#x200B;**增强型CPC**，选择&#x200B;**再营销列表**。

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. 单击保存并继续。
1. 添加图像或文本广告，然后开始再营销活动。

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [使用Web Personalization数据重新定位](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* 在Facebook中[个性化再营销](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

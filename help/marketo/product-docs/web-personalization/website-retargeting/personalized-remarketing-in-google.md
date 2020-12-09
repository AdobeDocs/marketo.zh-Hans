---
unique-page-id: 4720810
description: Google中的个性化再营销- Marketo Docs —— 产品文档
title: Google中的个性化再营销
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---


# Google中的个性化再营销 {#personalized-remarketing-in-google}

个性化的再营销使您能够借助RTP数据和Google Analytics的强大功能与用户重新互动，触及Google Display Network的触及范围。

>[!PREREQUISITES]
>
>* 使用Web个 [性化数据配置完成重定位](retargeting-with-web-personalization-data.md) 。
>* 查看 [再营销Google Analytics帮助](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645) 文档

>



## 在Google中创建再营销受众 {#creating-a-remarketing-audience-in-google}

1. 登录Google Analytics。 单击 **管理**、 **帐户**、 **属性**。 单击 **受众定义** 和 **受众**。

   ![](assets/remarketing-ga-screenshots.jpg)

1. 单击 **+新建受众**。

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **链接配置**:链接到您的Google Adwords帐户
1. **定义受众**:单击 **新建**。

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. 在受众生成器中，单击 **序列** , **然后在自定义Dimension、** 自定义变量和事件下查找RTP数据。

>[!TIP]
>
>如何在Analytics中查找RTP受众?
>
>Google Analytics:
>
>* 自定义变量：组织、行业
>* 事件类别:细分， Insightera-CTA,RTP再营销
>* 事件标签：区段名称、活动名称、受众名称

>
>
在Google Universal Analytics中：
>
>* 自定义Dimension:组织、行业、类别（财富500,1000强，全球2000强）、集团（企业、SMB）、ABM列表(指定客户列表)
>* 事件类别:RTP段、RTP活动RTP再营销
>* 事件标签：区段名称、活动名称、受众名称

>



**基于RTP分段受众数据的再营销受众示例**

1. 单击“ **序列”。**
1. 选择 **事件标签。**
1. 输 **入分段受众的名称** （如RTP中所示）。
1. 单击“ **应用**”。

![](assets/image2015-2-10-14-3a51-3a43.png)

**RTP行业受众示例**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. 单击“ **序列**”。
1. 选择** RTP行业**。
1. 输入 **行业名称** (例如， 金融服务、教育……)。
1. 单击“ **应用**”。
1. 输入 **受众名**。 单击 **保存**。

![](assets/image2015-1-15-18-3a29-3a16.png)

## 在Google Adwords中创建再营销广告活动 {#create-a-remarketing-ad-campaign-in-google-adwords}

1. 登录 **Google Adwords**。 单击 **活动**，选择“ **仅显示网络”**。

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. 输入 **活动**，选择 **类型再营销。**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. 输入 **广告组名称，** 输入 **增强的CPC**，选择 **再营销列表**。

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. 单击“保存”并继续。
1. 添加图像或文本广告，开始再营销活动。

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!NOTE]
>
>**相关文章**
>
>* [使用Web个性化数据重新定位](retargeting-with-web-personalization-data.md)
>* [Facebook中的个性化再营销](personalized-remarketing-in-facebook.md)


---
unique-page-id: 4720810
description: Google中的个性化再营销 — Marketo文档 — 产品文档
title: Google中的个性化再营销
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Google中的个性化再营销 {#personalized-remarketing-in-google}

通过个性化再营销，您可以使用RTP数据和Google Analytics的强大功能通过Google Display Network重新吸引用户。

>[!PREREQUISITES]
>
>* 完成 [使用Web个性化数据重新定位](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) 配置
>* 审核 [使用Google Analytics帮助进行再营销](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645) 文档。

## 在Google中创建再营销受众 {#creating-a-remarketing-audience-in-google}

1. 登录到您的Google Analytics。 单击 **管理员**， **帐户**， **属性**. 单击 **受众定义** 和 **受众**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. 单击 **+新建受众**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **链接配置**：链接到您的Google Adwords帐户。 **定义受众**：单击 **新建**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. 在受众生成器中，单击 **序列** 和 **查找RTP数据** 在“自定义Dimension”、“自定义变量”和“事件”下。

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
>在Google Universal Analytics：
>
>* 自定义Dimension：组织、行业、类别（《财富》500,1000强企业、全球2000强企业）、集团（企业、中小型企业）、ABM列表（指定客户列表）
>* 事件类别：RTP-Segment、RTP-Campaign、RTP-Remarketing
>* 事件标签：区段名称、促销活动名称、分段受众名称

**RTP分段受众数据的再营销受众示例**

1. 单击 **序列。**
1. 选择 **事件标签。**
1. 输入 **分段受众的名称** （如RTP中所示）。
1. 单击 **应用**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**RTP行业数据的受众示例**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. 单击 **序列**.
1. 选择 **RTP行业**.
1. 输入 **行业名称** (例如： 金融服务、教育……)。
1. 单击 **应用**.
1. 输入 **受众名称**. 单击 **保存**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## 在Google Adwords中创建再营销广告营销活动 {#create-a-remarketing-ad-campaign-in-google-adwords}

1. 登录 **Google Adwords**. 单击 **营销活动**，选择 **仅显示网络**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. 输入 **营销活动名称**，选择 **键入Remarketing。**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. 输入 **广告组名称，** 进入 **增强型CPC**，选择 **再营销列表**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. 单击保存并继续。
1. 添加图像或文本广告，然后开始再营销活动。

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [使用Web个性化数据重新定位](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [facebook中的个性化再营销](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

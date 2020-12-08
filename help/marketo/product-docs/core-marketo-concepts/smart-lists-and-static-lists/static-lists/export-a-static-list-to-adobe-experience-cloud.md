---
unique-page-id: 37356194
description: 将静态列表导出到Adobe Experience Cloud- Marketo Docs —— 产品文档
title: 将静态列表导出到Adobe Experience Cloud
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 0%

---


# 将静态列表导出到Adobe Experience Cloud {#export-a-static-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Marketo实例的HIPAA就绪部署无法使用此功能。

>[!NOTE]
>
>**先决条件**
>
>[设置Adobe Experience Cloud受众共享](http://docs.marketo.com/x/D4GMAg)

## 支持的目标应用程序 {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics **(仅** 有Adobe Audience Manager牌照)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe实时客户数据平台
* Adobe Target

## 如何导出列表 {#how-to-export-a-list}

1. 在Marketo中，查找并选择要导出的列表。

   ![](assets/one.png)

1. 单击 **列表操作** 下拉框，然后选 **择发送到Experience Cloud**。

   ![](assets/two-1.png)

1. 单击 **Audience Manager文件** “Experience Cloud文件夹”下拉框，并在中选择所需的目标文件夹。

   ![](assets/three-1.png)

1. 选择是创建新受众还是覆盖现有（在此示例中，我们将创建新的数据）。 输入新受众名称，然后单击“ **发送**”。

   ![](assets/four.png)

1. 单击 **确定**。

   ![](assets/five.png)

   >[!NOTE]
   >
   >受众会员资格最长可能需要6-8小时，才能完全填入Adobe。

## 注意事项 {#things-to-note}

**共享到Adobe Analytics**

对于同时拥有Adobe Audience Manager和Adobe Analytics的客户，此集成将允许受众从Market共享到您的Adobe Analytics报告套件，但是，在Adobe Audience Manager还需要执行一些其他配置步骤来实现这一点。 请查阅Adobe Audience Manager的文档，了解有关如何设置此设置的更多信息： [https://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html](http://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html)。

**Adobe Audience Manager客户的特征使用**

在Marketo中启动列表导出时，您会注意到Adobe Audience Manager实例中反映的以下更改：

* 对于导出列表中的所有潜在客户，Marketo将使用潜在客户的哈希电子邮件作为跨设备标识符来编写一个特征。 该特征的名称将与您在导出过程中指定的目标受众名称匹配。
* 对于Marketo已管理的所有ECID与导出列表中的Lead匹配，Marketo将使用ECID设备标识符编写一个特征。 该特征的名称将与您在导出过程中指定的目标受众名称匹配。
* Marketo还将使用ECID特征作为唯一分段标准，在Audience Manager实例中创建区段。 区段的名称将与您在导出过程中指定的目标受众名称匹配。

## 常见问题解答 {#faq}

**为什么Marketo的列表大小与Adobe的大小不同？**

在后台，受众集成通过将Marketo Munchkin cookies与相应的AdobeECID cookies同步来实现。 Marketo只能共享Marketo已同步ECID的Lead的会员资格数据。 为获得最佳效果，建议您在您感兴趣跟踪的所有页面上加载Marketo的munchkin.js跟踪脚本，并将Adobe的访客.js跟踪代码并行加载到该脚本，以便用于营销目的。

**cookie同步是如何工作的？**

当您的Marketo订阅启用Cookie同步时，Marketo的munchkin.js将尝试为您在集成设置过程中指定的AdobeIMS组织捕获和存储AdobeECID，并将这些ECID与相应的Marketo Cookie标识符匹配。 这使得Marketo的匿名用户用户档案能够丰富AdobeECID。

还需要进一步步骤来将匿名用户用户档案关联到潜在客户用户档案，潜在客户使用纯文本电子邮件进行标识。 具体如下所述： [https://docs.marketo.com/display/public/DOCS/Tracking+Anonymous+Activity+and+People](http://docs.marketo.com/display/public/DOCS/Tracking+Anonymous+Activity+and+People)。

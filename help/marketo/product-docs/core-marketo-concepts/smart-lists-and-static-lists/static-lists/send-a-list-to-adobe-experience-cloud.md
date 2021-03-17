---
unique-page-id: 37356194
description: 发送列表至Adobe Experience Cloud - Marketo Docs — 产品文档
title: 将列表发送到Adobe Experience Cloud
translation-type: tm+mt
source-git-commit: 96d6cc030ecd9d1da844fe27e1c6f62bbd181d62
workflow-type: tm+mt
source-wordcount: '787'
ht-degree: 0%

---


# 将列表发送到Adobe Experience Cloud {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Marketo实例的HIPAA就绪部署无法使用此功能。

>[!PREREQUISITES]
>
>[设置Adobe Experience Cloud受众共享](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## 支持的目标应用程序{#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics(**如果您拥有Adobe Audience Manager许可证，则仅限**)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe实时客户数据平台
* Adobe Target

## 如何发送静态列表{#how-to-send-a-static-list}

静态列表就是静态的。 除非您手动更改，否则Adobe Experience Cloud中的列表不会发生任何更改。

1. 在Marketo中，查找并选择要导出的列表。

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. 单击&#x200B;**列表操作**&#x200B;下拉框并选择&#x200B;**发送到Experience Cloud**。

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. 单击&#x200B;**Audience Manager文件夹**&#x200B;下拉列表，并在Experience Cloud中选择所需的目标文件夹。

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. 选择是创建新受众还是覆盖现有（在此示例中，我们将创建新的应用程序）。 输入新受众名称，然后单击&#x200B;**发送**。

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

1. 单击&#x200B;**确定**。

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

   >[!NOTE]
   >
   >受众会员资格最多可能需要6-8小时，才能在Adobe中完全填充内容。

## 如何发送同步的列表{#how-to-send-a-synced-list}

同步列表意味着您在Marketo中更新列表时，该更改会自动同步到Adobe Experience Cloud中的受众。

1. 在Marketo中，查找并选择要同步的列表。

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. 单击&#x200B;**列表操作**&#x200B;下拉框并选择&#x200B;**发送到Experience Cloud**。

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. 单击&#x200B;**受众库文件夹**&#x200B;下拉框，并在Experience Cloud中选择所需的目标文件夹。

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

1. 选择是创建新受众还是覆盖现有（在此示例中，我们将创建新的应用程序）。 输入新的受众名称，选中“保持受众成员身份同步”**框，然后单击“发送”**“发送”**。**

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. 单击&#x200B;**确定**。

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

## 如何停止列表同步{#how-to-stop-a-list-sync}

您可以随时停止列表同步。

1. 在Marketo中，查找并选择要停止同步的列表。

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

1. 单击&#x200B;**列表操作**&#x200B;下拉框并选择&#x200B;**停止列表同步**。

   ![](assets/send-a-list-to-adobe-experience-cloud-12.png)

1. 选择要停止同步的受众，然后单击&#x200B;**停止**。

   ![](assets/send-a-list-to-adobe-experience-cloud-13.png)

1. 单击&#x200B;**停止**&#x200B;进行确认。

   ![](assets/send-a-list-to-adobe-experience-cloud-14.png)

## 注意事项{#things-to-note}

**共享到Adobe Analytics**

对于同时拥有Adobe Audience Manager和Adobe Analytics的客户，此集成将允许受众从Market共享到您的Adobe Analytics报表包，但是，在Adobe Audience Manager中需要执行一些其他配置步骤来启用此功能。 请查看Adobe Audience Manager的文档，了解有关如何设置此设置的更多信息：[https://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html](https://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html)。

**Adobe Audience Manager客户的特征使用**

在Marketo中启动列表导出时，您会注意到Adobe Audience Manager实例中反映的以下更改：

* 对于导出列表中的所有潜在客户，Marketo将使用潜在客户的哈希电子邮件作为跨设备标识符编写一个特征。 该特征的名称将与您在导出过程中指定的目标受众名称匹配。
* 对于Marketo已管理的与导出列表中的潜在客户匹配的所有ECID，Marketo将使用ECID设备标识符编写一个特征。 该特征的名称将与您在导出过程中指定的目标受众名称匹配。
* Marketo还将使用ECID特征作为唯一的分段标准在您的Audience Manager实例中创建区段。 区段的名称将与您在导出过程中指定的目标受众名称匹配。

## 常见问题解答{#faq}

**为什么Marketo中的列表大小与Adobe中的不同？**

在后台，受众集成通过将Marketo Munchkin Cookie与相应的AdobeECID Cookie同步来工作。 Marketo只能共享Marketo已同步ECID的潜在客户的会员资格数据。 为获得最佳结果，建议您在您有兴趣跟踪的所有页面上为营销目的，并行加载Adobe的munchkin.js跟踪脚本和访客的.js跟踪代码。

**Cookie同步是如何工作的？**

为您的Marketo订阅启用Cookie同步后，Marketo的munchkin.js将尝试为您在集成设置过程中指定的AdobeIMS组织捕获和存储AdobeECID，并将这些ECID与相应的Marketo Cookie标识符匹配。 这使Marketo的匿名用户用户档案能够丰富AdobeECID。

需要进一步将匿名用户用户档案关联到潜在客户用户档案，该潜在客户使用纯文本电子邮件进行标识。 ](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md)中描述了具体的工作原理。[

**共享哪些信息？**

此集成仅共享从Marketo到Adobe的列表会员资格信息(例如，了解Lead X是列表 Y的成员)。 此集成不会将其他潜在客户属性共享给Adobe。

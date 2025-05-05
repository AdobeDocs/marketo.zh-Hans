---
unique-page-id: 37356194
description: 将列表发送到Adobe Experience Cloud - Marketo文档 — 产品文档
title: 向Adobe Experience Cloud发送列表
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
feature: Static Lists
source-git-commit: c10ecc0ccad28f2e480343acefe10f5eca2ae578
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 1%

---

# 向Adobe Experience Cloud发送列表 {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Marketo Engage实例的HIPAA就绪部署无法使用此功能。

>[!PREREQUISITES]
>
>[设置Adobe组织映射](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## 支持的目标应用程序 {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (仅当您拥有Adobe Audience Manager许可证时&#x200B;_才能获得_)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Real-time Customer Data Platform
* Adobe Target

## 如何发送静态列表 {#how-to-send-a-static-list}

静态列表就是这样，静态。 除非您手动进行更改，否则Adobe Experience Cloud中的列表不会发生任何更改。

1. 在Marketo中，找到要导出的列表。 右键单击它并选择&#x200B;**[!UICONTROL 发送至Experience Cloud]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. 单击&#x200B;**[!UICONTROL Audience Manager文件夹]**&#x200B;下拉列表，然后在Experience Cloud中选择所需的目标文件夹。

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. 选择是创建新受众还是覆盖现有受众（在本例中，我们将创建一个新受众）。 输入新的受众名称，然后单击&#x200B;**[!UICONTROL 发送]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. 单击&#x200B;**[!UICONTROL 确定]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >在Adobe中完全填充受众会员资格最多可能需要6-8小时。

## 如何发送同步列表 {#how-to-send-a-synced-list}

同步列表是指只要您更新Marketo中的列表，该更改就会自动同步到Adobe Experience Cloud中的受众。

1. 在Marketo中，找到要导出的列表。 右键单击它并选择&#x200B;**[!UICONTROL 发送至Experience Cloud]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. 单击&#x200B;**[!UICONTROL 受众库文件夹]**&#x200B;下拉列表，然后在Experience Cloud中选择所需的目标文件夹。

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. 选择是创建新受众还是覆盖现有受众（在本例中，我们将创建一个新受众）。 输入新的受众名称，选中&#x200B;**[!UICONTROL 保持受众成员资格同步]**&#x200B;框，然后单击&#x200B;**[!UICONTROL 发送]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. 单击&#x200B;**OK**。

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## 如何停止列表同步 {#how-to-stop-a-list-sync}

您可以随时停止同步列表。

1. 在Marketo中，找到并右键单击要停止同步的列表。 单击&#x200B;**[!UICONTROL 停止列表同步]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. 选择要停止同步的受众，然后单击&#x200B;**[!UICONTROL 停止]**。

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. 单击&#x200B;**[!UICONTROL 停止]**&#x200B;确认。

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## 注意事项 {#things-to-note}

**共享到Adobe Analytics**

* 对于拥有Adobe Audience Manager和Adobe Analytics的客户，此集成允许将受众从Marketo共享到Adobe Analytics报表包，但是，还需要在Adobe Audience Manager中执行一些其他配置步骤才能启用此功能。 请查阅[Adobe Audience Manager的文档](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html?lang=zh-Hans){target="_blank"}以了解有关如何设置此功能的更多信息。

* 如果列表为空，或没有具有ECID值的用户，则不会将列表名称推送到列表外部进行引用Marketo Engage。

Adobe Audience Manager客户的&#x200B;**特征使用情况**

当您在Marketo中启动列表导出时，您会注意到您的Adobe Audience Manager实例中反映了以下更改：

* 对于导出列表中的所有人员，Marketo将使用其经过哈希处理的电子邮件作为跨设备标识符来编写特征。 特征名称将与您在导出期间指定的目标受众名称匹配。
* 对于Marketo已设法与导出列表中的人员匹配的所有ECID，Marketo将使用ECID设备标识符编写特征。 特征名称将与您在导出期间指定的目标受众名称匹配。
* Marketo还将使用ECID特征作为唯一的分段标准，在Audience Manager实例中创建区段。 区段的名称将与您在导出期间指定的目标受众名称匹配。

## 常见问题解答 {#faq}

**为什么Marketo中的列表大小与Adobe中的列表大小不同？**

在本例中，受众集成是通过将Marketo Munchkin Cookie与相应的AdobeECID Cookie同步来工作的。 Marketo只能共享Marketo已为其同步ECID的人员的成员资格数据。 为了获得最佳结果，建议您在所有有兴趣跟踪的页面上同时加载Marketo的munchkin.js跟踪脚本和Adobe的visitor.js跟踪代码，以便用于营销目的。

**Cookie同步如何工作？**

为您的Marketo订阅启用Cookie同步后，Marketo的munchkin.js将尝试为您在集成设置期间指定的Adobe IMS组织捕获和存储AdobeECID，并将这些ECID与相应的Marketo Cookie标识符匹配。 这使得Marketo的匿名用户档案能够利用AdobeECID丰富内容。

还需要执行进一步步骤，将匿名用户配置文件与人员配置文件相关联，该人员配置文件使用纯文本电子邮件进行标识。 [此处](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}介绍了该功能的具体工作原理。

**共享哪些信息？**

此集成仅将列表成员资格信息从Marketo共享到Adobe（例如，知道人员X是列表Y的成员）。 没有其他人员属性通过此集成共享给Adobe。

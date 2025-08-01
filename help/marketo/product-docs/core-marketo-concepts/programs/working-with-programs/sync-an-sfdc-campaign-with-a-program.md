---
unique-page-id: 1147154
description: 将SFDC促销活动与项目同步 — Marketo文档 — 产品文档
title: 将SFDC促销活动与项目同步
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 1%

---

# 将SFDC促销活动与项目同步 {#sync-an-sfdc-campaign-with-a-program}

Marketo Engage允许您将项目与[!DNL Salesforce]营销活动同步，以维护两个系统中的相同人员列表，包括其状态。 让我们开始吧！

>[!PREREQUISITES]
>
>您需要先[启用 [!DNL Salesforce] 促销活动同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}。

>[!CAUTION]
>
>将SFDC促销活动与Marketo Engage项目同步时，将对该项目的子促销活动禁用隐式的SFDC操作(例如，添加到SFDC Campaign、同步到SFDC)。

1. 转到&#x200B;**[!UICONTROL Marketing Activities]**。

   ![](assets/login-marketing-activities-1.png)

1. 选择您的项目。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 单击&#x200B;**[!UICONTROL Program Actions]**，然后选择&#x200B;**[!UICONTROL Salesforce Campaign Sync]**。

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. 选择&#x200B;**[!UICONTROL Create New]**&#x200B;或选择现有的[!DNL Salesforce]营销活动。

   >[!TIP]
   >
   >如果选择现有[!DNL Salesforce]营销活动，请确保[与 [!DNL Salesforce] 营销活动和Marketo项目的项目状态匹配](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}。

1. 输入新营销活动的名称，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. 现在，您可以在项目摘要页面中验证Campaign同步详细信息。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   太棒了！ 现在，Marketo中的任何项目状态更改都会同步到SFDC营销活动，反之亦然。

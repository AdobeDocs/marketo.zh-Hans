---
unique-page-id: 1147154
description: 将SFDC活动与项目同步 — Marketo Docs — 产品文档
title: 将SFDC活动与项目同步
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 将SFDC活动与项目{#sync-an-sfdc-campaign-with-a-program}同步

Marketo允许您将项目与Salesforce活动同步，以便在两个系统中保持相同的人员列表，包括其状态。 开始吧！

>[!PREREQUISITES]
>
>您首先需要[启用Salesforce活动同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)。

>[!CAUTION]
>
>在将SFDC活动与Marketo项目同步时，项目的子活动将禁用隐含的SFDC操作(例如，添加到SFDC活动，同步到SFDC)。

1. 转至&#x200B;**营销活动**。

   ![](assets/login-marketing-activities-1.png)

1. 选择项目。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 单击&#x200B;**项目操作**，然后选择&#x200B;**Salesforce活动同步**。

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. 选择&#x200B;**新建**&#x200B;或选择现有的Salesforce活动。

   >[!TIP]
   >
   >如果您选择了现有的Salesforce活动，请确保[与Salesforce活动和Marketo项目的项目状态](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)匹配。

1. 输入新活动的名称，然后单击&#x200B;**保存**。

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. 现在，您可以在活动摘要页中验证项目同步详细信息。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   太棒了！ 现在，Marketo中的任何项目状态更改都会同步到SFDC活动，反之亦然。

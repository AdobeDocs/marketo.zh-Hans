---
unique-page-id: 1147154
description: 将SFDC促销活动与项目同步 — Marketo文档 — 产品文档
title: 将SFDC营销活动与项目同步
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
source-git-commit: 8781c6cf2e64543809fe697e75ae6884969a4e40
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 将SFDC营销活动与项目同步 {#sync-an-sfdc-campaign-with-a-program}

Marketo允许您将项目与Salesforce营销活动同步，以便在两个系统中保持相同的人员列表，包括其状态。 开始吧！

>[!PREREQUISITES]
>
>您需要 [启用Salesforce促销活动同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) 第一个。

>[!CAUTION]
>
>在将SFDC促销活动与Marketo计划同步时，将禁用该计划的子促销活动的隐含SFDC操作（例如，添加到SFDC促销活动、同步到SFDC）。

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-1.png)

1. 选择您的项目。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 单击 **计划操作**，然后选择 **Salesforce促销活动同步**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. 选择 **新建** 或选择现有的Salesforce营销活动。

   >[!TIP]
   >
   >如果您选择了现有的Salesforce营销活动，请确保 [匹配Salesforce营销活动和Marketo计划的项目状态](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. 输入新营销活动的名称并点击 **保存**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. 现在，您可以在项目摘要页面中验证营销活动同步详细信息。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   太棒了！ 现在，Marketo中的任何项目状态更改都会同步到SFDC促销活动，反之亦然。

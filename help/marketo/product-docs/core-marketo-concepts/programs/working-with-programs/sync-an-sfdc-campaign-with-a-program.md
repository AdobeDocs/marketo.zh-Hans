---
unique-page-id: 1147154
description: 将SFDC营销活动与项目同步 — Marketo文档 — 产品文档
title: 将SFDC Campaign与程序同步
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 将SFDC Campaign与程序同步 {#sync-an-sfdc-campaign-with-a-program}

Marketo允许您将项目与Salesforce营销活动同步，以维护两个系统中的相同人员列表，包括其状态。 让我们开始吧！

>[!PREREQUISITES]
>
>您将需要 [启用Salesforce Campaign同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) 首先。

>[!CAUTION]
>
>将SFDC营销活动与Marketo项目同步时，将对该项目的子营销活动禁用隐含的SFDC操作（例如，添加到SFDC营销活动、同步到SFDC）。

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-1.png)

1. 选择您的项目。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 单击 **项目操作**，然后选择 **Salesforce Campaign同步**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. 选择 **新建** 或选择现有的Salesforce营销活动。

   >[!TIP]
   >
   >如果选择现有Salesforce营销活动，请确保 [匹配Salesforce营销活动和Marketo项目的项目状态](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. 输入新营销活动的名称，然后单击 **保存**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. 现在，您可以在程序摘要页面中验证Campaign同步详细信息。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   太棒了！ 现在，Marketo中的任何项目状态更改都会同步到SFDC营销活动，反之亦然。

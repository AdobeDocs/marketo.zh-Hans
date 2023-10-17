---
unique-page-id: 1147031
description: 从SFDC删除人员 — Marketo文档 — 产品文档
title: 从SFDC删除人员
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# 从SFDC删除人员 {#delete-person-from-sfdc}

如果您需要从Salesforce中删除一组特定的潜在客户，但将其保留为Marketo Engage中的人员，则可以使用“从SFDC流程中删除人员”操作。

>[!NOTE]
>
>仅在与Salesforce集成时可用。

1. 在数据库中，单击要从Salesforce中删除的人员。 然后单击 **[!UICONTROL 人员操作]** 并选择 **[!DNL Salesforce]**.

   ![](assets/person-actions-salesforce.png)

1. 选择 **[!UICONTROL 从SFDC删除人员]**.

   ![](assets/delete-person-from-sfdc.png)

1. 确保 **[!UICONTROL 在Marketo中删除]** 设置是 **[!UICONTROL false]**，然后单击 **[!UICONTROL 立即运行]**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   在流程步骤运行后，您的人员将不再是Salesforce中的潜在客户，而是将保留在Marketo中。

   >[!CAUTION]
   >
   >如果您设置 **[!UICONTROL 在Marketo中删除]** 到 **[!UICONTROL true]** 删除Marketo中的人和Salesforce中的潜在客户，他们永远消失了。 无法撤消此操作。

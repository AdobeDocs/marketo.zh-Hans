---
unique-page-id: 1147031
description: 从SFDC删除人员 — Marketo文档 — 产品文档
title: 从SFDC删除人员
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# 从SFDC删除人员 {#delete-person-from-sfdc}

如果您需要从Salesforce中删除一组特定的潜在客户，但将其保留为Marketo Engage中的人员，则可以使用“从SFDC流程中删除人员”操作。

>[!NOTE]
>
>仅在与Salesforce集成时可用。

1. 在数据库中，单击要从Salesforce中删除的人员。 然后单击&#x200B;**[!UICONTROL 人员操作]**&#x200B;并选择&#x200B;**[!DNL Salesforce]**。

   ![](assets/delete-person-from-sfdc-1.png)

1. 选择&#x200B;**[!UICONTROL 从SFDC]**&#x200B;中删除人员。

   ![](assets/delete-person-from-sfdc-2.png)

1. 请确保Marketo **中的**&#x200B;删除设置为&#x200B;**[!UICONTROL false]**，然后单击&#x200B;**[!UICONTROL 立即运行]**。

   ![](assets/delete-person-from-sfdc-3.png)

   在流程步骤运行后，您的人员将不再是Salesforce中的潜在客户，而是将保留在Marketo中。

   >[!CAUTION]
   >
   >如果您将Marketo中的&#x200B;**[!UICONTROL Delete]**&#x200B;设置为&#x200B;**[!UICONTROL true]**，并从Marketo中删除人员和从Salesforce中删除潜在客户，则这些人员会永久性消失。 无法撤消此操作。

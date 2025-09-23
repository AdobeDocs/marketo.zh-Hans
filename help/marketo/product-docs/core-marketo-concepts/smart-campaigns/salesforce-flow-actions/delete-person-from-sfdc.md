---
unique-page-id: 1147031
description: 从SFDC中删除人员 — Marketo文档 — 产品文档
title: 从 SFDC 中删除人员
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 7%

---

# 从 SFDC 中删除人员 {#delete-person-from-sfdc}

如果您需要从Salesforce中删除一组特定的潜在客户，但将这些潜在客户保留为Marketo Engage中的人员，则可以使用“从SFDC中删除人员”流程操作。

>[!NOTE]
>
>仅在与[!DNL Salesforce]集成时可用。

1. 在数据库中，单击要从Salesforce中删除的人员。 然后单击&#x200B;**[!UICONTROL Person Actions]**&#x200B;并选择&#x200B;**[!DNL Salesforce]**。

   ![](assets/delete-person-from-sfdc-1.png)

1. 选择 **[!UICONTROL Delete Person from SFDC]**。

   ![](assets/delete-person-from-sfdc-2.png)

1. 确保&#x200B;**[!UICONTROL Delete in Marketo]**&#x200B;设置为&#x200B;**[!UICONTROL false]**，然后单击&#x200B;**[!UICONTROL Run Now]**。

   ![](assets/delete-person-from-sfdc-3.png)

   流程步骤运行后，您的人员将不再是[!DNL Salesforce]中的潜在客户，但将保留在Marketo中。

   >[!CAUTION]
   >
   >如果将&#x200B;**[!UICONTROL Delete in Marketo]**&#x200B;设置为&#x200B;**[!UICONTROL true]**&#x200B;并从Marketo中删除人员和Salesforce中的潜在客户，则这些人员会永久性消失。 无法撤消此操作。

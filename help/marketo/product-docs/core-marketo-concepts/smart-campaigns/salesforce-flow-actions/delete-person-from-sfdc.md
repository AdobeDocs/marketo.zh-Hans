---
unique-page-id: 1147031
description: 了解如何通过流程步骤从Salesforce中删除人员。 在潜在客户或联系人进入流程后，将其从SFDC中删除。
title: 从SFDC删除人员
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/f-Zvc4glfCtAagE314vrZjiWIcD3vaGIKmKGeZO18v0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 133
ht-degree: 0%

---

# 从SFDC删除人员 {#delete-person-from-sfdc}

如果您需要从Salesforce中删除一组特定的潜在客户，但将这些潜在客户保留为Marketo Engage中的人员，则可以使用“从SFDC中删除人员”流程操作。

>[!NOTE]
>
>仅在与[!DNL Salesforce]集成时可用。

1. 在数据库中，单击要从Salesforce中删除的人员。 然后单击&#x200B;**[!UICONTROL Person Actions]**&#x200B;并选择&#x200B;**[!DNL Salesforce]**。

   ![](assets/delete-person-from-sfdc-1.png)

1. 选择&#x200B;**[!UICONTROL Delete Person from SFDC]**。

   ![](assets/delete-person-from-sfdc-2.png)

1. 确保&#x200B;**[!UICONTROL Delete in Marketo]**&#x200B;设置为&#x200B;**[!UICONTROL false]**，然后单击&#x200B;**[!UICONTROL Run Now]**。

   ![](assets/delete-person-from-sfdc-3.png)

   流程步骤运行后，您的人员将不再是[!DNL Salesforce]中的潜在客户，但将保留在Marketo中。

   >[!CAUTION]
   >
   >如果将&#x200B;**[!UICONTROL Delete in Marketo]**&#x200B;设置为&#x200B;**[!UICONTROL true]**&#x200B;并从Marketo中删除人员和Salesforce中的潜在客户，则这些人员会永久性消失。 无法撤消此操作。

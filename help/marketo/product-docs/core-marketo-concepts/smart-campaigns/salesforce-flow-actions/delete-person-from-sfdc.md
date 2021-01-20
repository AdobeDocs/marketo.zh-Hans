---
unique-page-id: 1147031
description: 从SFDC中删除人员- Marketo Docs —— 产品文档
title: 从SFDC删除人员
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---


# 从SFDC {#delete-person-from-sfdc}中删除人员

如果您需要从Salesforce中删除一组特定的潜在客户，但将其保留为Marketo中的人员，则可以使用“从SFDC流中删除人员”操作。

>[!NOTE]
>
>仅当与Salesforce集成时可用。

1. 在数据库中，单击要从Salesforce中删除的人。 然后，单击&#x200B;**人员操作**&#x200B;并选择&#x200B;**Salesforce**。

   ![](assets/person-actions-salesforce.png)

1. 选择&#x200B;**从SFDC**&#x200B;删除人员。

   ![](assets/delete-person-from-sfdc.png)

1. 确保Marketo **中的**&#x200B;删除设置为&#x200B;**false**，然后单击&#x200B;**立即运行**。

   ![](assets/run-action-delete-lead-from-sfdc.png)

   流步骤运行后，您的人员将不再是Salesforce中的潜在客户，而将保留在Marketo中。

   >[!CAUTION]
   >
   >如果将Marketo **中的** Delete设置为&#x200B;**true**，并从Marketo中删除人员和Salesforce中的Lead，它们将永远消失。 这是无法撤消的。

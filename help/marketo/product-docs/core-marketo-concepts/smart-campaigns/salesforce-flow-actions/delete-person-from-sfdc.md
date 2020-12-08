---
unique-page-id: 1147031
description: 从SFDC中删除人员- Marketo Docs —— 产品文档
title: 从SFDC删除人员
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# 从SFDC删除人员 {#delete-person-from-sfdc}

如果您需要从Salesforce中删除一组特定的潜在客户，但将其保留为Marketo中的人员，则可以使用“从SFDC流中删除人员”操作。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>仅当与Salesforce集成时可用。

1. 在数据库中，单击要从Salesforce中删除的人。 然后，单击 **人员操作** ，并选 **择Salesforce**。

   ![](assets/person-actions-salesforce.png)

1. 选择 **从SFDC删除人员**。

   ![](assets/delete-person-from-sfdc.png)

1. 确保Marketo中 **的删除设** 置 **为false**，然后单击 **立即运行**。

   ![](assets/run-action-delete-lead-from-sfdc.png)

   流步骤运行后，您的人员将不再是Salesforce中的潜在客户，而将保留在Marketo中。

   >[!CAUTION]
   >
   >如果您在Marketo **中将** Delete **设置为True，并** 从Marketo中删除人员和Salesforce中的Lead，它们将永远消失。 这是无法撤消的。


---
unique-page-id: 2360301
description: 了解如何在Sales Insight中设置星星和火焰的分数字段。 将Marketo得分字段映射到Salesforce中的MSI显示。
title: 在 Sales Insight 中设置用于星级和火焰标识的评分字段
exl-id: 640f6d53-71ee-4a6d-b28a-82f3825b8f8e
feature: Marketo Sales Insights
source-git-commit: 03f984d4049c119267c7b2c2baa4e68c7db34ad0
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 11%

---

# 设置要在[!UICONTROL Stars]中用于[!UICONTROL Flames]和[!DNL Sales Insight]的分数字段 {#set-score-fields-to-be-used-for-stars-and-flames-in-sales-insight}

>[!NOTE]
>
>**需要管理员权限**

默认情况下，[!DNL Marketo Sales Insight]使用&#x200B;**[!UICONTROL Lead Score]**&#x200B;字段计算星星和火焰。 但是，如果您想选择其他字段，请执行以下操作：

>[!TIP]
>
>如果您还没有自定义得分字段，下面是如何[创建](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)这些字段。

>[!NOTE]
>
>**定义**
>
>* **[!UICONTROL Stars]**：星代表与其他潜在客户相比的潜在客户总分数。
>* **[!UICONTROL Flames]**：火焰代表紧迫性 — 商机分数最近发生了多少变化。
>

1. 在&#x200B;**[!UICONTROL Admin]**&#x200B;下，单击&#x200B;**[!UICONTROL Sales Insight]**。

   ![](assets/image2014-9-16-13-3a27-3a19.png)

1. 在&#x200B;**[!UICONTROL Lead Scoring Settings]**&#x200B;下，单击&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2014-9-16-13-3a27-3a33.png)

1. 选择要用于&#x200B;**[!UICONTROL Stars]**&#x200B;的字段。

   ![](assets/image2014-9-16-13-3a27-3a45.png)

1. 选择要用于&#x200B;**[!UICONTROL Flames]**&#x200B;的字段。

   ![](assets/image2014-9-16-13-3a28-3a1.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/image2014-9-16-13-3a28-3a18.png)

   >[!NOTE]
   >
   >[!DNL Sales insight]需要一些时间来重新计算。 您可以稍后查看CRM以查看星星和火焰。

   >[!MORELIKETHIS]
   >
   >[优先级、紧迫性、相对分数和最佳匹配](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)

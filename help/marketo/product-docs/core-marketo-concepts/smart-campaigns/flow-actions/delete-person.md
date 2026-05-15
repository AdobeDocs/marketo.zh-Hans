---
unique-page-id: 1147082
description: 了解如何使用流程步骤从数据库中删除人员。 从Marketo中删除符合标准的人员。
title: 删除人员
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/89EPt9SVBCuluSojdqLE4BawaPGGbzHLSmYHV9w6Uko
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 127
ht-degree: 3%

---

# 删除人员 {#delete-person}

错误的人有时会进入您的数据库。 可以使用“删除人员”流程步骤删除这些人员。

![](assets/delete-person-1.png)

>[!CAUTION]
>
>在删除人员时，也将删除其所有历史RCE数据。 无法撤消此操作。

1. 当您在流程步骤中拖动时，它也会自动设置为从您的CRM中删除。

   ![](assets/delete-person-2.png)

1. 您可以从Marketo Engage中删除，但不能从CRM中删除，如下所示：

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>从CRM _中删除此人仅适用于[!DNL Salesforce]_。 如果您从Marketo中删除人员并选择将他们保留在[!DNL Salesforce]中，则当他们的[!DNL Salesforce]记录更新时，将在Marketo中重新创建他们。

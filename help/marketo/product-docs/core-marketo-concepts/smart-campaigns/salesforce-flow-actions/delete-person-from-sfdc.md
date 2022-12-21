---
unique-page-id: 1147031
description: 从SFDC中删除人员 — Marketo文档 — 产品文档
title: 从SFDC中删除人员
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# 从SFDC中删除人员 {#delete-person-from-sfdc}

如果您需要从Salesforce中删除一组特定的潜在客户，但将它们保留为Marketo中的人员，则可以使用“从SFDC中删除人员”流程操作。

>[!NOTE]
>
>仅在与Salesforce集成时可用。

1. 在数据库中，单击要从Salesforce中删除的人员。 然后，单击 **人员操作** 选择 **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. 选择 **从SFDC中删除人员**.

   ![](assets/delete-person-from-sfdc.png)

1. 确保 **在Marketo中删除** 设置 **false**，然后单击 **立即运行**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   在流程步骤运行后，您的人员将不再是Salesforce中的潜在客户，但将保留在Marketo。

   >[!CAUTION]
   >
   >如果设置 **在Marketo中删除** to **true** 删除Marketo的人员和Salesforce的潜在客户，他们就永远消失了。 无法撤消。

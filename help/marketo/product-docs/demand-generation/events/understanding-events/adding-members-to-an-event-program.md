---
unique-page-id: 37355758
description: 将成员添加到事件程序 — Marketo文档 — 产品文档
title: 将成员添加到事件程序
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# 将成员添加到事件程序 {#adding-members-to-an-event-program}

本文仅适用于使用事件上限或事件目标的用户。

>[!CAUTION]
>
>将人员列表直接导入事件程序中，会阻止这些记录被计入目标跟踪报表和事件上限进展报表中的实际注册中。 请按照下面的说明确保记录被计数。

1. 创建并[将人员添加到静态列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md)。

1. [创建智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)。

1. 在步骤2中创建的智能营销活动的智能列表中，查找并添加&#x200B;**[!UICONTROL Member of List]**&#x200B;筛选器。

   ![](assets/three.png)

1. 查找并选择您在步骤1中创建的列表。

   ![](assets/four.png)

1. 在流程中，查找并添加&#x200B;**[!UICONTROL Change Program Status]**&#x200B;流程步骤。

   ![](assets/five.png)

1. 查找并选择您的活动计划。

   ![](assets/six.png)

1. 选择所需的状态。

   ![](assets/seven.png)

1. 在[!UICONTROL Schedule]选项卡中，单击&#x200B;**[!UICONTROL Run Once]**。

   ![](assets/eight.png)

1. 选择&#x200B;**[!UICONTROL Run Now]**&#x200B;并单击&#x200B;**[!UICONTROL Run]**。

   ![](assets/nine.png)

1. 运行智能营销策划后，成员会被添加到项目中，并计入目标跟踪和事件上限进展计算中。

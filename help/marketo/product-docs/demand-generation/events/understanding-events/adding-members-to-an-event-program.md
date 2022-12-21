---
unique-page-id: 37355758
description: 向事件计划添加成员 — Marketo文档 — 产品文档
title: 向事件程序添加成员
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# 向事件程序添加成员 {#adding-members-to-an-event-program}

本文仅适用于使用事件上限或事件目标的用户。

>[!CAUTION]
>
>将人员列表直接导入事件程序将阻止这些记录被计入目标跟踪报表和事件上限进度报表中的实际注册中。 请按照以下说明确保记录被计数。

1. 创建和 [将人员添加到静态列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [创建智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. 在您在步骤2中创建的智能营销活动的智能列表中，查找并添加 **列表成员** 过滤器。

   ![](assets/three.png)

1. 查找并选择在步骤1中创建的列表。

   ![](assets/four.png)

1. 在流程中，查找并添加 **更改程序状态** 流步骤。

   ![](assets/five.png)

1. 查找并选择您的事件项目。

   ![](assets/six.png)

1. 选择所需的状态。

   ![](assets/seven.png)

1. 在计划选项卡中，单击 **运行一次**.

   ![](assets/eight.png)

1. 选择 **立即运行** 单击 **运行**.

   ![](assets/nine.png)

1. 智能营销活动运行后，会将成员添加到项目，并将在“目标跟踪”和“事件上限进度”计算中进行计数。

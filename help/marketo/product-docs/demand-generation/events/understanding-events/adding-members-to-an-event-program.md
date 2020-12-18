---
unique-page-id: 37355758
description: 将成员添加到事件项目- Marketo Docs —— 产品文档
title: 将成员添加到事件项目
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# 将成员添加到事件项目{#adding-members-to-an-event-program}

本文仅适用于使用事件上限或事件目标的用户。

>[!CAUTION]
>
>将人员列表直接导入事件项目将阻止这些记录计入目标跟踪报表和事件上限进度报表中的实际注册。 请按照以下说明确保记录被计数。

1. 创建并[将人员添加到静态列表](http://docs.marketo.com/x/ecKt)。
1. [创建智能活动](http://docs.marketo.com/x/M4AR)。
1. 在您在步骤2中创建的智能列表的智能活动中，查找并添加列表&#x200B;**过滤器的**&#x200B;成员。

   ![](assets/three.png)

1. 查找并选择您在步骤1中创建的列表。
1. ![](assets/four.png)

1. 在“流”中，查找并添加&#x200B;**更改项目状态**&#x200B;流步骤。
1. ![](assets/five.png)

1. 查找并选择您的事件项目。

   ![](assets/six.png)

1. 选择所需状态。

   ![](assets/seven.png)

1. 在“计划”选项卡中，单击&#x200B;**运行一次**。
1. ![](assets/eight.png)

1. 选择&#x200B;**立即运行**&#x200B;并单击&#x200B;**运行**。
1. ![](assets/nine.png)

1. 智能活动运行后，成员将添加到项目，并将计入目标跟踪和事件上限进度计算。


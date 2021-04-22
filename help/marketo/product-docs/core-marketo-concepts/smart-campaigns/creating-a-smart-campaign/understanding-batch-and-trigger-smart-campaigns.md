---
unique-page-id: 2953132
description: 了解批处理和触发智能活动- Marketo文档 — 产品文档
title: 了解批处理和触发智能活动
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 了解批处理和触发智能活动{#understanding-batch-and-trigger-smart-campaigns}

智能活动有两种：批处理和触发器。

## 批智能活动{#batch-smart-campaign}

>[!NOTE]
>
>**定义**
>
>批活动在特定时间启动并同时影响特定的一组人员。 例如，向加利福尼亚州的所有人发送电子邮件。

批量智能活动在智能列表部分中仅具有过滤器（即，没有触发器）。

![](assets/batch-filter.png)

单击&#x200B;**计划**&#x200B;选项卡将确认智能活动设置为“批处理”。

![](assets/batch-c4.png)

**批智能活动**

* 可以安排重复使用，如每日、每周和每月。 你也可以让他们只跑一次。
* 在[项目计划视图](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md)上可见。 智能活动中“等待”步骤后的任何内容都不会包含在视图中。

<br> 

## 触发智能活动{#trigger-smart-campaign}

>[!NOTE]
>
>**定义**
>
>触发智能活动根据触发的事件一次影响一个人。 触发器的示例包括单击电子邮件中的链接。

如果智能活动在智能列表部分内使用至少一个触发器，则模式将自动设置为触发。

![](assets/trigger.png)

单击&#x200B;**计划**&#x200B;选项卡将确认智能活动设置为“已触发”。

![](assets/trigger2.png)

**触发智能活动**

* 无法为递归安排时间。 只能将它们设置为活动或非活动。
* 可以设置多个触发器。 但是，如果触发了任何触发器，将运行活动操作。

>[!TIP]
>
>使用[活动日志](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md)查看智能活动中发生的分步操作。 您可以在人员详细信息页面的最后一个选项卡中找到活动日志。
